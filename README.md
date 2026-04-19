# Amazon DMS

AWS Database Migration Service (AWS DMS) helps you migrate databases to AWS quickly and securely. The source database remains fully operational during the migration, minimizing downtime to applications that rely on the database. AWS DMS can migrate your data to and from the most widely used commercial and open-source databases, supporting homogeneous migrations within the same database engine and heterogeneous migrations between different engines.

- **URL:** https://aws.amazon.com/dms/
- **Run:** [![Run in Postman](https://run.pstmn.io/button.svg)](https://www.postman.com/api-evangelist/amazon-web-services/collection/)

**Tags:** AWS, Data Replication, Database, Database Migration, Migration

**Created:** 2024-01-15 | **Modified:** 2026-04-19

## APIs

- **Amazon DMS API** - Provides programmatic access to create and manage replication instances, endpoints, replication tasks, and monitor migration progress for database migrations to AWS.
  - **Base URL:** https://dms.amazonaws.com
  - **Version:** 2016-01-01
  - **OpenAPI:** [amazon-dms-openapi.yaml](openapi/amazon-dms-openapi.yaml)

### Common Properties

| Property | URL |
|---|---|
| Documentation | https://docs.aws.amazon.com/dms/latest/APIReference/ |
| Getting Started | https://aws.amazon.com/dms/getting-started/ |
| Terms of Service | https://aws.amazon.com/service-terms/ |
| Privacy Policy | https://aws.amazon.com/privacy/ |
| Sign Up | https://portal.aws.amazon.com/billing/signup |
| GitHub Organization | https://github.com/aws |
| Status Page | https://health.aws.amazon.com/health/status |

### Features

| Feature | Description |
|---|---|
| Homogeneous Migration | Migrate between databases of the same engine type with minimal conversion |
| Heterogeneous Migration | Migrate between different database engines using Schema Conversion Tool |
| Continuous Data Replication | Continuously replicate data changes using change data capture (CDC) |
| Minimal Downtime Migration | Keep source database operational during migration for high availability |
| Multi-AZ Replication | Provision replication instances across multiple Availability Zones for resilience |
| Premigration Assessment | Run automated assessments to identify migration issues before starting |

### Use Cases

| Use Case | Description |
|---|---|
| Database Consolidation | Consolidate multiple databases into a single AWS-managed database |
| Cross-Engine Migration | Migrate from Oracle or SQL Server to open-source Aurora or PostgreSQL |
| Development and Testing | Continuously replicate production data to development environments |
| Active-Active Replication | Maintain synchronized database replicas across regions for failover |
| Analytics Migration | Migrate transactional databases to analytical data warehouses like Redshift |

### Integrations

| Integration | Description |
|---|---|
| Amazon Aurora | Target Aurora MySQL and Aurora PostgreSQL for cost-efficient managed databases |
| Amazon RDS | Migrate to RDS instances for fully managed relational database hosting |
| Amazon Redshift | Migrate data warehouses or replicate transactional data for analytics |
| AWS Schema Conversion Tool | Convert database schemas for heterogeneous migrations between engine types |
| Amazon S3 | Stream migration data to S3 for archival or downstream processing |

## Artifacts

### OpenAPI

| Name | Description | File |
|---|---|---|
| Amazon DMS OpenAPI | OpenAPI 3.x specification for the Amazon DMS API | [amazon-dms-openapi.yaml](openapi/amazon-dms-openapi.yaml) |

### JSON Schema

| Schema | Description | File |
|---|---|---|
| ReplicationInstance | Managed compute instance for hosting replication tasks | [amazon-dms-replication-instance-schema.json](json-schema/amazon-dms-replication-instance-schema.json) |
| Endpoint | Source or target database endpoint | [amazon-dms-endpoint-schema.json](json-schema/amazon-dms-endpoint-schema.json) |
| ReplicationTask | Task defining data migration between endpoints | [amazon-dms-replication-task-schema.json](json-schema/amazon-dms-replication-task-schema.json) |
| Certificate | SSL certificate for encrypted migration connections | [amazon-dms-certificate-schema.json](json-schema/amazon-dms-certificate-schema.json) |
| Connection | Connection between replication instance and endpoint | [amazon-dms-connection-schema.json](json-schema/amazon-dms-connection-schema.json) |
| TableStatistics | Per-table migration progress statistics | [amazon-dms-table-statistics-schema.json](json-schema/amazon-dms-table-statistics-schema.json) |

### JSON Structure

| Schema | Description | File |
|---|---|---|
| ReplicationInstance | JSON Structure for ReplicationInstance | [amazon-dms-replication-instance-structure.json](json-structure/amazon-dms-replication-instance-structure.json) |
| Endpoint | JSON Structure for Endpoint | [amazon-dms-endpoint-structure.json](json-structure/amazon-dms-endpoint-structure.json) |
| ReplicationTask | JSON Structure for ReplicationTask | [amazon-dms-replication-task-structure.json](json-structure/amazon-dms-replication-task-structure.json) |

### JSON-LD

| Name | Description | File |
|---|---|---|
| Amazon DMS Context | JSON-LD 1.1 context for Amazon DMS types and properties | [amazon-dms-context.jsonld](json-ld/amazon-dms-context.jsonld) |

## Capabilities

### Shared API Definitions

| Name | Description | File |
|---|---|---|
| Amazon DMS API | Shared Naftiko capability definition for DMS API operations | [dms-api.yaml](capabilities/shared/dms-api.yaml) |

### Workflows

| Workflow | Description | Tools | Personas | File |
|---|---|---|---|---|
| Database Migration Management | End-to-end database migration lifecycle using AWS DMS | 14 | Database Engineer, Cloud Architect | [database-migration-management.yaml](capabilities/database-migration-management.yaml) |

## Vocabulary

| Name | Description | File |
|---|---|---|
| Amazon DMS Vocabulary | Unified taxonomy mapping operational and capability dimensions | [amazon-dms-vocabulary.yaml](vocabulary/amazon-dms-vocabulary.yaml) |

## Rules

| Name | Description | File |
|---|---|---|
| Amazon DMS Spectral Rules | Spectral governance rules for Amazon DMS API quality | [amazon-dms-spectral-rules.yml](rules/amazon-dms-spectral-rules.yml) |

## Maintainers

- Kin Lane - kin@apievangelist.com
