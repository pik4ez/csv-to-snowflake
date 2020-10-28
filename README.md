# CSV to Snowflake

Loads data from CSV to Snowflake. Creates a table based on CSV caption. 

## Usage

```
./csv_to_snowflake -h
```

Example:

```
csv-to-snowflake --account mf00000.eu-central-1 --user user@example.org --role sysadmin --db mydb --schema myschema --table mytable /path/to/file.csv
```

## CSV format

By default, the tool accepts "excel"-formatted CSV files:
* Comma-delimited fields.
* Lines delimited by '\r\n'.

You may change those using `--csv-delimiter` and `--csv-lineterminator` flags.

## Debug

To get the most verbose debug output, you may set `--log-level debug`.

To run in debug mode, which may perform some additional checks just for debug purposes, set the flag `--debug true`.
