## Metadata

name: RSpec Coding Preferences
description: Preferences for developing and maintaining RSpec code
dependencies: ruby>=3.4.8, mise, rspec, test-prof

## When to Apply

Apply these rules when developing and maintaining RSpec test suites.

## Rules for RSpec Usage

- Use `:aggregate_failures` for multiple expectations in RSpec.

- Prefer `let!` over `before` blocks for creating test data.

- When possible, set a subject with a variable name to reduce repetition in
  expect statements.

- Align the left brace of multiple, contiguous (no blank line between) let
  and let! statements to make the code more readable.

- Separate a multiline let or let! statement with a blank line. Multiline
  let or let! statements should prefer do/end rather than braces.

- If test-prof is installed, apply these rules:
  - Use `test-prof` matchers for better test coverage and performance.
  - Try to use let_it_be instead of let! for shared test data.

- Divide tests into two sections: one for normal operation (happy path) and one
  for error handling and edge cases.

- Do not nest describe blocks more than two levels deep. The first level
  is RSpec.describe, the outermost block. There can be an additional describe block
  for each section. Innermost blocks should use context or it blocks.

- It is acceptable to create a folder to decompose large test suites further.
  For example, a test suite for a controller can be organized in a folder, with
  a file for each action.

## Things to Consider

- Would the test suite benefit from the addition of FactoryBot,
  Shoulda, Faker, or other testing libraries?

- Does the RSpec configuration record failed tests so --only-failures
  can be used to re-run only a portion of the suite?

- Does the configuration record and report the slowest tests in the suite?
