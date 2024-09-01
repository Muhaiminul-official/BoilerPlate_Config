
---

# Boilerplate Configurations for VS Code

This repository contains boilerplate configurations for various programming languages to help you quickly set up new projects.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Configurations](#configurations)
  - [C Boilerplate](#c-boilerplate)
  - [C++ Boilerplate](#cpp-boilerplate)
  - [Java Boilerplate](#java-boilerplate)
- [VS Code Extensions](#vs-code-extensions)

## Introduction

This repository provides snippets for creating boilerplate code in C, C++, and Java. These snippets are designed to streamline the process of starting new projects by automatically generating basic code structures.

## Installation

To use these snippets, you'll need to add them to your Visual Studio Code snippets configuration. Follow these steps:

1. Open Visual Studio Code.
2. Go to `File` > `Preferences` > `User Snippets`.
3. Select the language for which you want to add the snippet (e.g., `c.json`, `cpp.json`, `java.json`).
4. Copy and paste the relevant snippet configuration from this repository into the appropriate file.

## Usage

Once the snippets are added, you can trigger them by typing the prefix (e.g., `@`) in a file of the corresponding language. This will automatically insert the boilerplate code into your file.

## Configurations

###  C Boilerplate 

**File**: `c.json`

```json
{
	"boilerplate": {
		"prefix": "@",
		"body": [
			"#include <stdio.h>",
			"",
			"int main()",
			"{",
			"    $1",
			"    return 0;",
			"}"
		],
		"description": "Basic C program boilerplate"
	}
}
```

###  C++ Boilerplate 

**File**: `cpp.json`

```json
{
	"boilerplate": {
		"prefix": "@",
		"body": [
			"#include <iostream>",
			"using namespace std;",
			"",
			"int main()",
			"{",
			"    $1",
			"    return 0;",
			"}"
		],
		"description": "Basic C++ program boilerplate"
	}
}
```

###  Java Boilerplate 

**File**: `java.json`

```json
	{
	"boilerplate": {
		"prefix": "@",
		"body": [
			"import java.util.*;",
			"import static java.lang.Math.*;",
			"",
			"public class ${1:Main} {",
			"    public static void main(String[] args) {",
			"        $2",
			"    }",
			"}"
		],
		"description": "Basic Java Main class boilerplate with imports"
	  }
      }

```

##  VS Code Extensions

To enhance your development experience, consider installing the following Visual Studio Code extensions:

- **C/C++ Extension Pack**: Provides IntelliSense, debugging, and code browsing for C and C++.
- **Code Runner**: Runs code snippets in the terminal.
- **Java Extension Pack**: Includes essential Java extensions such as Language Support for Java, Debugger for Java, and Maven for Java.

These extensions can improve productivity by offering features like code suggestions, debugging support, and more.

---

