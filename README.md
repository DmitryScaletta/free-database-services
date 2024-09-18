# Free Database Services

See also [free heroku alternatives](https://github.com/DmitryScaletta/free-heroku-alternatives)

Only free tiers

| Name                                | Type                   | Storage | Free Tier Limits (per month)  |
| ----------------------------------- | ---------------------- | ------- | ----------------------------- |
| [Supabase](#supabase)               | Postgres               | 500MB   | 5GB out                       |
| [Tembo](#tembo)                     | Postgres               | 10GB    | 1TB out                       |
| [MongoDB Atlas](#mongodb-atlas)     | MongoDB                | 5GB     | 10GB in, 10GB out             |
| [Neon](#neon)                       | Serverless Postgres    | 512MB   | ?                             |
| [CockroachDB](#cockroachdb)         | Serverless Postgres    | 10GB    | 50M Request Units             |
| [Xata](#xata)                       | Serverless Postgres    | -       | 15GB I/O+storage              |
| [Cloudflare D1](#cloudflare-d1)     | Serverless D1 (SQLite) | 5GB     | 5M reads/day, 100k writes/day |
| [Turso](#turso)                     | LibSQL (SQLite)        | 9GB     | 1B reads, 25M writes          |
| [Vercel Postgres](#vercel-postgres) | Serverless Postgres    | 256MB   | 60 hours compute time         |
| [Nile](#nile)                       | Serverless Postgres    | 10GB    | 2B reads, 20M writes          |
| [Upstash](#upstash)                 | Serverless Redis       | 256MB   | 10k cmds/day, 50GB in/out     |
| [Deno KV](#deno-kv)                 | Deno KV                | 1GB     | 450k reads, 300k writes       |

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

## Tembo

[Pricing](https://tembo.io/pricing/)

* 3 Free Instances
* 0.25 vCPU & 1 GB Memory
* Unlimited Reads/Writes
* PostgREST, pg_graphql
* [User Defined Applications](https://tembo.io/docs/tembo-cloud/application-services/custom) - deploy containers next to your Postgres instance

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

* Limit of 10 databases
* Up to 100 Tenants per workspace

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
