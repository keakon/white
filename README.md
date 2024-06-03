A fork of the Black formatter but prefers single quotes.

# Installation

```sh
pip install .
```

# Development Mode

```sh
pip install -e .
```

# Usage


```sh
black {source_file_or_directory}
```

# Integration with VSCode

Install [Black Formatter](https://marketplace.visualstudio.com/items?itemName=ms-python.black-formatter) and edit the settings.json file:
```
{
    "[python]": {
        "editor.defaultFormatter": "ms-python.black-formatter",
        "editor.formatOnSave": true,
        "editor.codeActionsOnSave": {
            "source.organizeImports": "explicit"
        },
    },
    "black-formatter.path": ["/bin/black"]  // change it to the actual path
}
```