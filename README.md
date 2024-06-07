# Metabase with Docker Compose

Run [Metabase](https://www.metabase.com/) with Docker and Docker Compose,
using PostgreSQL as application database.

Based on official docker images for [PostgreSQL] and [Metabase].

## Usage

- Clone this repository.
- Copy `.env.sample` to `.env` and adjust the variables.
- Create `metanet` network to connect metabase to other docker databases.
- Start services locally using Docker Compose.

  ```shell
  $ docker network create --driver bridge metanet
  $ docker compose up
  ```

## References

https://www.metabase.com/docs/latest/operations-guide/running-metabase-on-docker.html
https://github.com/Cambalab/metabase-compose

[PostgreSQL]: https://hub.docker.com/_/postgres
[Metabase]: https://hub.docker.com/r/metabase/metabase
