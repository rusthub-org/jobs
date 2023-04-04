# jobs.kousun.com

[中文](./README-ZH.md)

The **frontend** for https://jobs.kousun.com, a **Web Application Server built on Rust Web Stacks**: tide, async-std, fluent, graphql_client, surf, rhai, handlebars, lettre ...

> [KouSun | 蔻隼](https://kousun.com) aims to build a **multi-language** CMS(Content Management System) based on **Rust Web stacks**, with long-term upgrade and maintenance.

## Demo site

- [jobs.kousun.com - Projects Matchmaking](https://jobs.kousun.com)
- [kids.kousun.com - Kids Education](https://kids.kousun.com)
- [niqin.com - Books Platform](https://niqin.com)

## Build & run

``` Bash
git clone https://github.com/rusthub-org/jobs.kousun.com
cd jobs.kousun.com
```

Rename file `.env.example` to `.env`, or put the environment variables into a `.env` file:

```
DOMAIN=jobs.kousun.com
ADDR=127.0.0.1
PORT=7401
LOG_LEVEL=Debug

GQL_PROT=http
GQL_ADDR=127.0.0.1
GQL_PORT=8400
GQL_URI=gql
GQL_VER=v1
GIQL_VER=v1i

EMAIL_SMTP=<smtp.server>
EMAIL_FROM=<email_account>
EMAIL_USERNAME=<username>
EMAIL_PASSWORD=<password>
```

Then, build & run:

``` Bash
cargo build
cargo run # or cargo watch -x run
```

WebUI: connect to http://127.0.0.1:7401 with browser.

## Backend

- [kousun-api](https://github.com/rusthub-org/api.kousun.com)

See also:

- https://github.com/zzy/tide-async-graphql-mongodb - Clean boilerplate for graphql services, wasm/yew & handlebars frontend
- https://github.com/zzy/surfer - [WIP] Blog based on graphql services & wasm/yew
