# DeepWiki to Markdown Converter

## Overview

This project provides a command-line tool to convert DeepWiki pages into Markdown files. It fetches content from a DeepWiki page for a specified project (in the format `owner/repo`) and generates Markdown files for each page.

**Note:** Your repository must already be indexed on [DeepWiki](https://deepwiki.com/) for this tool to work.

## Installation

To install this project, simply clone the repository and install the required dependencies:

```bash
git clone https://github.com/he1senbrg/deepwiki-md
cd deepwiki-md
```

### Install Dependencies:

```bash
pip install -r requirements.txt
```

## Usage

The script can be run from the command line by specifying the project name (in the format `owner/repo`) and an optional output directory.

### Command Line Arguments:

* `project_name` (required): The DeepWiki project to convert, in the format `owner/repo`. Example: `python/cpython`.
* `out_dir` (optional): The directory where the markdown files will be saved. If not provided, the default output directory is `out`.

### Example Commands:

* Convert a DeepWiki page for the project `python/cpython` and save the markdown files in the default `out` directory:

```bash
python main.py python/cpython
```

* Convert a DeepWiki page for the project `python/cpython` and save the markdown files in a custom directory:

```bash
python main.py python/cpython custom_directory
```


# Contributing

Use **`black`** to automatically format your code.


To install `black`, run the following command:

```bash
pip install black
```

After making your changes, run the following command to format your code:

```bash
black .
```

# Disclaimer

This project is provided as-is, with no guarantees or warranties of any kind. I take no responsibility for how it is used, or any issues that may arise from its use.

If you use this tool to generate documentation for your project, please include a credit to [DeepWiki](https://deepwiki.com/) in your project's README.

# License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
