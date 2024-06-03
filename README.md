A fork of the Black formatter but prefers single quotes.

# Installation

```sh
pip install .
```

# Development

```sh
pip install -e .
```

# Usage

To get started right away with sensible defaults:

```sh
black {source_file_or_directory}
```

# Integration with VSCode

Install [https://marketplace.visualstudio.com/items?itemName=ms-python.black-formatter](Black Formatter) and edit the settings.json file:
```
{
    "[python]": {
        "editor.defaultFormatter": "ms-python.black-formatter",
        "editor.formatOnSave": true,
        "editor.codeActionsOnSave": {
            "source.organizeImports": "explicit"
        },
    },
    "black-formatter.path": ["/bin/black"]  // change to the actual path
}
```
