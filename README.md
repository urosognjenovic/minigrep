## About

Minigrep is a CLI tool for searching a file for a specifed string written in Rust.

## Features

- **Modular design**: Most of the code is found in `lib.rs`, except for collecting the argument values, error handling, and calling the `run` function, which remain in `main.rs`.
- **Error handling**: Custom and descriptive errors that are handled by `main.rs`.
- **Test coverage**: Developed using the test-driven development process (TDD).
- **Case insensitive search**: Disables case sensitivity for more flexible searches.

## Usage

Clone the repo:

```
git clone https://github.com/urosognjenovic/minigrep
```

Navigate to the repo:

```
cd minigrep
```

Run the program (replace `STRING_TO_SEARCH` and `FILE_PATH` with the desired string and file path, respectively):

```
cargo run -- STRING_TO_SEARCH FILE_PATH
```

Optionally, you can enable the case insensitive search by setting the `IGNORE_CASE` env variable to true:

```
IGNORE_CASE=true cargo run -- STRING_TO_SEARCH FILE_PATH
```