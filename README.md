# TodoX (WORK IN PROGRESS)

## About

This is a terminal todo list tracker written in C.

## Usage
```bash
./build/todox [command] [task]?
```

### \[command\]:

1. **list**: list pending tasks
2. **list-all**: list pending and completed tasks
3. **list-completed**: list completed tasks
4. **purge**: remove all tasks
5. **add** [task]: add pending task
6. **complete** [task]: mark [task] as completed

### \[task\]

String of 999 characters maximum.

## Dependencies
- A C compiler
- [make](https://www.gnu.org/software/make/)
- [cmake](https://cmake.org/)

## Setup
Create the build directory. From the root of the project, run:

```bash
mkdir build
cmake -S . -B build
mv ./build/compile_commands.json ./compile_commands.json
```

This might be necessary to get code completion/snippets.

## Features

### Done

The following features are done:

1. Add new tasks
2. Persist tasks in the system
3. List all tasks
4. List completed tasks
5. List pending tasks
6. Mark tasks as completed
7. Purge all tasks
8. Remove specific tasks

## Compiling

From the project's root directory, run:

```bash
cmake -S . -B build
mv ./build/compile_commands.json ./compile_commands.json
make -C build
```
