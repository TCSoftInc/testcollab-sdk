
# testcollab-sdk

This SDK allows [Test Collab](https://testcollab.com/) clients to call API easily, build custom workflows, reports, and integrations with CI/CD pipelines and more.

## Installation

To install the library, use npm:

```sh
npm install testcollab-sdk
```

## Usage Example

You'll need to authenticate the client before you can use any methods.

There are 2 possible authentication methods:

a) API key: To generate API key: login to your TestCollab account and go to 'My Profile Settings' and switch to API Token tab. Click on "Generate new API token".

b) Access token: This requires logging into API programmatically with this SDK using login method which will provide a auth token. 

For the purpose of this documentation, we'll stick to the API key based authorization.


### Authentication

API Key method:

```javascript
import { Configuration, TestPlansApi, TestPlanTestCasesApi, TestPlansAssignmentApi } from 'testcollab-sdk';

let apiKey = '123456-abc';

let config = new Configuration({
        fetchApi: (url, options) => {
            // append the token to the url if no query string is present
            if (!url.includes('?')) {
                url = url + '?token=' + apiKey;
            }
            else {
                url = url + '&token=' + apiKey;
            }
            return fetch(url, options)
        },
    
    })
const testPlansApi = new TestPlansApi(config);
```


### Test Plan Add

```javascript
        const response = await testPlansApi.addTestPlan({
            testPlanPayload: {
                project: 1234,
                title: 'From SDK',
                description: 'This is a test plan is created using the Node.js SDK',
                status: 1,
                priority: 1,
                testPlanFolder: null,
                customFields: []

            }
        });

        // get the test plan id
        const testPlanId = response.id;
        console.log('Test Plan ID: ' + testPlanId)
```

### Add New Test Cases to Test Plan

```javascript
        const testPlanCases = new TestPlanTestCasesApi(config);

        const res2 = await testPlanCases.bulkAddTestPlanTestCases({
            testPlanTestCaseBulkAddPayload:
            {
                testplan: testPlanId,
                "testCaseCollection": {
                    testCases: [1, 2, 3],
                    selector: []
                }
            }
        });
        //console.log(res2)
```

### Assign test cases to a tester in test plan

```javascript
        const testPlanAssignment = new TestPlansAssignmentApi(config);
        const res3 = await testPlanAssignment.assignTestPlan({
            project: 1234,
            testplan: testPlanId,
            testPlanAssignmentPayload: {
                "executor": "me",
                "assignmentCriteria": "testCase",
                "assignmentMethod": "automatic",
                "assignment": {
                    "user": [2],
                    "testCases": {
                        "testCases": [],
                        "selector": []
                    },
                    "configuration": null
                },
                "project": 1234,
                "testplan": testPlanId
            }
        })
        console.log(res3)
```

## API Documentation

Detailed API documentation is available at [Test Collab OpenAPI specs](https://developers.testcollab.com/).

## Author

Test Collab Software LLC

## Contact Information

For support, please contact us at [support@testcollab.com](mailto:support@testcollab.com).
