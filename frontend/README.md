# Frontend: web application server

The **frontend** for https://junhen.com, a **Web Application Server built on Rust Web Stacks**: tide, async-std, fluent, graphql_client, surf, rhai, handlebars, lettre ...

## Build & run

``` Bash
git clone https://github.com/rusthub-org/jobs
cd ./frontend
```

Rename file `.env.example` to `.env`, or put the environment variables into a `.env` file:

```
DOMAIN=junhen.com
ADDR=127.0.0.1
PORT=7401
LOG_LEVEL=Debug

GQL_PROT=http
GQL_ADDR=127.0.0.1
GQL_PORT=8401
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
