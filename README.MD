## steps
```bash
1. python3 -m venv venv
2. source venv/bin/activate
3. pip install sphinx
4. sphinx-quickstart docs
```
## make html file
```bash
1. cd docs
2. make html
3. make epub
4. make man
```

## create pages
```bash
1. mkdir pages
2. cd pages
3. create rst file
4. edit toctree in index.rst
5. make html
```

```bash
> Project name: ai docs
> Author name(s): victor
> Project release []: 1.1.1
> Project language [en]:
```

## add webhook
```bash
1. go to read the docs project 
2. admin
3. Integrations
4. Add webbook
5. copy the link and paste to github (setting -> webhook -> payload url)
6. python setup.py sdist (to generate dist folder)
7. pip install twine (to push to pypi)
8. twine upload dist/trial-bot-1.1.1.tar.gz (you need to register to pypi first)
```

## creating pypi
entry point: https://stackoverflow.com/questions/774824/explain-python-entry-points