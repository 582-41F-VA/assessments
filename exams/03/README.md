# Exam 3

> Weight: 10%\
> Due: November 17

The "App.tsx" file included in your repository implements a
`<LangSelect>` component that allows users to choose their desired
display language. To render messages in the chosen language, a `<T>`
component is used. Currently, a `lang` prop is used to pass the chosen
language from `<App>` down to `<T>`. Your task for this assignment is to
refactor the code so that the chosen language is stored in context
instead.

## Starter files and submission

To access the starter files, first [accept the assignment][Classroom].
Then, clone your repository using `git clone <url>`, where `<url>` is
the link provided to you after accepting the assignment.

To submit your assignment, push your changes to the `main` branch on the
`origin` remote. Code pushed on other branches will not be assessed.

[Classroom]: https://classroom.github.com/a/HqxT0sLt

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
