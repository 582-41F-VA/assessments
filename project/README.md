# Project: Spelling Bee

> Weight: 20%\
> Due: November 10\
> Modality: in teams of 2

[Spelling Bee] is a word game created by Frank Longo in which players
use letters from an hexagonal honeycomb structure to form as many words
as possible. Here are the rules:

- Words must contain at least 4 letters.
- Words must include the center letter.
- Letters can be used more than once.

Players score points based on the words they submit.

- 4-letter words are worth 1 point.
- Longer words earn 1 point per letter.
- Each puzzle includes at least one "pangram" which uses every letter.
  These are worth 7 extra points.

The more points a player scores, the higher their rank. Ranks are based
on a percentage of maximum points in a puzzle.

| Rank       | Percentage |
| ---------- | ---------- |
| Beginner   | 0%         |
| Good Start | 2%         |
| Moving Up  | 5%         |
| Good       | 8%         |
| Solid      | 15%        |
| Nice       | 25%        |
| Great      | 40%        |
| Amazing    | 50%        |
| Genius     | 70%        |
| Queen Bee  | 100%       |

## Instructions

Your task for this project is to implement your own version of Spelling
Bee using React. Here are the requirements:

- The page has two sections: controls on the left and scoreboard on the
  right.
- The controls section has an input for players to enter words, either
  by typing on their keyboard when the input is focused, or clicking on
  the letters in the honeycomb.
- To submit a word, players can either click on a "Submit" button or
  press on the "Return" key. If the word is too short or not in the
  words list, an error is shown.
- Players can click on a "Reset" button to reset the input's value.
- Players can click on a "Shuffle" button to shuffle the order of the
  letters in the honeycomb (except for the center letter).
- The scoreboard section has two tabs. The score tab shows the list of
  words found and the points each is worth. The rank tab shows the list
  of ranks and the minimum score required for each. Refer to the
  included mockup for details.

Your repository includes a "puzzle.ts" file with data you should use for
testing. Values such as the minimum score for each rank must be computed
dynamically. For rendering the honeycomb, we suggest using a 3 × 5 grid
of buttons. The `clip-path` CSS property and the `polygon` CSS function
can be used to render buttons as hexagons.

[Spelling Bee]: https://www.nytimes.com/puzzles/spelling-bee

## Setup

1. Pair up with another student.
2. Choose who will be responsible for creating the repository. That
   student must click [here][Classroom] and follow the instructions.
3. Change the name of the repository to include both of your names.
   (Settings → General → Repository name)
4. Give your teammate access to the repository. (Settings →
   Collaborators and teams → Manage access)

[Classroom]: https://classroom.github.com/a/DuYe-b_B

## Pull request workflow

To make collaboration smoother and encourage code review, you will share
your code with your teammate using GitHub's pull request workflow. Here
are the steps to follow once you have cloned the repository:

1. Make sure your local main branch is up to date with the remote main
   branch by running `git pull`.

2. From your local main branch, create a local feature branch with
   `git checkout -b <branch-name>`, where `<branch-name>` corresponds to
   the name of the feature you will implement.

3. Commit your changes with `git add <path>` and `git commit` (many
   times if necessary).

4. Once your code is ready, push your commits to GitHub with
   `git push -u origin <branch-name>`.

5. Using GitHub's web interface, create a pull request (Pull requests →
   New pull request → feature branch's name → Create pull request).

6. Let your teammate review your pull request. If necessary, make
   changes to your pull request by pushing new commits (repeat step #2
   and #3).

7. Let your teammate rebase and merge your pull request (Pull requests →
   pull request's name → Rebase and merge). If your pull request is
   out-of-date with main, GitHub will not let you merge it. In that
   case:

   1. Back in your terminal, switch to your local main branch with
      `git checkout main`.

   2. Sync your local main branch with the remote main branch using
      `git pull`.

   3. Switch back to your local feature branch with
      `git checkout <branch-name>`.

   4. Incorporate the latest changes from the main branch into your
      local feature branch with `git rebase main`.

   5. Fix merge conflicts, if any.

   6. Update your remote feature branch with `git push --force`.

8. Delete the remote feature branch (Code → main → view all branches →
   trash icon).

9. Back in your terminal, switch to your local main branch with
   `git checkout main`.

10. Sync your local main branch with the remote main branch using
    `git pull`.

11. Delete your local feature branch with `git branch -D <branch-name>`.

12. Repeat for every feature.

## Assessment criteria

- Program design
  - requirements are met
  - program flow is decomposed into manageable, logical pieces
  - data structures are appropriate
  - common code is unified, not duplicated
  - appropriate algorithms are used, and coded cleanly
  - interfaces are used correctly
  - markup is semantic
  - return statements focus on markup with minimal logic

- Readability
  - constants are used instead of hard-coded values
  - complex or meaningful expressions are named
  - naming is consistent and descriptive
  - inline comments are used only to explain reasoning
  - type annotations are correct (see `bun typecheck`)
  - code is well formatted (see `bun fmt`)

- Version control
  - commits contain related changes
  - messages are consistent and informative
  - changes are merged using pull requests

- Teamwork
  - workload is divided evenly (styling will not be assessed and
    therefore doesn't count toward your workload)
  - comments on pull requests are useful
  - peer assessment
