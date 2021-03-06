[Back to Overview](./overview.md)

# Create Work Item - Change Notes

#### 1.5.5
- Fix null reference when duplicate handling is enabled and input data for work item creation is invalid.
- Log errors to standard log output instead of debug output.

#### 1.5.4
- Fix error when trying to set iteration path to the special value {team ID}@currentIteration during work item duplicate update.

#### 1.5 3
- Fix compatibility issues with Team Foundation Server versions prior to 2018 Update 2.

#### 1.5.2
- Fix error **Cannot read property 'isNew' of null** when new work item could not be created.
.
#### 1.5.1
- Fix error **Cannot read property '...' of undefined** in output variable creation.

#### 1.5.0
- Fix an error **Cannot read property 'relations' of null**
- Output variables are now also created when duplicate handling is active and duplicates are found.
- Add new special value *CWI.WorkItemEditUrl* to access the editor URL of a work item for output variable creation.
- Special values and field names for output variable creation are now case-insensitive.
- Fix creation of output variables for identity values. Ouput variables for identity values now have the format *Display Name &lt;Uniqe Name&gt;* where unique name is the UPN for Azure DevOps Services or the domain account for Team Foundation Server/Azure DevOps Server.
- Add support for updating a single duplicate work item.

#### 1.4.0
- Add support for linking PR with WorkItem.

#### 1.3.5
- Fix issue in WIQL generation that sometimes failed the duplicate prevention.

#### 1.3.4
- Fix another issue with identity validation (failed for on-prem identities in domain format (e.g., "Some User <Domain\\SUser>")).

#### 1.3.3
- Fix an issue with identity value validation (failed for email addresses that have mixed casing).

#### 1.3.2
- Fix performance issue when testing identity values.

#### 1.3.1
- Update docs (fix link to on-prem extension).

#### 1.3.0
- Fix compatibility issue with latest Azure DevOps deployment leading to the error **VS403666: The email of the identity is not viewable**.
- Remove support for Team Foundation Server 2017 due to library incompatibility.

#### 1.2.2
- Fix bug in output variable creation that led to empty variables.

#### 1.2.1
- Remove error log message when not items to link are found.

#### 1.2.0
- Add support for creating work items in different team projects.
- Add new link option to link all work items associated with the current build/release to the created work item.

#### 1.1.1
- Fix bug in variable substitution that could lead to variables not being replaced by their actual values.
- Update extension manifest to include links to license, GitHub repository for issue tracking.
- Add YAML documentation.

#### 1.1.0
- Add support for creating work items in a team's current iteration.
- Add support for output variables.
- Fix nested variable substitution and handling of variables with equal signs (e.g., URLs).

#### 1.0.7
- Fix error in additional fields editor due to new "magic fields" in work items.

#### 1.0.5
- Fix null references when linking or preventing duplicates.

#### 1.0.4
- Update docs to reflect the new *Azure DevOps Services* brand.

#### 1.0.3
- Fix invalid handling of empty patch operations.

#### 1.0.2
- Fix input checking - Assigned To should be optional as documented.

#### 1.0.1
- Fix publisher ID.

#### 1.0.0
- Initial version
- Supports creating work items, linking new work item to build, linking new work item to other work items, preventing duplicates based on key fields.