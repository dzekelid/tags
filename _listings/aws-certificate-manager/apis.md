---
name: AWS Certificate Manager
x-slug: aws-certificate-manager
description: AWS Certificate Manager is a service that lets you easily provision,
  manage, and deploy Secure Sockets Layer/Transport Layer Security (SSL/TLS) certificates
  for use with AWS services. SSL/TLS certificates are used to secure network communications
  and establish the identity of websites over the Internet. AWS Certificate Manager
  removes the time-consuming manual process of purchasing, uploading, and renewing
  SSL/TLS certificates. With AWS Certificate Manager, you can quickly request a certificate,
  deploy it on AWS resources such as Elastic Load Balancers or Amazon CloudFront distributions,
  and let AWS Certificate Manager handle certificate renewals. SSL/TLS certificates
  provisioned through AWS Certificate Manager are free. You pay only for the AWS resources
  you create to run your application.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_ACM_certificate-manager.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Tags
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-certificate-manager/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Certificate Manager API Add Tags To Certificate
  x-api-slug: aws-certificate-manager-api
  description: Adds one or more tags to an ACM Certificate.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_ACM_certificate-manager.png
  humanURL: https://aws.amazon.com/certificate-manager/
  baseURL: ://///?Action=AddTagsToCertificate
  tags: Certificate Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-certificate-manager/actionaddtagstocertificate-get-openapi.md
- name: AWS Certificate Manager API List Tags For Certificate
  x-api-slug: aws-certificate-manager-api
  description: Lists the tags that have been applied to the ACM Certificate.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_ACM_certificate-manager.png
  humanURL: https://aws.amazon.com/certificate-manager/
  baseURL: ://///?Action=ListTagsForCertificate
  tags: Certificate Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-certificate-manager/actionlisttagsforcertificate-get-openapi.md
- name: AWS Certificate Manager API Remove Tags From Certificate
  x-api-slug: aws-certificate-manager-api
  description: Remove one or more tags from an ACM Certificate.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_ACM_certificate-manager.png
  humanURL: https://aws.amazon.com/certificate-manager/
  baseURL: ://///?Action=RemoveTagsFromCertificate
  tags: Certificate Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-certificate-manager/actionremovetagsfromcertificate-get-openapi.md
- name: AWS Certificate Manager API
  x-api-slug: aws-certificate-manager-api
  description: AWS Certificate Manager is a service that lets you easily provision,
    manage, and deploy Secure Sockets Layer/Transport Layer Security (SSL/TLS) certificates
    for use with AWS services. SSL/TLS certificates are used to secure network communications
    and establish the identity of websites over the Internet. AWS Certificate Manager
    removes the time-consuming manual process of purchasing, uploading, and renewing
    SSL/TLS certificates. With AWS Certificate Manager, you can quickly request a
    certificate, deploy it on AWS resources such as Elastic Load Balancers or Amazon
    CloudFront distributions, and let AWS Certificate Manager handle certificate renewals.
    SSL/TLS certificates provisioned through AWS Certificate Manager are free. You
    pay only for the AWS resources you create to run your application.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_ACM_certificate-manager.png
  humanURL: https://aws.amazon.com/certificate-manager/
  baseURL: :///
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/aws-certificate-manager/openapi.md
x-common:
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/reference/acm/index.html
- type: x-documentation
  url: http://docs.aws.amazon.com/acm/latest/APIReference/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/certificate-manager/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=206
- type: x-getting-started
  url: https://aws.amazon.com/certificate-manager/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/certificate-manager/pricing/
- type: x-website
  url: https://aws.amazon.com/certificate-manager/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---