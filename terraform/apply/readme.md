# Terraform - Apply

Runs terraform apply

## Example Usage

```yaml
  - uses: Chinilla/actions/terraform/apply@main
    with:
      workspace: vanillanet-us-west-2
      varfile: vars/vanillanet-us-west-2.tfvars
      terraform_dir: terraform
```

### Parameters

`workspace` The terraform workspace to run in. Can pass "default" if not using workspaces. [Workspace Documentation](https://www.terraform.io/language/state/workspaces).

`varfile` The vars file to pass to terraform

`terraform_dir` Path to the directory that contains the terraform configuration
