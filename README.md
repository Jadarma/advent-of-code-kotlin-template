# Advent of Code Kotlin - Project Template

This is a self-contained starter project template for solving [Advent of Code](https://adventofcode.com/) puzzles in 
Kotlin!
It uses [AocKt](https://github.com/Jadarma/advent-of-code-kotlin) and [Kotest](https://kotest.io) to minimize boilerplate and provide
a smooth development experience.

## 🏗️ Use This Template

1. Make sure you're logged in to GitHub
2. Click the green ***Use this template*** button _(not fork!)_.
3. Select _Create a new repository_.
4. Choose yourself as the owner, a descriptive name, and a visibility(*).
5. Click _Create repository_.
6. Clone your repository, and open the project with IntelliJ IDEA.
7. Solve puzzles!

> [!CAUTION]
> ***(\*) DO NOT Commit Puzzle Inputs On Public Repos!***
>
> _It is against the rules to redistribute your puzzle inputs!_
>
> Inputs are intentionally git-ignored by default.
> This means that you would have to re-download your inputs and solutions every time you clone from a different machine.
> To avoid that, use something like [`git-crypt`](https://github.com/AGWA/git-crypt) to ensure inputs can only be read
> by you if you plan on sharing your repository publicly.

## 📝 Workflow Example

A step-by-step tutorial workflow is [documented here](https://jadarma.github.io/advent-of-code-kotlin/workflow.html).

It covers:
- The project file structure;
- How to add inputs and solutions;
- How to write tests and interpret their output;
- How to use the DSL to solve puzzles.

## ▶️ Running your Code

### From IntelliJ (Recommended)

If you have the [Kotest Plugin](https://plugins.jetbrains.com/plugin/14080-kotest) installed, the IDE will show a 
'Run' gutter icon near any `AdventSpec` in your code.
After that, you can re-run the same test using `Ctrl+F5`, or pressing the _Rerun_ button in the test tool window.
This provides the most comfortable feedback loop when solving new problems.
You may also run tests in bulk by right clicking on a test package.

### From Gradle / CLI

You can also run your tests from Gradle.

To run a specific test, pass it via its FQN:

```shell
./gradlew test --tests 'aockt.y9999.Y9999D01Test'
```

You may also filter and run tests in bulk.
For example, running all tests within the same year package:

```shell
./gradlew test --tests 'aockt.y9999.*'
```

If for whatever reason you want to run tests in bulk but skip the parts that have been marked as expensive, you can 
filter them out as well:

```shell
./gradlew test -Dkotest.tags='!Expensive'
```
