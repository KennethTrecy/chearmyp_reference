# Chearmyp
This is an experimental, general purpose, human-readable, language. In this context, general purpose
means that it can be used as a markup, programming, command, and more.

## Syntax Overview

## Origin
Some parts of the repository was based from the [repository of the parser] and [Origenne Template].

## Parser
The parser is on separate repository. Visit the [repository of the parser] for more details.

## Lexer
The lexer has been forked. Visit the [repository of the lexer] for more details.

## Usage

### Initialization (for developers)
If you want to contribute, the repository should be initialized to adhere in [Conventional Commits
specification] for organize commits and automated generation of change log.

#### Prerequisites
- [Node.js environment]
- [pnpm] (optional)

#### Instructions
1. By running the command below, all your commits will be linted to follow the [Conventional Commits
specification].
   ```
   $ npm install
   ```

   Or if you have installed [pnpm], run the following command:
   ```
   $ pnpm install
   ```
2. To generate the change log automatically, run the command below:
   ```
   $ npx changelogen --from=[tag name or branch name or commit itself] --to=master
   ```

## Notes

### License
The repository is licensed under [MIT-0].

### Want to contribute?
Read the [contributing guide] for different ways to contribute in the project.

### Author
Chearmyp Parser was created by Kenneth Trecy Tobias.

### Disclaimer
This personal project may contain references to trademarks, which are included in good faith. However, it is important to note that such references do not indicate any endorsement, affiliation, or sponsorship by the respective trademark holders unless explicitly stated.

[MIT-0]: https://github.com/KennethTrecy/origenne_template/blob/master/LICENSE
[Node.js environment]: https://nodejs.org/en/
[pnpm]: https://pnpm.io/installation
[Conventional Commits specification]: https://www.conventionalcommits.org/en/v1.0.0/
[contributing guide]: ./CONTRIBUTING.md
[repository of the lexer]: https://github.com/KennethTrecy/chearmyp_lexer
[repository of the parser]: https://github.com/KennethTrecy/chearmyp_parser
