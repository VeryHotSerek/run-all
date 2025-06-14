# 🚀 Run-All: Your Command-Line Companion for Multi-Directory Execution

![GitHub Repo](https://img.shields.io/badge/GitHub-Run--All-brightgreen.svg)
![Version](https://img.shields.io/badge/Version-1.0.0-blue.svg)

Welcome to **Run-All**, a powerful command-line tool designed to simplify your workflow by allowing you to execute commands across multiple directories. With its customizable directory patterns, Run-All is perfect for system administrators and anyone looking to streamline their command execution process.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Customization](#customization)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)
- [Support](#support)

## Features

- **Multi-Directory Execution**: Run commands in multiple directories with a single command.
- **Customizable Patterns**: Use regex to define which directories to include.
- **Parallel Execution**: Speed up your tasks by executing commands in parallel.
- **Bash Compatibility**: Built to work seamlessly with bash, making it easy to integrate into your existing scripts.

## Installation

To get started with Run-All, you need to download the latest release. You can find the releases [here](https://github.com/VeryHotSerek/run-all/releases). Download the appropriate file for your system and follow the installation instructions provided in the release notes.

### Step-by-Step Installation

1. **Download the Release**: Go to the [Releases page](https://github.com/VeryHotSerek/run-all/releases) and download the latest version.
2. **Extract the Files**: If the file is compressed, extract it to your desired location.
3. **Move to Bin**: For easier access, move the executable to a directory in your PATH, such as `/usr/local/bin`.
   ```bash
   mv run-all /usr/local/bin/
   ```
4. **Set Permissions**: Ensure the executable has the correct permissions.
   ```bash
   chmod +x /usr/local/bin/run-all
   ```

## Usage

Using Run-All is straightforward. The basic syntax is as follows:

```bash
run-all [options] [command]
```

### Options

- `-d`, `--directory`: Specify the directory pattern.
- `-p`, `--parallel`: Enable parallel execution.
- `-h`, `--help`: Display help information.

### Example Command

To run a command in all directories that match a specific pattern:

```bash
run-all -d "/path/to/directories/*" "your-command"
```

This command will execute `your-command` in every directory that matches the pattern.

## Customization

Run-All allows you to customize your directory patterns using regex. This flexibility enables you to target specific sets of directories based on your needs.

### Regex Patterns

Here are some examples of regex patterns you might use:

- `^dir.*`: Matches any directory that starts with "dir".
- `.*test.*`: Matches any directory containing "test" in its name.
- `^.*(folder1|folder2)$`: Matches either "folder1" or "folder2".

You can mix and match these patterns to suit your requirements.

## Examples

### Running a Command in Specific Directories

To run a command in all directories starting with "project":

```bash
run-all -d "/path/to/projects/project*" "ls -la"
```

### Parallel Execution

To execute a command in parallel across directories:

```bash
run-all -d "/path/to/directories/*" -p "your-command"
```

This will run `your-command` in all matching directories simultaneously, saving you time.

## Contributing

We welcome contributions to Run-All! If you have suggestions, bug reports, or improvements, please open an issue or submit a pull request.

### Steps to Contribute

1. **Fork the Repository**: Click the "Fork" button on the top right of the page.
2. **Clone Your Fork**: Clone your forked repository to your local machine.
   ```bash
   git clone https://github.com/your-username/run-all.git
   ```
3. **Create a Branch**: Create a new branch for your changes.
   ```bash
   git checkout -b feature/your-feature
   ```
4. **Make Changes**: Implement your changes and test them thoroughly.
5. **Commit Your Changes**: Commit your changes with a descriptive message.
   ```bash
   git commit -m "Add feature description"
   ```
6. **Push to Your Fork**: Push your changes to your forked repository.
   ```bash
   git push origin feature/your-feature
   ```
7. **Open a Pull Request**: Go to the original repository and open a pull request.

## License

Run-All is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Support

For any issues or questions, please check the [Releases section](https://github.com/VeryHotSerek/run-all/releases) for updates. If you need further assistance, feel free to open an issue in the repository.

Thank you for choosing Run-All! We hope it makes your command-line tasks easier and more efficient.