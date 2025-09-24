# Exam 2

> Weight: 10%\
> Due: October 27

![mockup](mockup.excalidraw.svg)

Your task for this exam is to implement a `PinPad` component that allows
users to enter a 4-digit PIN (personal identification number). Here are
the requirements:

- Users can enter up to 4 digits.
- As they enter their PIN, only the last digit remains visible; previous
  digits are replaced by asterisks.
- Users can click the "clear" button to reset the PIN.
- The component accepts an optional `pin` prop as the default value.
- It also calls the `onChange` prop with the updated `pin` argument
  whenever the PIN changes.

## Starter files and submission

To access the starter files, first [accept the assignment][Classroom].
Then, clone your repository using `git clone <url>`, where `<url>` is
the link provided to you after accepting the asignment.

To submit your assignment, push your changes to the `main` branch on the
`origin` remote. Code pushed on other branches will not be assessed.

[Classroom]: https://classroom.github.com/a/l5jaOYpw

## Assessment criteria

- Program design [5]
  - requirements are met
  - program flow is decomposed into manageable, logical pieces
  - data structures are appropriate
  - common code is unified, not duplicated
  - appropriate algorithms are used, and coded cleanly
  - interfaces are used correctly
  - markup is semantic
  - return statements focus on markup with minimal logic

- Readability [5]
  - constants are used instead of hard-coded values
  - complex or meaningful expressions are named
  - naming is consistent and descriptive
  - inline comments are used only to explain reasoning
  - type annotations are correct (see `bun typecheck`)
  - code is well formatted (see `bun fmt`)
