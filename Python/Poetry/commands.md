# All important commands for Poetry

## For poetry 2.0.0 and above, need additional package to run `poetry shell` 
`pip install poetry-plugin-shell` 

## Install poetry
`python -m pip install poetry`

## Init new shell
`poetry shell`

## Create new env
`poetry init`

## Install lock file
`poetry install`

## Install lock file with specific extras
`poetry install -E <extra_name1> -E <extra_name2>`
`poetry instal --extras "<extra_name1> <extra_name2>"`

## Install lock file with all extras
`poetry install --all-extras`

## Add new package
`poetry add <package_name>@<version_num>`

## Remove pacakge
`poetry remove <pacakge_name>`

## Add new package as part of dependency group
`poetry add <package_name> --group <optional_group>`

## Add new package as optional
`poetry add --optional <package_name>`

Manually add into extras
```
# A list of all of the optional dependencies, some of which are included in the below `extras`. They can be opted into by apps.
psycopg2 = { version = "^2.9", optional = true }
mysqlclient = { version = "^1.3", optional = true }

[tool.poetry.extras]
mysql = ["mysqlclient"]
pgsql = ["psycopg2"]
databases = ["mysqlclient", "psycopg2"]
```

## Add package as development package
`poetry add --group dev <package_name>`

## Check cache list
`poetry cache list`

## Clear specific Poetry cache
`poetry cache clear <cache_name> --all`

## Clear all Poetry caches
`poetry cache clear --all .`
