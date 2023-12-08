# Test Multiple python version in virtual env

## Concept

- For poetry we have to do 
```sh
poetry env use 3.9

poetry install
pytest

poetry env use 3.10

poetry install
pytest

....
```
- How about do this 
`pyproject.toml`

```sh
[tool.<toolname>]
python_version = ["3.9", "3.10"]
```
- Run the tool which will do all of the above tests with the specified version.
