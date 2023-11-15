## Update pip package

- Update the code
- Update the Dependencies in requirements.txt and in pyproject.toml, if necessary. 
```bash
pipreqs --mode no-pin --force . 
```
- Update the pyproject.toml version, and metadata, if necessary.
- Build the project:
```bash
python -m build
```
- Republish: 

```bash
twine check dist/*
twine upload -r pypi dist/*
```

- Check your package at: 
https://pypi.org/project/madenntools/

- Push changes to github, including the new .whl file for the github package