# `ibm_schematics_job` Ansible Module

The `ibm_schematics_job` module manages IBM Cloud Schematics jobs. This module can:

- Create a new Schematics job.
- Update an existing Schematics job.
- Delete a Schematics job.
- Retrieve details of a Schematics job.

## Requirements

- `ibm-cloud-sdk-core`
- `ibm-cloud-ansible-modules`

## Parameters

- **`name`**: Name of the job (Required).
- **`resource_group`**: Resource group name (Required).
- **`action`**: Action to be performed (Required).
- **`inputs`**: Input variables for the job.

## Usage Example

```yaml
- name: Create Schematics job
  ibm_schematics_job:
    name: my_job
    resource_group: my_resource_group
    action: create
    inputs:
      - name: var1
        value: value1
