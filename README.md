# Github tag stars

## Introduction

This is our programming exercise. Our goal is to evaluate your programming skills, the ability to make technical decisions and to document the work done.

## What we will evaluate

1. README.md is well written, with the instructions needed to run the application, etc;
2. The code is well written, clean and cohesive;
3. Implementation of the solution is working as expected;
4. There are well written automated tests (i.e., the unit and integration tests cover the expected behavior);
5. There is linter/static code analysis;
6. RESTful API design needs to be implemented correctly using the HTTP verbs and the proper Status Code;
7. An API documentation has to be delivered with comprehensible and maintainable format;

We want to evaluate your ability to deliver code with the best programming practices, with sufficient documentation for other developers to understand what you did and actively contribute to the project.


## How to share your code with us

We want you to experience how we work on a daily basis. That's why we ask you to use the best standard gitflow practices and also the following instructions:

Create a README.md file describing how to configure your project, containing the commands that must be executed to run the software and the tests.
If you have made use of any Linter (esling, rubycop, creed, etc.), send the file together with the project.
Open a single pull request to the main branch of the private repository that we have invited you to contribute with all the code of the exercise.

# Exercise ✏️

GitHub is a social network of programmers that has an interesting functionality that allows you to ["star" other users repositories](https://docs.github.com/en/get-started/exploring-projects-on-github/saving-repositories-with-stars). The users activate that just by pressing a button. But it has some limitations when we consider GitHub heavy users.

You are an active GitHub user, who is always looking for new projects and enjoying those who are interesting. You would like to be able to add a label or tag to a repository so that it can be found later. For example, you've found a repository called `react` and you would like to add `javascript` and `frontend` tags to it. Because GitHub does not have this functionality, you want to build a simple system that can help with this task


## Use case

You are an active GitHub user, who is always looking for new and interesting projects. You want to add a label or tag to a repository so that it can be found later. For example: you've found a repository called react and you would like to add javascript and frontend tags to it. Because GitHub does not have this functionality, you want to build a simple system that can help you with this task.

## Requirements of the exercise


- [Required] Retrive starred repositories of a user's GitHub profile;
- [Required] Manage retrieved repositories tags (i.e., add, edit, delete);
- [Required] Filter repositories by tags;
- [Optional] Tags suggestions based on the overral use of the tag in other repositores;
- [Optional] A frontend graphical app to interact with the backend;

## User stories

### Story 1: Obtain starred repositories

```
As a GitHub user
I want to provide my username
So that I can see all repositories that I've starred
```

Requirements

- You should get starred repositories using the GitHub Public API.
- The information that must be retrieved is: repository ID, repository name, description, HTTP URL, and language.

### Story 2: Add tags to repositories

```
As a GitHub user
I want to be able to add tags to repositories that I've starred
So that I can easily find them later by tags
```

Requirements

- A repository cannot have duplicated tags.

### Story 3: Search repositories by tags

```
As a GitHub user
I want to be able to search by a specific tag
So that I can see my starred repositories that I've added this tag
```

Requirements

- The search field should work for queries with strings in half (e.g., by typing "doc", the "docker" and "ex_doc" repositories must be returned).

## Back-end instructions

- It is up to the candidate decide how to persist the data.
- Each action must have its specific route respecting the convention of http verb and status code.
- Repositories and their tags must persist at a database or file system.
