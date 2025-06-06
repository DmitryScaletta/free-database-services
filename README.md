# Free Database Services

See also [free heroku alternatives](https://github.com/DmitryScaletta/free-heroku-alternatives)

Only free tiers

| Name                                            | Type                   | Storage | Free Tier Limits (per month)  |
| ----------------------------------------------- | ---------------------- | ------- | ----------------------------- |
| [Supabase](#supabase)                           | Postgres               | 500MB   | 5GB out                       |
| [EdgeDB](#edgedb)                               | EdgeDB (Postgres)      | 1GB     | 2GiB network egress           |
| [MongoDB Atlas](#mongodb-atlas)                 | MongoDB                | 5GB     | 10GB in, 10GB out             |
| [Neon](#neon)                                   | Serverless Postgres    | 512MB   | ?                             |
| [CockroachDB](#cockroachdb)                     | Serverless Postgres    | 10GB    | 50M Request Units             |
| [Xata](#xata)                                   | Serverless Postgres    | -       | 15GB I/O+storage              |
| [TiDB Cloud Serverless](#tidb-cloud-serverless) | Serverless MySQL       | 25GB*   | 250M Request Units            |
| [Cloudflare D1](#cloudflare-d1)                 | Serverless D1 (SQLite) | 5GB     | 5M reads/day, 100k writes/day |
| [Turso](#turso)                                 | LibSQL (SQLite)        | 9GB     | 1B reads, 25M writes          |
| [SQLite Cloud](#sqlite-cloud)                   | SQLite                 | 1GB     | ?                             |
| [Vercel Postgres](#vercel-postgres)             | Serverless Postgres    | 256MB   | 60 hours compute time         |
| [Nile](#nile)                                   | Serverless Postgres    | 1GB     | 50M query tokens              |
| [Upstash](#upstash)                             | Serverless Redis       | 256MB   | 10k cmds/day, 50GB in/out     |
| [Deno KV](#deno-kv)                             | Deno KV                | 1GB     | 450k reads, 300k writes       |
| [MotherDuck](#motherduck)                       | DuckDB                 | 10GB    | 10 CU Hours Per Month         |

## Supabase

[Pricing](https://supabase.com/pricing)

* 2 Core shared CPU, 1 GB RAM
* 2 active free projects, as many as you want paused projects (500MB storage per project)
* Pausing after 1 week of inactivity
* [PostgREST](https://supabase.com/docs/guides/api), [pg_graphql](https://supabase.com/docs/guides/graphql)
* Additional features
  * Auth: 50,000 monthly active users
  * Storage: 1GB, 50MB max file size
  * Realtime: Postgres Changes, 200 Concurrent Peak Connections, 2M Messages/Month
  * Edge Functions: 500,000 Invocations, 10MB Script size, 10 Functions

## EdgeDB

[Pricing](https://www.edgedb.com/pricing)

* Free tier instance includes:
  * 1/4 compute unit (1/16 vCPU, 1/2 GiB RAM)
  * 1GiB disk space
  * 2GiB network egress


## MongoDB Atlas

[Pricing](https://www.mongodb.com/pricing) | [Free Shared Limitations](https://www.mongodb.com/docs/atlas/reference/free-shared-limitations/)

* 512MB to 5GB of storage
* You can deploy at most one M0 free cluster per Atlas project
* 250 Projects per Atlas User ([source](https://www.mongodb.com/docs/atlas/reference/atlas-limits/#organization-and-project-limits))

## Neon

[Pricing](https://neon.tech/pricing) | [Plans](https://neon.tech/docs/introduction/plans)

* 1 project w/10 branches
* 0.25 vCPU, 1GB RAM
* Always-available primary branch compute, 5 compute hours (20 active hours)/month on branch computes
* Autosuspend: Compute scales to zero after 5 minutes of inactivity
* Region availability: The Free Tier is available in all supported regions
* Advanced Postgres features: Connection pooling, logical replication, and 60+ Postgres extensions

## CockroachDB

[Pricing](https://www.cockroachlabs.com/pricing/) | [Plan a CockroachDB Serverless Cluster](https://www.cockroachlabs.com/docs/cockroachcloud/plan-your-cluster-serverless)

* All cluster activity, including SQL queries, bulk operations, and background jobs, is measured in Request Units, or RUs. An RU is an abstracted metric that represents the compute and I/O resources used by a database operation. In addition to queries that you run, background activity, such as automatic statistics to optimize your queries or connecting a changefeed to an external sink, also consumes RUs

## Xata

[Pricing](https://xata.io/pricing) | [Pricing (Docs)](https://xata.io/docs/concepts/pricing)

* The storage size represents the amount of data stored in the transactional database. Database storage in Xata encompasses not only disk space but also I/O rates and compute resources. The listed price per GB combines the costs of the three components allocated to each workspace
* Free plan: 15 parallel requests (6 primary + 9 from replicas) to the database
* Free tier: Limited to 75 requests/second (qps)
* Additional Features
  * Elasticsearch integration
  * File attachments (2GB, S3 and Cloudflare's CDN)
  * Image transformations (10k)
  * 250 AI-powered questions per workspace
  * Free plan users can request data restoration from a daily backup through our support team

## TiDB Cloud Serverless

[Pricing](https://www.pingcap.com/pricing/) | [Pricing Details](https://www.pingcap.com/tidb-serverless-pricing-details/) | [Limitations and Quotas](https://docs.pingcap.com/tidbcloud/serverless-limitations) | [MySQL Compatibility](https://docs.pingcap.com/tidbcloud/mysql-compatibility)

* Up to 5 clusters for free tier account.
* Monthly Free Quota for serverless clusters: store 5 GiB of row-based data, 5 GiB of columnar data, and consume 50 million RUs for one month.
* 25 GB of row storage, 25 GB of column storage, and 250M Request Units (RUs) for free per month for each organization.
* Unsupported MySQL features: Stored procedures and functions, Triggers, Events, User-defined functions (see [full list](https://docs.pingcap.com/tidbcloud/mysql-compatibility#unsupported-features))

## Cloudflare D1

[Pricing](https://developers.cloudflare.com/d1/platform/pricing/)

* There are no data transfer (egress) or throughput (bandwidth) charges for data accessed from D1.

## Turso

[Pricing](https://turso.tech/pricing) | [Usage & Billing](https://docs.turso.tech/help/usage-and-billing)

* Up to 500 databases
* Up to 3 locations
* Point in time restore (1 day)
* Unlimited Embedded Replicas
* Database Branching

## SQLite Cloud

[Pricing](https://sqlitecloud.io/pricing)

* Currently in beta
* Up to 0.5 vCPUs
* Up to 0.5 GB RAM
* Cold starts after 3 days of inactivity
* Unlimited Edge Functions, Unlimited Webhooks, Pub/Sub

## Vercel Postgres

[Pricing](https://vercel.com/docs/storage/vercel-postgres/usage-and-pricing) | [Limits](https://vercel.com/docs/storage/vercel-postgres/limits)

* 1 database
* 60 hours compute time (per month)
* Databases for those on Hobby plans are configured with 0.25 logical CPUs
* Compute time is calculated based on the active time of your database, multiplied by the number of CPUs available
* If there are no incoming requests for a specified duration (default 300 seconds), the database scales down to zero, effectively pausing compute time billing
* Each Postgres database uses 33MB of storage space, even before any data is stored

## Nile

[Pricing](https://www.thenile.dev/pricing)

* Query tokens are abstract units of CPU and memory used when queries are executed on the serverless compute
  * Reading one row of 1024 bytes - ~680K query tokens for 1M queries
  * Writing one row of 1024 bytes - ~1.46M query tokens for 1M queries
  * Scanning 1000 rows of 1024 bytes, return 1 - ~9M query tokens for 1M queries
* Unlimited number of databases
* Unlimited number of tenant DBs

## Upstash

[Pricing](https://upstash.com/pricing)

* 1,000 Max commands per second
* 10,000 Daily command limit
* 1MB Max request size
* 100MB Max record size
* Persistence
* REST API
* Global replication: Free tier allows max one read replica

## Deno KV

[Deno KV](https://deno.com/kv) | [Deno Deploy Pricing](https://deno.com/deploy/pricing)

* Can connect to KV from outside of Deno Deploy
* 450,000 KV read units/mo (4kb)
* 300,000 KV write units/mo (1kb)
* 1 DB region

## MotherDuck

[Pricing](https://motherduck.com/product/pricing/)

