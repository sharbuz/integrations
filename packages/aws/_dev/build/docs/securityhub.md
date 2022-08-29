# Security Hub

The [AWS Security Hub](https://docs.aws.amazon.com/securityhub/) integration collects and parses data from AWS Security Hub REST APIs.

## Compatibility

  1. The minimum compatible version of this module is `Elastic Agent 8.4.0`.
  2. This module is tested against `AWS Security Hub API version 1.0`.

## To collect data from AWS Security Hub APIs, users must have an Access Key and a Secret Key. To create API token follow below steps:

  1. Login to https://console.aws.amazon.com/.
  2. Go to https://console.aws.amazon.com/iam/ to access the IAM console.
  3. On the navigation menu, choose Users.
  4. Choose your IAM user name.
  5. Select Create access key from the Security Credentials tab.
  6. To see the new access key, choose Show.

## Note

  1. For the current integration package, it is recommended to have interval in hours.
  2. For the current integration package, it is compulsory to add Secret Access Key and Access Key ID.

## Logs

### Findings

This is the [`securityhub_findings`](https://docs.aws.amazon.com/securityhub/1.0/APIReference/API_GetFindings.html#API_GetFindings_ResponseElements) data stream.

{{event "securityhub_findings"}}

{{fields "securityhub_findings"}}

### Insights

This is the [`securityhub_insights`](https://docs.aws.amazon.com/securityhub/1.0/APIReference/API_GetInsights.html#API_GetInsights_ResponseElements) data stream.

{{event "securityhub_insights"}}

{{fields "securityhub_insights"}}