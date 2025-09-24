# Exam 1

> Weight: 10%\
> Due: September 29

Your task for this exam is to implement two components for a cooking
recipes website.

The first component, `Recipe`, receives an array of ingredients and
renders them as an unordered list. Ingredients are represented as
objects with the following properties:

```ts
type Ingredient = {
    id: number;
    name: string;
    bought: boolean;
};
```

By default, all ingredients are shown, but if the `showBought` prop is
set to false, only unbought ingredients are rendered.

The second component, `Ingredient`, is used to render each ingredient
with a checkbox input. If the ingredient has already been bought, the
checkbox is checked and the name of the ingredient is struck through.

The interfaces for both components's props are already defined in
"Recipe.tsx". Make sure to follow them.

Finally, in addition to the components, you must submit a 5 to 10
minutes video recording in which you explain how the evaluation of the
expression below unfolds according to the substitution model covered in
class.

```tsx
<Ingredient name={"tomato"} bought={true} />;
```

Your explanation should walk through the process step by step. Make sure
both your code and your face remain visible for the entire video.

## Starter files and submission

To access the starter files, first [accept the assignment][Classroom].
Then, clone your repository using `git clone <url>`, where `<url>` is
the link provided to you after accepting the asignment.

To submit your assignment, push your changes to the `main` branch on the
`origin` remote. Code pushed on other branches will not be assessed.

To record the video, use Teams’ built‑in recording feature. You can do
so by starting a meeting by yourself (Calendar → Meet now → More →
Record and transcribe). When you finish, the video will be automatically
saved to your OneDrive. Be sure to include the OneDrive link in the
message of your final commit. Don't upload your video on GitHub.

[Classroom]: https://classroom.github.com/a/pGrvmSzK

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
