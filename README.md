# Calendar app

<!-- ![banner]() -->

<!-- ![badge]()
![badge]()
[![license](https://img.shields.io/github/license/:user/:repo.svg)](LICENSE) -->
<!-- [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme) -->

A simple app for archiving, rendering, and creating calendar events

Using Sveltekit + Typescript on the frontend, keeping everything as close to 'web native' as possible.

Using a lot of AWS services for the backend: DynamoDB, S3, Amplify, Cognito, CDK, Lambda, API Gateway, KMS.


## Table of Contents

<!-- - [Security](#security) -->
- [Background](#background)
- [Install](#install)
- [Usage](#usage)
- [API](#api)
- [Contributing](#contributing)
- [License](#license)

<!-- ## Security

### Any optional sections -->

## Background

### Product Goals

1. an archiving tool - from GCal and offline to personal cloud + backups
2. a bridging tool from GCal - that allows for GCal integration whilst also removing the need to check that platform
3. a long-form personal design system and UI

### Rationale

A while ago I was really adamant about keeping a calendar of useful events. I'd add anything and everything to my calendar. I amassed a large amount of calendar event which I'd like to bring into MY OWN ecosystem.

I've always maintained a simple rule of offline online events, but this has been tricky to continue when most people are super comfortable with Google Calendar.

So the solution is in part:
- 1. an archiving tool - from GCal and offline to personal cloud + backups
- 2. a bridging tool from GCal - that allows for GCal integration whilst also removing the need to check that platform

Final consideration is something I call `personal UI` and `personal tech`. We're at a point where building the tools that are most popular is achievable by small teams. 

Equally, the UI that serve many, don't serve the individual.

I subscribe to the idea that some web services are timeless and essential: email, calendar, notes, consuming video, consuming audio. 

Yet right now we have to bounce between different brands for these things. The largest companies in the world fighting for our attention.

Why should we accept this scenario? Does it benefit us?!!

In my case I'd like to start building a `personal app suite` and as part of this a `personal design system` and a `personal UI language`. 

All systems designed for long term use (10years+) and geared around constant evolution depending on personal scenarios: disability, changes in motivation etc.

- 3. a long-form personal design system and UI



## Install

```
npm i
```

### More

See [Sveltekit install](./docs/CREATE_SVELTE_README.md).

## Usage

```
npm run dev -- --open
```

<!-- Note: The `license` badge image link at the top of this file should be updated with the correct `:user` and `:repo`. -->

<!-- ### Any optional sections -->

## API

### Goals

- Efficient archiving of past events in S3
- Built-in data storage redundancy
- Built-in hot data in DynamoDB - burstable, low cost 
- Modern DynamoDB table design
- Cognito auth
- Amplify frontend deployment and auth
- Lambda + API Gateway controllers + SQS or EventBridge is needed for queues
- CDK for infrastructure as code
- Security using KMS - encryption as rest and in-transit
- Diamond pattern testing suite - more e2e and integration, than unit tests

<!-- ### Any optional sections -->

<!-- ## More optional sections -->

## Contributing

Not accepted at present

<!-- See [the contributing file](CONTRIBUTING.md)!

PRs accepted.

Small note: If editing the Readme, please conform to the [standard-readme](https://github.com/RichardLitt/standard-readme) specification. -->

<!-- ### Any optional sections -->

## License

<!-- [MIT © Richard McRichface.](../LICENSE) -->
