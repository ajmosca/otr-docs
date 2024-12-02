# Getting Started

The o!TR processor is a tool which generates ratings 

## Prerequisites

Install the following tools:

- [Rust](https://www.rust-lang.org/)
- [Setup Database](o-TR-Database.md)

## Environment variables

This project utilizes a `.env` file for configuring environment variables. A `env_example` file is provided for reference. The contents are as follows:

```
CONNECTION_STRING=
```

Setup the environment variables:

<procedure>
    <step>
        Rename the <code>env_example</code> file provided to <code>.env</code>.
    </step>
    <step>
        Set the <code>CONNECTION_STRING</code> to the database connection string as described <a href="Database-Setup.md">here</a>.
    </step>
</procedure>

## Processing data

Once the o!TR API and database are running and the environment variables are configured, the processor is ready to run.

Run the processor:

```Rust
cargo run -r
```