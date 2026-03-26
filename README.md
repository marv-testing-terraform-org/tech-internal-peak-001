<!-- BEGIN_TF_DOCS -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_github"></a> [github](#requirement\_github) | ~> 6.0 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_github"></a> [github](#provider\_github) | 6.11.1 |
| <a name="provider_time"></a> [time](#provider\_time) | 0.13.1 |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [github_branch.my_branch](https://registry.terraform.io/providers/integrations/github/latest/docs/resources/branch) | resource |
| [github_branch_default.my_branch_default](https://registry.terraform.io/providers/integrations/github/latest/docs/resources/branch_default) | resource |
| [github_branch_protection.my_branch](https://registry.terraform.io/providers/integrations/github/latest/docs/resources/branch_protection) | resource |
| [github_repository.my_repository](https://registry.terraform.io/providers/integrations/github/latest/docs/resources/repository) | resource |
| [github_repository_custom_property.my_owner_contact](https://registry.terraform.io/providers/integrations/github/latest/docs/resources/repository_custom_property) | resource |
| [github_repository_custom_property.my_team_contact](https://registry.terraform.io/providers/integrations/github/latest/docs/resources/repository_custom_property) | resource |
| [github_repository_dependabot_security_updates.my_dependabot_security_updates](https://registry.terraform.io/providers/integrations/github/latest/docs/resources/repository_dependabot_security_updates) | resource |
| [github_repository_file.my_files](https://registry.terraform.io/providers/integrations/github/latest/docs/resources/repository_file) | resource |
| [github_team.my_team](https://registry.terraform.io/providers/integrations/github/latest/docs/resources/team) | resource |
| [github_team_repository.my_team_repository](https://registry.terraform.io/providers/integrations/github/latest/docs/resources/team_repository) | resource |
| [time_sleep.wait_for_repo](https://registry.terraform.io/providers/hashicorp/time/latest/docs/resources/sleep) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_github_organization"></a> [github\_organization](#input\_github\_organization) | This is the target GitHub organization or individual user account to manage. | `string` | n/a | yes |
| <a name="input_github_repo_client_name"></a> [github\_repo\_client\_name](#input\_github\_repo\_client\_name) | Optional.  Used for generating the repository name | `string` | n/a | yes |
| <a name="input_github_repo_delete_branch_on_merge"></a> [github\_repo\_delete\_branch\_on\_merge](#input\_github\_repo\_delete\_branch\_on\_merge) | Set to true to enable GitHub delete branch on merge for the repository | `string` | `true` | no |
| <a name="input_github_repo_description"></a> [github\_repo\_description](#input\_github\_repo\_description) | Optional.  Provide a description of the purpose of the repo. | `string` | n/a | yes |
| <a name="input_github_repo_owner_contact"></a> [github\_repo\_owner\_contact](#input\_github\_repo\_owner\_contact) | Owner contact for this repository (email, Slack channel, etc.) | `string` | n/a | yes |
| <a name="input_github_repo_prefix"></a> [github\_repo\_prefix](#input\_github\_repo\_prefix) | Optional.  Prefix used for generating the repository name | `string` | n/a | yes |
| <a name="input_github_repo_project"></a> [github\_repo\_project](#input\_github\_repo\_project) | Project identifier abbreviation, for generating the repository name | `string` | n/a | yes |
| <a name="input_github_repo_required_approving_review_count"></a> [github\_repo\_required\_approving\_review\_count](#input\_github\_repo\_required\_approving\_review\_count) | Require x number of approvals to satisfy branch protection requirements | `number` | `1` | no |
| <a name="input_github_repo_suffix"></a> [github\_repo\_suffix](#input\_github\_repo\_suffix) | Optional.  Suffix used for generating the repository name | `string` | `"001"` | no |
| <a name="input_github_repo_team_contact"></a> [github\_repo\_team\_contact](#input\_github\_repo\_team\_contact) | Team contact for this repository (email, Slack channel, etc.) | `string` | n/a | yes |
| <a name="input_github_repo_visibility"></a> [github\_repo\_visibility](#input\_github\_repo\_visibility) | Visibility type: `public`, `internal`, `private`. Set to private to create a private repository. Repositories are created as public (e.g. open source) by default. | `string` | n/a | yes |
| <a name="input_github_token"></a> [github\_token](#input\_github\_token) | Personal Access Token Value for the Github Organization | `string` | n/a | yes |

## Outputs

No outputs.
<!-- END_TF_DOCS -->