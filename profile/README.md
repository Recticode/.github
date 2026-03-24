# Recticode

Practice real-world coding by fixing bugs in actual codebases, not solving toy problems.

## What is this?

Recticode is a cli-based platform where you:
- pull a coding challenge (a real mini codebase)
- identify and fix a bug or implement a feature
- run tests to verify your solution
- submit your fix

Instead of writing isolated functions, you work with realistic systems.

## Why?

Most platforms train you to:
- solve algorithm problems from scratch

But real dev work is more like:
- reading existing code
- debugging issues
- making safe changes without breaking things

Recticode is built to train **that skill**.

## How it works
1. install the cli
2. fetch a challenge
3. work locally in your editor
4. run tests
5. submit your solution

## Install
```
pip install recticode
```

Check it works:
```
recticode --help
```

## Example Flow
```
# login
recticode login

# get a challenge
recticode start <challenge-name>

# work on the code locally...

# run tests
recticode check

# submit your fix
recticode submit
```

## Challenge Format

Each challenge includes:
- a small codebase (multiple files)
- a realistic bug or task
- test cases to validate behaviour

Examples:
- duplicate payments being triggered
- broken authentication logic
- slow api endpoint
- incorrect database updates

## Open Source

Recticode is fully open source.

You can:
- create your own challenges
- share them with others
- improve the platform

## Creating your own challenges

- define a codebase
- introduce a bug or requirement
- write test cases that validate correct behaviour

Goal:
> Make it feel like real dev work, not puzzles.

## Vision

Recticode aims to become:
- a better way to practise real-world development
- a community-driven library of system challenges
- a bridge between learning and actual job skills

## Feedback

This project is experimental

If you try it or have thoughts:
- open an issue
- start a discussion
- reach out
