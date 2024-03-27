# Hello 👋
We are [Mycelial Inc.](https://mycelial.com), and we offer modern data
infrastructure for the Edge and the Cloud.

Ever worried about the security and efficiency of your data as it hops through the Cloud during ETL processes? We did too, which led us to create Mycelial.
Historically, ETL processes have been bottlenecked by the need to route data through central Cloud services (Segment, Fivetran, Airbyte), introducing latency, security concerns, and unnecessary compute costs.
Mycelial is our answer to these challenges, a SaaS control plane that orchestrates direct, point-to-point ETL pipelines, bypassing the need for central Cloud transit entirely. All you need is a Mycelial Daemon (myceliald) running, and you can remotely orchestrate ETL pipelines that move your data any which way you want.
Highlights:
* myceliald is 100% Rust and the binary is only ~20mb.
* myceliald has a constant memory footprint - <30mb! - even under significant load.
* myceliald has connectors for many of the key data services you’re already running, such as:
    * Postgres
    * SQLite
    * MySQL
    * Kafka
    * Snowflake
    * Amazon Redshift, and
    * File streaming
* Mycelial is 100% OSS and Apache 2 licensed. You are welcome to run your own Control Plane if you’d like! (link to docs for tutorials)
* Mycelial is “real-time” - as source data changes, myceliald will sync your data on the cadence you choose. No connection? myceliald keeps track of what data has already been synced to which destinations and will catch up when connection is restored.
* Mycelial gives you Apache NiFi-like speeds and securely transfers data directly between daemons. This ensures data integrity and speed without the traditional cloud overhead. Use the compute you’ve got with no extra fees!
With Mycelial, organizations achieve unparalleled data transfer efficiency, enhanced security, and significant cost savings, all while maintaining full control over their data.

Mycelial offers you an easy solution to your data movement needs.

Checkout this [README](https://github.com/mycelial/mycelial) to learn more.

If you'd like to chat about our libraries, we welcome you to join [our
Discord](https://discord.gg/mycelial) or contact us on
[twitter](https://twitter.com/@mycelial).
