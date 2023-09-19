
<div align="center">
  <a href="https://github.com/GovA11y/getting-started">
    <img src="https://raw.githubusercontent.com/GovA11y/.github/main/assets/logos/transparent/partial.svg" alt="Logo" width="100" height="100">
  </a>

<h3 align="center">Getting Started</h3>

  <p align="center">
    This is the master installation file for GovA11y. You should be able to start this all easily from a the CLI.
    <br />
    <a href="https://github.com/GovA11y/getting-started"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/GovA11y/getting-started">View Demo</a>
    ·
    <a href="https://github.com/GovA11y/getting-started/issues">Report Bug</a>
    ·
    <a href="https://github.com/GovA11y/getting-started/issues">Request Feature</a>
  </p>
</div>

### Prerequisites

Docker

### Installation

1) Rename [`.env_template`](.env_template) to `.env` and configure accordingly.

2) Launch Docker Compose
```bash
docker compose up -d
```

3) Setup Hasura

    - Go to http://localhost:7051 and login with the `HASURA_GRAPHQL_ADMIN_SECRET` variable you set earlier.
    - Connect the Postgres Database
        - Go to [http://localhost:7051/console/data/v2/manage/database/add?driver=postgres](http://localhost:7051/console/data/v2/manage/database/add?driver=postgres)
        - Select `Connection Parameters`
        - Enter the `POSTGRES_USER` and `POSTGRES_PASSWORD` you set earlier.
        - Click Connect

