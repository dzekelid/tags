---
name: AWS Database Migration Service
x-slug: aws-database-migration-service
description: AWS Database Migration Service helps you migrate databases to AWS easily
  and securely. The source database remains fully operational during the migration,
  minimizing downtime to applications that rely on the database. The AWS Database
  Migration Service can migrate your data to and from most widely used commercial
  and open-source databases. The service supports homogenous migrations such as Oracle
  to Oracle, as well as heterogeneous migrations between different database platforms,
  such as Oracle to Amazon Aurora or Microsoft SQL Server to MySQL. It also allows
  you to stream data to Amazon Redshift from any of the supported sources including
  Amazon Aurora, PostgreSQL, MySQL, MariaDB, Oracle, SAP ASE and SQL Server, enabling
  consolidation and easy analysis of data in the petabyte-scale data warehouse. AWS
  Database Migration Service can also be used for continuous data replication with
  high-availability.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AWSDatabaseMigrationService.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Tags
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-database-migration-service/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Database Migration Service API Add Tags To Resource
  x-api-slug: aws-database-migration-service-api
  description: Adds metadata tags to a DMS resource, including replication instance,
    endpoint, security group, and migration task.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AWSDatabaseMigrationService.png
  humanURL: https://aws.amazon.com/dms/
  baseURL: ://///?Action=AddTagsToResource
  tags: Resource Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-database-migration-service/actionaddtagstoresource-get-openapi.md
- name: AWS Database Migration Service API List Tags For Resource
  x-api-slug: aws-database-migration-service-api
  description: Lists all tags for an AWS DMS resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AWSDatabaseMigrationService.png
  humanURL: https://aws.amazon.com/dms/
  baseURL: ://///?Action=ListTagsForResource
  tags: Resource Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-database-migration-service/actionlisttagsforresource-get-openapi.md
- name: AWS Database Migration Service API Remove Tags From Resource
  x-api-slug: aws-database-migration-service-api
  description: Removes metadata tags from a DMS resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AWSDatabaseMigrationService.png
  humanURL: https://aws.amazon.com/dms/
  baseURL: ://///?Action=RemoveTagsFromResource
  tags: Resource Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-database-migration-service/actionremovetagsfromresource-get-openapi.md
- name: AWS Database Migration Service API
  x-api-slug: aws-database-migration-service-api
  description: AWS Database Migration Service helps you migrate databases to AWS easily
    and securely. The source database remains fully operational during the migration,
    minimizing downtime to applications that rely on the database. The AWS Database
    Migration Service can migrate your data to and from most widely used commercial
    and open-source databases. The service supports homogenous migrations such as
    Oracle to Oracle, as well as heterogeneous migrations between different database
    platforms, such as Oracle to Amazon Aurora or Microsoft SQL Server to MySQL. It
    also allows you to stream data to Amazon Redshift from any of the supported sources
    including Amazon Aurora, PostgreSQL, MySQL, MariaDB, Oracle, SAP ASE and SQL Server,
    enabling consolidation and easy analysis of data in the petabyte-scale data warehouse.
    AWS Database Migration Service can also be used for continuous data replication
    with high-availability.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AWSDatabaseMigrationService.png
  humanURL: https://aws.amazon.com/dms/
  baseURL: :///
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-database-migration-service/openapi.md
x-common:
- type: x-documentation
  url: http://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/dms/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/dms/getting-started/
- type: x-partners
  url: https://aws.amazon.com/dms/partners/
- type: x-pricing
  url: https://aws.amazon.com/dms/pricing/
- type: x-schema-conversion
  url: https://aws.amazon.com/dms/#sct
- type: x-testimonials
  url: https://aws.amazon.com/dms/testimonials/
- type: x-website
  url: https://aws.amazon.com/dms/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---