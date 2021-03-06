## Requirements

No requirements.

## Providers

| Name | Version |
|------|---------|
| <a name="provider_random"></a> [random](#provider\_random) | 3.1.3 |

## Modules

| Name | Source | Version |
|------|--------|---------|
| <a name="module_db"></a> [db](#module\_db) | terraform-aws-modules/rds/aws | 3.1.0 |
| <a name="module_security_group"></a> [security\_group](#module\_security\_group) | terraform-aws-modules/security-group/aws | ~> 4.0 |
| <a name="module_vpc"></a> [vpc](#module\_vpc) | terraform-aws-modules/vpc/aws | ~> 3.0 |

## Resources

| Name | Type |
|------|------|
| [random_password.mysql](https://registry.terraform.io/providers/hashicorp/random/latest/docs/resources/password) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_aws_region"></a> [aws\_region](#input\_aws\_region) | n/a | `string` | n/a | yes |
| <a name="input_environment"></a> [environment](#input\_environment) | environment | `string` | n/a | yes |
| <a name="input_mysql_db_availability_zone"></a> [mysql\_db\_availability\_zone](#input\_mysql\_db\_availability\_zone) | the availability zone where db will be created | `string` | `"us-east-2a"` | no |
| <a name="input_mysql_engine"></a> [mysql\_engine](#input\_mysql\_engine) | n/a | `string` | `"mysl"` | no |
| <a name="input_mysql_engine_version"></a> [mysql\_engine\_version](#input\_mysql\_engine\_version) | n/a | `string` | `"8.0.25"` | no |
| <a name="input_mysql_family"></a> [mysql\_family](#input\_mysql\_family) | n/a | `string` | `"mysql8.0"` | no |
| <a name="input_mysql_instance_class"></a> [mysql\_instance\_class](#input\_mysql\_instance\_class) | n/a | `string` | `"db.t3.small"` | no |
| <a name="input_mysql_major_engine_version"></a> [mysql\_major\_engine\_version](#input\_mysql\_major\_engine\_version) | n/a | `string` | `"8.0"` | no |
| <a name="input_mysql_retention_period"></a> [mysql\_retention\_period](#input\_mysql\_retention\_period) | number of days to retain db backups | `number` | `7` | no |
| <a name="input_mysql_storage"></a> [mysql\_storage](#input\_mysql\_storage) | amount of GBs to allocate for each mysql instance | `number` | `20` | no |
| <a name="input_project_name"></a> [project\_name](#input\_project\_name) | project name | `string` | n/a | yes |
| <a name="input_tags"></a> [tags](#input\_tags) | Resource tags | `object({})` | `{}` | no |
| <a name="input_username"></a> [username](#input\_username) | the username of the database | `string` | `"mysql"` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_mysql_url"></a> [mysql\_url](#output\_mysql\_url) | URL MySQL |
