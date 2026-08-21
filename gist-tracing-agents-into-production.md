# Tracing agents into production: the question that matters

Code review stops at deploy. Tracing starts there.

An agent can pass every test, ship clean, and still make decisions in production nobody reviewed: which tool it called, how many times it retried, what it fed into a query. Tracing exists to make those runs visible instead of assumed.

That gap gets expensive fast. Snowflake's own usage data shows a single unfiltered Cortex AI query hitting 1.18 billion rows and generating a $5,000 charge in one call. No warning, no budget alert, the query technically correct the whole time. Standard FinOps tooling never saw it coming because it wasn't built to watch a single LLM call.

Tracing and evaluation close that gap before the query runs, not after the invoice: cost and latency analysis, regression tests before a change ships, feedback loops that catch drift while it's still cheap to fix.

The real question isn't whether your agent works. It's whether you'd know before it does something you'd have to explain.

Full course on tracing agents into production: [andreinita.co/learning/langsmith](https://andreinita.co/learning/langsmith/?utm_source=github&utm_medium=gist&utm_campaign=profile)
