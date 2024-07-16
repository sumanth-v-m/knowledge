# Manage `ibm_cm_offering_instance` Resources

## Synopsis

This module creates, updates, or deletes an `ibm_cm_offering_instance`. By default, the module will look for an existing `ibm_cm_offering_instance`.

## Requirements

- `CatalogManagementV1`

## Parameters

| Parameter              | Choices/Defaults | Comments                                                                              |
|------------------------|------------------|---------------------------------------------------------------------------------------|
| `catalog_id`           | string           | Catalog ID this instance was created from.                                            |
| `channel`              | string           | Channel to pin the operator subscription to.                                          |
| `cluster_all_namespaces` | boolean          | Choices: `true`, `false` <br> Designate to install into all namespaces.                |
| `cluster_id`           | string           | Cluster ID.                                                                           |
| `cluster_namespaces`   | list / elements=string | List of target namespaces to install into.                                            |
| `cluster_region`       | string           | Cluster region (e.g., us-south).                                                      |
| `crn`                  | string           | Platform CRN for this instance.                                                       |
| `id`                   | string           | Provisioned instance ID (part of the CRN).                                            |
| `install_plan`         | string           | Type of install plan (also known as approval strategy) for operator subscriptions. Can be either `automatic`, which automatically upgrades operators to the latest in a channel, or `manual`, which requires approval on the cluster. |
| `instance_identifier`  | string           | Version Instance identifier.                                                          |
| `kind_format`          | string           | The format this instance has (helm, operator, ova...).                                |
| `label`                | string           | The label for this instance.                                                          |
| `last_operation`       | dictionary       | The last operation performed and status.                                              |
| `message`              | string           | Additional information about the last operation.                                      |
| `operation`            | string           | Last operation performed.                                                             |
| `state_`               | string           | State after the last operation performed.                                             |
| `transaction_id`       | string           | Transaction ID from the last operation.                                               |
| `updated`              | string           | Date and time last updated.                                                           |
| `metadata`             | dictionary       | Map of metadata values for this offering instance.                                    |
| `offering_id`          | string           | Offering ID this instance was created from.                                           |
| `resource_group_id`    | string           | ID of the resource group to provision the offering instance into.                     |
| `rev`                  | string           | Cloudant revision.                                                                    |
| `schematics_workspace_id` | string        | ID of the schematics workspace, for offering instances provisioned through schematics.|
| `state`                | string           | Choices: `present` ←, `absent` <br> Should the resource be present or absent.         |
| `url`                  | string           | URL reference to this object.                                                         |
| `version`              | string           | The version this instance was installed from (not version ID).                        |
| `x_auth_refresh_token` | string           | IAM Refresh token.                                                                    |

## Examples

Examples coming soon.
