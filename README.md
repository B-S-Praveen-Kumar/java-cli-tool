# Java CLI Tool

A lightweight command-line tool that helps developers quickly generate Java project structures and common source files directly from the terminal.

Instead of manually creating folders and boilerplate files, this CLI automates the process while enforcing Java naming conventions and preventing common mistakes like duplicate packages.

---

## Why This Tool Exists

Setting up a Java project often involves repetitive steps:

- Creating project folders
- Building package directory structures
- Writing boilerplate classes and interfaces
- Ensuring naming conventions are followed

This CLI simplifies those tasks so you can focus on writing actual code.

---

## Features

- Create Java project structures instantly
- Generate packages using standard Java naming conventions
- Create classes, interfaces, enums, and main classes
- Prevent duplicate packages and classes
- Reject Java reserved keywords in package names
- Works directly from the terminal

---

## Installation

Clone the repository:

```bash
$git clone https://github.com/B-S-Praveen-Kumar/java-cli-tool.git
cd java-cli-tool
```

Make the CLI executable:

```bash
$chmod +x javacli
```

(Optional) Install globally so it can be used from anywhere:

```bash
$sudo mv javacli /usr/local/bin/
```

Now the command javacli will be available system-wide.

## Usage

Create a New Java Project

```bash
$javacli new MyProject
```

Project structure created:

```text
MyProject
└── src
```

Create a Package

```bash
$javacli pkg MyProject com.example.service
```

Structure created:

```text
MyProject
└── src
    └── com
        └── example
            └── service
```

Create a Class

```zsh
$javacli class MyProject com.example.service ExampleService
```

Generated file:

```text
MyProject/src/com/example/service/ExampleService.java
```

Example generated code:

```java
package com.example.service;

public class ExampleService {

}
```