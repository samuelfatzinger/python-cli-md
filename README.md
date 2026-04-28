# python-cli

A prototype Python command-line client for Apache Stratos.

## Overview

This project contains an early command-line interface for interacting with an Apache Stratos backend. The client accepts username and password options, starts an interactive `stratos>` shell, and includes basic command interpreter and HTTP request utility code.

## Requirements

- Python 3

## Usage

Run the Stratos client with a username and password:

```bash
python cli/stratos.py --username USERNAME --password PASSWORD
```

or:

```bash
python cli/stratos.py -u USERNAME -p PASSWORD
```

After authentication input is provided, the client opens an interactive shell:

```text
stratos>
```

## Available Commands

The command interpreter currently includes a basic `add` command:

```text
add
```

This prints a confirmation message from the command interpreter.

To exit the shell, use EOF:

```text
Ctrl+D
```

## Project Structure

```text
cli/
  receivers/
  __init__.py
  cmdinterpretor.py
  stratos.py
  utils.py

LICENSE
README
```

## Notes

- This appears to be an early or prototype implementation.
- Username and password values are currently printed to the terminal.
- Utility code includes an HTTP connection to `127.0.0.1:9763` using the `/stratos` endpoint prefix.
- Compiled `.pyc` files are not included in the project structure above.

## License

This project is licensed under the Apache License 2.0. See the `LICENSE` file for details.
