## Metadata

name: Ruby Coding Preferences
description: Preferences for developing and maintaining Ruby code
dependencies: ruby>=3.4.8, mise

## When to Apply

Apply these rules when developing and maintaining Ruby projects.

## Rules for Ruby Usage

- Order methods, functions, and variables alphabetically by name.

- Use single quotes for strings unless interpolation is required.

- Prefer early returns (also known as guard clauses)over nested conditionals.

- Use white space such as blank lines to make code more readable.
  - If a code statement spans multiple lines, add a blank line before and after the
    statement to make it easier to read.

- Use `freeze` on constant arrays and hashes.

- Class `self.` methods should appear first, followed by initialize (if
  needed), then instance methods, then private instance methods.

- If an attr_reader is not used outside of the class, define it in the private
  section of the class.

- When a method call spans multiple lines, use parentheses after the method
  name and indent each argument two spaces on subsequent lines.

- When an assignment is multiline, add a blank line before and after the
  block of code, insert a newline after the equal sign and follow other rules
  listed here to format the rest of the statement.

- Use `%w[]` for word arrays (not `%w{}`).

- Use `is_a?` instead of `kind_of?`.

- Use .tap (if possible)if a method is used to build a single return value.

- Add spaces around default parameters: `def method(arg = default)`.

- Alphabetize arrays in ransackable methods.

- Align scope arrows (`->`) vertically when there are many scopes.

- Try to align the assignment operator (`=`) vertically when there are many
  assignments in sequence.

- If Rubocop is installed, use it to enforce other coding standards. If
  Rubocop's styles conflict with these guidelines, use Rubocop's configuration
  file to override the conflicting rules, but provide an alert about the
  discrepancies.

## Resources

See the skills file for Rails Coding Preferences.
