# TILerator [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A CL tool that will be able to generate TIL posts. It will be able to convert text, snippets of code, and images to HTML format

# Features

Mandatory Features

- Provide `--version` or `-v` flag to view version
- Provide `--help` or `-h` flag to view help/usage message
- Provide a path for a file to generate an html file
- Provide a path for a directory to generate html files for each text file within folder
- Adds HTML markup tags such as `<p>...</p>` to text
- Outputs files to `./til` folder by default
- Handle markdown files

Optional Features

- Parses title from text file to enhance HTML with `<h1>...</h1>` markup tags
- Allows a custom output folder path to be passed using `--output` or `-o` flag

# Usage/Examples

```
TILerator [flag] <filePath | directoryPath>
```

Pass in a flag

```
TILerator <flag>

--> TILerator -v
```

Pass in a file path or directory path

```
TILerator <filePath | directoryPath>

--> TILerator ./examples/example1.txt
```

Use the `-o` or `--output` flag to generate html files in a custom folder

```
---> TILerator ./examples/til_Sample.txt -o ./htmlFiles
```

Use the `-c` or `--config` flag to specify all options in a TOML config file

```
---> TILerator -c config.toml ./examples/til_Sample.txt
```

## Flags

| Flag          | Description                               |
| ------------- | ----------------------------------------- |
| -v, --version | Displays version of tool                  |
| -h, --help    | Display help/usage menu                   |
| -o, --output  | Allows for custom output folder           |
| -c, --config  | Specify all options in a TOML config file |

> Custom output folder path must be placed right after `-o/--output` flag
