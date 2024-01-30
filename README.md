# The Dojo Blueprint
Welcome to the Dojo Coding Mastermind Game Plan document. A simple and proven game-plan to become a globally competitive and talented software developer. One with the tools to live a life with time and location freedom while enjoying $3k-$20k/monthly income through a salary, freelancing or mix.

This might be one of the most important documents you ever read to drastically scale your income as a developer and improve your quality of life. A shift in mindset will be had, many call it a transformation.

It’s a very principal oriented game-plan.

I personally created this freedom centered “blueprint” based on what has worked for me and the clients I’ve worked with. 

I always like to highlight that technology is freedom IF you learn to leverage it. We are currently in one of the greatest wealth transfers in history, the emerging digital economies are right at the center of it. 

Developers are superstars. 

### Who will join the Dojo?

This repository contains the source for [The Dojo Blueprint](https://blueprint.dojo.io).

## Contribution

Every contribution, regardless of its size, plays a pivotal role in refining this blueprint.

- **General Guidelines**:
  - Focus on enhancements directly related to the blueprints's content.
  - For typos, errors, or improvements, you don't need a related issue to submit a PR.
  - Review specific areas of interest in [the repository issues](https://github.com/dbejarano820/dojo-blueprint/issues).

### Setup

1. **Rust Packages**:
   - Install the `cargo` toolchain via [rustup](https://rustup.rs/).
   - Install [mdBook](https://rust-lang.github.io/mdBook/guide/installation.html) and its translation extension:

```shell
cargo install mdbook --version 0.4.31 && cargo install mdbook-i18n-helpers --version 0.1.0
```

2. **Machine Packages**:

- For translations, install [gettext](https://www.gnu.org/software/gettext/): `sudo apt install gettext`.
- On Mac, you can use `brew install gettext` to install.

3. **Repository Operations**:

- Clone the main repository: `git clone https://github.com/dbejarano820/dojo-blueprint && cd dojo-blueprint`.
- Create and work on a branch in your fork. If you're unfamiliar, use this [guide](https://akrabat.com/the-beginners-guide-to-contributing-to-a-github-project/) for assistance.
- Once done, submit a PR to merge your edits. Ensure you tag the reviewer for feedback (`@dbejarano820`).

4. **Formatting**

- Run `npm i`
- Then after completing your documentation run `npm run format`
- Finally run `prettier --write .`

### Understanding the Book's Structure

The Dojo Blueprint is optimized for mdBook:

- `src/SUMMARY.md`: The blueprint's structural outline. For adding chapters, modify this document.
- `src/`: This directory holds individual chapters. Each is a markdown file, like `ch35.md`. Use subdirectories for added resources.
- `book.toml`: The primary configuration file (regular contributors might not need to adjust this).

### Editing Guidelines

#### Work Locally in English

Ensure all edits to Markdown files are in English.

- Use `mdbook serve` to initiate a local server. Access the book at [localhost:3000](http://localhost:3000) or append `--open` to the command to launch a browser automatically: `mdbook serve --open`.
- After editing, refresh the browser to see updates. When satisfied, push your changes through a PR.

<!-- #### Translations

Targeting a global readership, this book will undergo translations over time.

- **Initial Version Always in English**: Always write files in the `src` directory in English. This consistency allows for smooth auto-translation.
- **Translation Process**:
- Launch a local server for the intended language, e.g., `./translations.sh es`. Without specifying a language, only English translations get extracted.
- Modify the translation file of interest, like `po/es.po`. Tools like [poedit](https://poedit.net/) can be beneficial.
- Commit changes only in the `po/xx.po` file. When opening a PR, start with the prefix `i18n`.

The translation work is inspired from [Comprehensive Rust repository](https://github.com/google/comprehensive-rust/blob/main/TRANSLATIONS.md). -->

<!-- ##### Initiating a New Translation

For starting translations in a new language:

- Employ `./translations.sh new xx`, replacing `xx` with your language code. This action generates a language file.
- For updating the `xx.po` file, use `./translations.sh xx`.
- Avoid the above command if the `xx.po` file already exists (which means you are not initiating a new translation). -->
