## Metadata

name: Rails Preferences
description: Preferences for developing and maintaining Rails code
dependencies: ruby>=3.4.8, mise

## When to Apply

Apply these rules when developing and maintaining Rails code.

## Rules for Rails Usage

- Try to keep things alphabetical within a section, such as all of the
  `has_many` statements.

- Put a blank line after all associations are defined.

- Put a blank line after all validations are defined.

- Delegations should go after modules are included.

- Associations should appear after delegations and before validations.

- accepts_nested_attributes_for should appear after validations.

- Scopes should appear after accepts_nested_attributes_for.

- When organizing Rails model files, follow this order:

  1. Schema comment (annotate gem).
  2. Module includes.
  3. Constants.
  4. Delegates.
  5. Gems/Plugins (has_paper_trail, has_secure_token, etc.).
  6. Callbacks (alphabetized: after_*, before_*, around_*).
  7. Associations.
    - belongs_to (alphabetized).
    - has_one.
    - has_many.
    - has_and_belongs_to_many.
  8. Validations.
    - validates (alphabetized by attribute).
    - validate (alphabetized by method name).
  9. Scopes (alphabetized).
  10. Class methods (self.) - alphabetized.
  11. Instance methods - alphabetized.
  12. Ransackable methods (ransackable_associations, ransackable_attributes).
  13. Private methods - alphabetized.

## Resources

See the skills file for Ruby Coding Preferences.

## JavaScript/Vue

- Order computed properties alphabetically.
- Order imports alphabetically within groups.
- Use arrow functions for callbacks.

## Vue

- Try to add whitespace between elements that make up sections to make things
  easier to read.
- Order the const assignment statements alphabetically when possible.

## Testing

- Use `:aggregate_failures` for multiple expectations in RSpec.
- Prefer `let!` over `before` blocks for creating test data.
- When possible, set a subject with a variable name to reduce repetition in
  expect statements.
- Align the left brace of multiple, contiguous (no blank line between) let
  and let! statements.
- Separate a multiline let or let! statement with a blank line.

## Recent Activity

<!-- claude-mem-context - auto-generated section, do not edit manually -->

### Jan 26, 2026

| ID    | Time    | T  | Title                                   | Read |
|-------|---------|----|-----------------------------------------|------|
| #2550 | 4:30 PM | ✅ | st-settings.json file read for sorting  | ~330 |
| #2549 | "       | ✅ | Alphabetical key sorting for settings   | ~293 |

<!-- end claude-mem-context -->
