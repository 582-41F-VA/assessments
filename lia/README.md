# LIA

> Weight: 30%\
> Due: March 10\
> Modality: in teams of 3

For this LIA, your task is to implement the React front-end for an issue
tracker, similar to GitHub Issues or Jira. Here are the required
features:

- Users can create projects from the homepage. Each project has a name.
- Users can edit the name of a project.
- Users can delete projects.
- Users can create members in a project. Each member has a name.
- Users can edit the name of a member.
- Users can delete a member from a project.
- Users can create labels in a project. Each label has a name.
- Users can edit the name of a label.
- Users can delete a label from a project.
- Users can create issues in a project. Each issue has a title and a
  description.
- Users can see the list of issues in a project.
- Users can delete issues.
- Users can assign and unassign members to an issue.
- Users can assign and unsassign labels to an issue.
- Issues can be filtered by labels and assignees.
- Issues can be searched by title. Search results can be filtered as
  above.

Your single-page application must use the router implemented in class,
and connect to the Django back-end provided in your repository.

To avoid hardcoding the server's development hostname when using
`fetch`, create a ".env" file in the "web" directory, and set an
environment variable like so:

```env
API_BASE_URL="http://localhost:8000"
```

You can then access it in your code with via `process.env.API_BASE_URL`.

## Setup

1. Team up with two other students.
2. Choose who will be responsible for creating the repository. That
   student must click [here][Classroom] and follow the instructions.
3. Change the name of the repository to include both of your names.
   (Settings → General → Repository name)
4. Give your teammate access to the repository. (Settings →
   Collaborators and teams → Manage access)

[Classroom]: https://classroom.github.com/a/IEd2D1eZ

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
