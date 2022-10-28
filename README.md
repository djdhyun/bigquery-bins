# bigquery-bins

Versatile tools for maintaining BigQuery 

## Dependencies

* python3
* pip install google-cloud==0.34.0
* pip install google-cloud-bigquery==2.34.3
* google-cloud-sdk (gsutil, bq)

## Setup
* `export PATH=${this_repo}/bin:${PATH}`

## Usage

* `show_tables ${project_id}.${dataset_id}`
* `describe ${project_id}.${dataset_id}.${table_id}`
* `show_partitions ${project_id}.${dataset_id}.${table_id}`
* `jobtrack ${job_id}`
* `jobfetch` : Fetch all job names that are currently running in the activated project.
* `cat ${sql_file} | bqq` : Run `bq query` and make the output in the tsv format
* `cat ${sql_file} | bqd` : Run `bq query --dry_run=true`
