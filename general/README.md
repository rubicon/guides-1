# General Guidelines

Style and best practices that apply to all languages and frameworks.

## Philosophy

- These are not to be blindly followed; strive to understand these and ask when
  in doubt.
- Don't duplicate the functionality of a built-in library.
- Don't swallow exceptions or "fail silently."
- Don't write code that guesses at future functionality.
- Exceptions should be exceptional.
- Keep the code simple.

## Code Review

Use a linter to automatically review your GitHub pull requests for style guide
violations.

## Formatting

- Break long lines after 80 characters.
- Delete trailing spaces.
- Don't misspell.
- Use [Unix-style line endings] (`\n`).
- Use spaces around operators, except for unary operators, such as `!`.

[unix-style line endings]: http://unix.stackexchange.com/questions/23903/should-i-end-my-text-script-files-with-a-newline

## Naming

- Avoid abbreviations.
- Avoid object types in names (`user_array`, `email_method` `CalculatorClass`,
  `ReportModule`).
- Prefer naming classes after domain concepts rather than patterns they
  implement (e.g. `Guest` vs `NullUser`, `CachedRequest` vs `RequestDecorator`).
- Name the enumeration parameter the singular of the collection (`users.each { |user| greet(user) }`).
- Name variables, methods, and classes to reveal intent. This includes documentation and
  examples (e.g. don't use `foo`, `bar`, `baz` in examples).
- Treat acronyms as words in names (`XmlHttpRequest` not `XMLHTTPRequest`), even
  if the acronym is the entire name (`class Html` not `class HTML`).

## Organization

- Order methods so that caller methods are earlier in the file than the methods
  they call.
- Order methods so that methods are as close as possible to other methods they
  call.
