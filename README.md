# sql-review-action-example

Example for configuring the [SQL Review GitHub Action](https://github.com/marketplace/actions/sql-review).

This example configures [an action](.github/workflows/sql-review.yml) triggered when opening a PR:

1. Check against MySQL SQL rules for files under [migration/mysql](migration/mysql).
1. Check against PostgreSQL SQL rules for files under [migration/postgres](migration/postgres).
1. Check against TiDB SQL rules for files under [migration/tidb](migration/tidb).

[sql-review-override.yml](./sql-review-override.yml) defines the rule to override the [default prod review rule template](https://www.bytebase.com/sql-review-guide).
