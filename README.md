# Introduction

```
The aim of this project is to automate the SQS Creation tasks coming to SCM.
```
# Getting Started

```
Connections and Stages created for each AWS environment.
```
When you want to run this release, the values to be used for AWS SQS must be entered. The default values and their
explanations are discussed below.

## Values and Explanations to be Entered

## During Release

```
1. name: "(Optional) The name of the queue. This parameter will be as an input."
2. delay_seconds: "(Optional) The time in seconds that the delivery of all messages in the queue will be delayed."
3. visibility_timeout_seconds: (Optional) The visibility timeout for the queue. An integer from 0 to 43200 (12 hours).
The default for this attribute is 30."
4. max_message_size: "(Optional) The limit of how many bytes a message can contain before Amazon SQS rejects
it. An integer from 1024 bytes (1 KiB) up to 262144 bytes (256 KiB). The default for this attribute is 262144 (
KiB)"
5. message_retention_seconds: "(Optional) The number of seconds Amazon SQS retains a message. Integer
representing seconds, from 60 (1 minute) to 1209600 (14 days). The default for this attribute is 345600 (4 days)."
6. receive_wait_time_seconds: "(Optional) The time for which a ReceiveMessage call will wait for a message to
arrive (long polling) before returning. An integer from 0 to 20 (seconds). The default for this attribute is 0, meaning
that the call will return immediately."
```
## Default Values of the Above Variables

- name: Always start with "sqs-" prefix
- delay_seconds: 0
- visibility_timeout_seconds: 30
- max_message_size: 262144
- message_retention_seconds: 1209600
- receive_wait_time_seconds: 0


