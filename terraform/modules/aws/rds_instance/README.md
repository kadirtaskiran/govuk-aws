## Module: aws::rds_instance

Create an RDS instance


## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| allocated_storage | The allocated storage in gigabytes. | string | `10` | no |
| backup_retention_period | The days to retain backups for. | string | `7` | no |
| backup_window | The daily time range during which automated backups are created if automated backups are enabled. | string | `01:00-03:00` | no |
| create_replicate_source_db | Specifies that this resource is a Replicate database, and to use this value as the source database. This correlates to the identifier of another Amazon RDS Database to replicate | string | `0` | no |
| default_tags | Additional resource tags | map | `<map>` | no |
| engine_name | RDS engine (eg mysql, postgresql) | string | `` | no |
| engine_version | Which version of MySQL to use (eg 5.5.46) | string | `` | no |
| instance_class | The instance type of the RDS instance. | string | `db.t1.micro` | no |
| maintenance_window | The window to perform maintenance in. | string | `Mon:04:00-Mon:06:00` | no |
| multi_az | Specifies if the RDS instance is multi-AZ | string | `false` | no |
| name | The common name for all the resources created by this module | string | - | yes |
| parameter_group_name | Name of the parameter group to make the instance a member of. | string | `` | no |
| password | Password for accessing the database. | string | `` | no |
| replicate_source_db | Specifies that this resource is a Replicate database, and to use this value as the source database. This correlates to the identifier of another Amazon RDS Database to replicate | string | `false` | no |
| security_group_ids | Security group IDs to apply to this cluster | list | - | yes |
| skip_final_snapshot | Set to false to create a final snapshot when the cluster is deleted. | string | `true` | no |
| storage_type | One of standard (magnetic), gp2 (general purpose SSD), or io1 (provisioned IOPS SSD). The default is gp2 | string | `gp2` | no |
| subnet_ids | Subnet IDs to assign to the aws_elasticache_subnet_group | list | `<list>` | no |
| username | User to create on the database | string | `` | no |

## Outputs

| Name | Description |
|------|-------------|
| rds_instance_address |  |
| rds_instance_endpoint |  |
| rds_instance_id |  |
| rds_instance_resource_id |  |
| rds_replica_address |  |
| rds_replica_endpoint |  |
| rds_replica_id |  |
| rds_replica_resource_id |  |
