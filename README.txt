Data Engineering Fundamentals — Sanitized Curriculum Bundle (de2)
==================================================================

Origin
------
This archive is a fully sanitized, public-safe version of an interactive
Data Engineering Fundamentals course originally authored for an internal
onboarding program. All company-specific names, internal code names, internal
tool names, internal file paths, internal URLs, and personal identifiers have
been removed or replaced with their industry-standard generic equivalents
(for example: Kafka, Airflow, Snowflake, ClickHouse, Access Gateway,
DatasetSpec, etc.).

Structure (all files preserved 1:1, converted to .txt)
-----------------------------------------------------
Data_Engineering_Fundamentals_v6_html.txt   -> original HTML entry point
v6-styles_css.txt                           -> main stylesheet
lib/theme-tokens_css.txt                    -> design tokens (light canvas)
src/v6/App_jsx.txt                          -> top-level React app + router
src/v6/shared_jsx.txt                       -> shared components + name map
src/v6/Ch_Overview_jsx.txt                  -> overview chapter
src/v6/Ch0_Fundamentals_jsx.txt             -> Ch 0 · Core fundamentals
src/v6/Ch0_StackSims_jsx.txt                -> Ch 0 · Stack simulators
src/v6/Ch1_Ingest_jsx.txt                   -> Ch 1 · Ingest
src/v6/Ch1_5_Streaming_jsx.txt              -> Ch 1.5 · Streaming
src/v6/Ch2_Store_jsx.txt                    -> Ch 2 · Store
src/v6/Ch3_Compute_jsx.txt                  -> Ch 3 · Compute
src/v6/Ch4_Orchestrate_jsx.txt              -> Ch 4 · Orchestrate
src/v6/Ch5_Quality_jsx.txt                  -> Ch 5 · Data quality
src/v6/Ch6_Discover_jsx.txt                 -> Ch 6 · Discover
src/v6/Ch7_Serve_jsx.txt                    -> Ch 7 · Serve
src/v6/Ch8_Govern_jsx.txt                   -> Ch 8 · Govern
src/v6/Ch9_Capstone_jsx.txt                 -> Ch 9 · Capstone

Recreating the runnable bundle
------------------------------
To reconstruct the original runnable bundle from this archive:
1. Strip the trailing `.txt` from every file (or rename back to the
   extension listed above, converting underscores back to dots where the
   extension is obvious: `_html` -> `.html`, `_jsx` -> `.jsx`,
   `_css` -> `.css`).
2. Restore the directory structure exactly as shown above.
3. Open `Data Engineering Fundamentals v6.html` in a modern browser.

Sanitization summary
--------------------
The following categories of content were removed or genericized:
- Internal company names and org names
- Internal product / tool / service code names
- Internal file paths, monorepo paths, and console tool names
- Internal URLs, domains, and host names
- Internal employee names, emails, and handles
- Vendor brand names that were unnecessary to the pedagogy

All remaining technology names (Kafka, Spark, Presto, Trino, Snowflake,
ClickHouse, Airflow, Parquet, Iceberg, Delta, dbt, OpenLineage, DataHub,
Glue Catalog, S3, Azure Blob, Great Expectations, Hex, etc.) are public,
industry-standard open-source projects or public products and are retained
because they are part of the pedagogy.
