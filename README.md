# Yap API Framework
Next-gen API framework with low-code approach on AWS Serverless

## Introduction

Yap is a new web framework designed by the team Young App, which aims to be a smaller, more expressive, and more robust foundation for API management and automation workflows with low-code approach and security. By leveraging async functions, Yap allows you to ditch callbacks and greatly increase error-handling and policies. provides an elegant suite of methods that make writing servers fast and enjoyable. Yap is based on Webhooks and HTTP.

## Motivation

The Young App Platform (YAP) helps to automate business workflows across cloud and on-premise apps providing employees with prompt communication and building in teams advanced collaboration. For example, YAP automates quotes processing for cash business, which may involve multiple apps (AWS, HelloSign, Stripe, etc.).

#### Automation and low-code

Without automated integration, organizations cannot leverage the full power of data in multiple applications, for example, to re-enter data in applications or constantly switch context across applications to accomplish tasks.

YAP combines the enterprise-grade workflow automation platform and ease of use expected from client apps supporting both cloud-based and on-premise systems.

#### Designed on AWS Lambda and Cloud providers Solutions

Serverless computing is a cloud-computing execution model in which the cloud provider runs the server, and dynamically manages the allocation of machine resources. Yap use Serverless Framework,  free and open-source web framework written using Node.js. Serverless is the first framework developed for building applications on AWS Lambda, a serverless computing platform provided by Amazon as a part of Amazon Web

## Features

#### API Management

API management is the process of creating and publishing web application programming interfaces (APIs), enforcing their usage policies, controlling access, nurturing the subscriber community, collecting and analyzing usage statistics, and reporting performance. API Management provides the core competencies to ensure a successful API program through developer engagement, business insights, analytics, security, and protection.

#### API policies

It’s important to realize that exposing your API services makes easier to manage them. Why? When you keep your API policies separate, you ensure control over their performance and delivery. Independence is the key to your API policies’ success and future deployment.

Further, it’s important to modernize your API strategy. Keeping API well-structured prevents overexposing API that results in stucking in little things. Unifying API policies simplifies API management.

## Application

A Yap application is an object containing an array of middleware functions and policies which are composed and executed in a stack-like manner upon request. Yap is similar to many other middleware systems that you may have encountered such as Koa, Connect.

The obligatory hello world application:

```
const Yap = require('@youngapp/yap');
const app = new Yap();

app.use(async ctx => {
  ctx.body = 'Hello World';
});

export default app
```