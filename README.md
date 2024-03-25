# CLI Code Packer

This Command Line Interface (CLI) tool allows you to package code files into a single file using various options and commands. It is developed in C# using the System.CommandLine library.

## Installation
1. Clone the repository to your local machine.
2. Build the project using Visual Studio or `dotnet build`.

## Usage
1. Ensure the CLI executable is added to the PATH environment variable for easy access.
2. Run the CLI application using the short name: ```cli```.
3. Use the following commands for packaging files and creating response files:

### Command: bundle
```bash
shortname bundle --language [all/certain languages] --output [bundle filename] --note [true/false] --sort [alphabet/code type] --remove-empty-lines [true/false] --author [name]
```

#### Options:
- `--language` (`-l`): List of programming languages to include in the bundle. Type `all` to include all code files.
- `--output` (`-o`): Specify the name of the exported bundle file.
- `--note` (`-n`): Include source code as a comment in the bundle file.
- `--sort` (`-s`): Specify the order of copying the code files (default: alphabetically).
- `--remove-empty-lines` (`-r`): Delete empty lines from the source code.
- `--author` (`-a`): Register the name of the creator of the file.

### Command: create-rsp
```bash
cli create-rsp
```
This command will guide you through creating a response file with all the required options for the `bundle` command.

## Setting Up CLI in Path
1. Open Control Panel -> System -> Advanced System Settings -> Environment Variables...
2. Edit the Path variable and add the location of the CLI executable.
3. Now you can run the CLI commands from any location in the command prompt.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
