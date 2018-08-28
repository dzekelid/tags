---
name: Pay Run
x-slug: pay-run
description: PayRun.io is a RESTful payroll and auto enrolment API built by developers
  for developers. It is a 100% compliant solution hosted in our own private cloud,
  providing realtime payroll calculations and regulatory reporting to HMRC.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/payrun-logo.jpeg
x-kinRank: "7"
x-alexaRank: "0"
tags: Tags
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/apis.md
specificationVersion: "0.14"
apis:
- name: Pay Run.IO Get all employee tags
  x-api-slug: pay-run-io
  description: Gets all the tags from the employee
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/payrun-logo.jpeg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io////Employer/{EmployerId}/Employee/{EmployeeId}/Tags
  tags: Employee,Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/employeremployeridemployeeemployeeidtags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/employeremployeridemployeeemployeeidtags-get-openapi.md
- name: Pay Run.IO Get all employee revision tags
  x-api-slug: pay-run-io
  description: Gets all the tags from the employee revision
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/payrun-logo.jpeg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io////Employer/{EmployerId}/Employee/{EmployeeId}/Tags/{EffectiveDate}
  tags: Employee,Revision,Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/employeremployeridemployeeemployeeidtagseffectivedate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/employeremployeridemployeeemployeeidtagseffectivedate-get-openapi.md
- name: Pay Run.IO Get all employee tags
  x-api-slug: pay-run-io
  description: Gets all the employee tags
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/payrun-logo.jpeg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io////Employer/{EmployerId}/Employees/Tags
  tags: Employee,Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/employeremployeridemployeestags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/employeremployeridemployeestags-get-openapi.md
- name: Pay Run.IO Get all pay code tags
  x-api-slug: pay-run-io
  description: Gets all the tags from the pay code
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/payrun-logo.jpeg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io////Employer/{EmployerId}/PayCode/{PayCodeId}/Tags
  tags: Pay,Code,Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/employeremployeridpaycodepaycodeidtags-get-openapi.md
- name: Pay Run.IO Get all pay code tags
  x-api-slug: pay-run-io
  description: Gets all the pay code tags
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/payrun-logo.jpeg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io////Employer/{EmployerId}/PayCodes/Tags
  tags: Pay,Code,Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/employeremployeridpaycodestags-get-openapi.md
- name: Pay Run.IO Get all pay run tags
  x-api-slug: pay-run-io
  description: Gets all the tags from the pay run
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/payrun-logo.jpeg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io////Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRun/{PayRunId}/Tags
  tags: Pay,Run,Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/employeremployeridpayschedulepayscheduleidpayrunpayrunidtags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/employeremployeridpayschedulepayscheduleidpayrunpayrunidtags-get-openapi.md
- name: Pay Run.IO Get all pay run tags
  x-api-slug: pay-run-io
  description: Gets all the pay run tags
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/payrun-logo.jpeg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io////Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRuns/Tags
  tags: Pay,Run,Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/employeremployeridpayschedulepayscheduleidpayrunstags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/employeremployeridpayschedulepayscheduleidpayrunstags-get-openapi.md
- name: Pay Run.IO Get all pay schedule tags
  x-api-slug: pay-run-io
  description: Gets all the tags from the pay schedule
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/payrun-logo.jpeg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io////Employer/{EmployerId}/PaySchedule/{PayScheduleId}/Tags
  tags: Pay,Schedule,Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/employeremployeridpayschedulepayscheduleidtags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/employeremployeridpayschedulepayscheduleidtags-get-openapi.md
- name: Pay Run.IO Get all pay schedule tags
  x-api-slug: pay-run-io
  description: Gets all the pay schedule tags
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/payrun-logo.jpeg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io////Employer/{EmployerId}/PaySchedules/Tags
  tags: Pay,Schedule,Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/employeremployeridpayschedulestags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/employeremployeridpayschedulestags-get-openapi.md
- name: Pay Run.IO Get all employer tags
  x-api-slug: pay-run-io
  description: Gets all the tags from the employer
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/payrun-logo.jpeg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io////Employer/{EmployerId}/Tags
  tags: Employer,Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/employeremployeridtags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/employeremployeridtags-get-openapi.md
- name: Pay Run.IO Get all employer revision tags
  x-api-slug: pay-run-io
  description: Gets all the tags from the employer revision
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/payrun-logo.jpeg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io////Employer/{EmployerId}/Tags/{EffectiveDate}
  tags: Employer,Revision,Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/employeremployeridtagseffectivedate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/employeremployeridtagseffectivedate-get-openapi.md
- name: Pay Run.IO Get all employer tags
  x-api-slug: pay-run-io
  description: Gets all the employer tags
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/payrun-logo.jpeg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io////Employers/Tags
  tags: Employer,Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/employerstags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/employerstags-get-openapi.md
- name: Pay Run.IO
  x-api-slug: pay-run-io
  description: PayRun.io is a RESTful payroll and auto enrolment API built by developers
    for developers. It is a 100% compliant solution hosted in our own private cloud,
    providing realtime payroll calculations and regulatory reporting to HMRC.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/payrun-logo.jpeg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/pay-run/openapi.md
x-common:
- type: x-website
  url: http://www.payrun.io
- type: x-documentation
  url: https://developer.payrun.io/docs/home/index.html
- type: x-twitter
  url: https://twitter.com/PayRun_io
- type: x-website
  url: http://api.test.payrun.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---