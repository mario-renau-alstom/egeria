<!-- SPDX-License-Identifier: Apache-2.0 -->
<!-- Copyright Contributors to the Egeria project. -->


# Repository origin test case

Validate the retrieval of the server origin descriptor from the open metadata repository.

## Operation

This test uses the getServerOrigin operation (`../open-metadata/admin-services/users/{userId}/servers/{serverName}/server-origin`)
operation to test that the repository knows its origin descriptor.

## Assertions

* **repository-origin-01** Origin descriptor retrieved from repository.

   The origin descriptor has successfully been retrieved from the server.
If this assertion fails, check that the server is started and the
open metadata services are activated.

## Discovered properties

* **Repository origin id** descriptive name for the server implementation

## Example output

```json
{
      "class" : "OpenMetadataTestCaseResult",
      "testCaseId" : "repository-origin",
      "testCaseName" : "Repository origin test case",
      "testCaseDescriptionURL" : "https://odpi.github.io/egeria/open-metadata-compliance-suite/docs/origin-workbench/repository-origin-test-case.md",
      "successMessage" : "Repository origin descriptor successfully retrieved",
      "successfulAssertions" : [ "Origin descriptor retrieved from repository." ],
      "unsuccessfulAssertions" : [ ],
      "discoveredProperties" : {
        "Repository origin id" : "Egeria OMAG Server"
      }
}
```