## Setting Repository Credentials
`poetry config http-basic.<repo_name> <username> <password>`

```bash
export POETRY_PYPI_TOKEN_<REPO_NAME>=my-token
export POETRY_HTTP_BASIC_<REPO_NAME>_USERNAME=<username>
export POETRY_HTTP_BASIC_<REPO_NAME>_PASSWORD=<password>
```