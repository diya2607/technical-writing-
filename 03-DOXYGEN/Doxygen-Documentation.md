
# 📚 DOXYGEN — AUTOMATED CODE DOCUMENTATION

<p align="center">
  <b>TECHNICAL WRITING | MODULE 03</b>
</p>

> Doxygen is a documentation generator that creates structured documentation from specially formatted comments in source code.

---

## 📑 TABLE OF CONTENTS

1. Introduction to Doxygen
2. Features
3. Installation
4. Basic Workflow
5. Documentation Comments
6. Special Commands
7. Documenting Functions
8. Documenting Classes
9. Documenting Variables
10. Documenting Files
11. Main Page Documentation
12. Configuration File
13. Generating HTML Documentation
14. Generating PDF Documentation
15. Graphs and Diagrams
16. Advantages and Applications

## 01. INTRODUCTION

Doxygen is an open-source documentation tool.

It supports languages such as:
- C
- C++
- Java
- Python
- C#
- PHP

It reads source code and specially formatted comments to generate documentation.

## 02. FEATURES

- Automatic documentation generation.
- HTML and LaTeX output.
- Function and class documentation.
- Cross-references.
- Class diagrams.
- Inheritance diagrams.
- Search functionality.
- Configurable output.

## 03. INSTALLATION

Official website:

https://www.doxygen.nl/

On macOS, using Homebrew:

```bash
brew install doxygen
```

Check installation:

```bash
doxygen --version
```

Graph visualisation can also use Graphviz:

```bash
brew install graphviz
```

## 04. BASIC WORKFLOW

1. Write source code.
2. Add documentation comments.
3. Create a Doxygen configuration file.
4. Configure input and output settings.
5. Run Doxygen.
6. Open the generated documentation.

## 05. DOCUMENTATION COMMENTS

Doxygen recognises specially formatted comments.

**Style 1:**

```cpp
/**
 * This function adds two numbers.
 */
```

**Style 2:**

```cpp
///
/// This function adds two numbers.
///
```

**Style 3:**

```cpp
//! This function adds two numbers.
```

These comments are used to generate documentation.

## 06. SPECIAL COMMANDS

| Command | Purpose |
|---|---|
| `@brief` | Short description |
| `@details` | Detailed explanation |
| `@param` | Describes parameter |
| `@return` | Describes return value |
| `@author` | Author information |
| `@date` | Date information |
| `@file` | File description |
| `@class` | Class documentation |
| `@see` | Related reference |
| `@note` | Additional note |
| `@warning` | Important warning |
| `@example` | Example reference |
| `@todo` | Future task |

The `@` and backslash command forms are generally interchangeable.

## 07. DOCUMENTING FUNCTIONS

Example:

```cpp
/**
 * @brief Adds two integers.
 *
 * This function calculates the sum
 * of two given integer values.
 *
 * @param a First number.
 * @param b Second number.
 * @return Sum of the two numbers.
 */
int add(int a, int b) {
    return a + b;
}
```

## 08. DOCUMENTING CLASSES

```cpp
/**
 * @class Student
 * @brief Represents a student.
 *
 * Stores student information.
 */
class Student {
public:

    /// Student name
    string name;

    /**
     * @brief Displays student details.
     */
    void display();
};
```

## 09. DOCUMENTING VARIABLES

```cpp
/// Stores the student age.
int age;
```

Or:

```cpp
int age; ///< Stores the student age.
```

## 10. DOCUMENTING FILES

At the beginning of a source file:

```cpp
/**
 * @file main.cpp
 * @brief Main program file.
 * @author Your Name
 * @date 2026
 */
```

## 11. MAIN PAGE DOCUMENTATION

A special main page can be created using:

```cpp
/**
 * @mainpage Project Documentation
 *
 * @section intro Introduction
 * Welcome to the project.
 *
 * @section features Features
 * - Easy to use
 * - Well documented
 */
```

This provides an introductory page for generated documentation.

## 12. CONFIGURATION FILE

Doxygen uses a configuration file named `Doxyfile`.

Generate it using:

```bash
doxygen -g
```

Important settings:

| Setting | Purpose |
|---|---|
| `PROJECT_NAME` | Project name |
| `PROJECT_NUMBER` | Version number |
| `INPUT` | Source input |
| `FILE_PATTERNS` | File types |
| `RECURSIVE` | Search subfolders |
| `OUTPUT_DIRECTORY` | Output location |
| `GENERATE_HTML` | HTML generation |
| `GENERATE_LATEX` | LaTeX generation |
| `EXTRACT_ALL` | Include undocumented entities |
| `HAVE_DOT` | Graphviz support |

## 13. GENERATING HTML DOCUMENTATION

First create a Doxyfile.

Configure the project settings.

Then execute:

```bash
doxygen Doxyfile
```

The generated HTML documentation is usually placed inside:

```text
html/
```

Open:

```text
html/index.html
```

This displays the documentation in a web browser.

## 14. GENERATING PDF DOCUMENTATION

Enable LaTeX output in the Doxyfile:

```text
GENERATE_LATEX = YES
```

Then run:

```bash
doxygen Doxyfile
```

Doxygen generates LaTeX files inside the `latex/` output directory.

Compile the generated LaTeX project using an appropriate LaTeX compiler to produce a PDF.

## 15. GRAPHS AND DIAGRAMS

Doxygen can generate diagrams when Graphviz is configured.

Useful settings:

```text
HAVE_DOT = YES
CLASS_DIAGRAMS = YES
CALL_GRAPH = YES
CALLER_GRAPH = YES
```

These help visualise relationships between classes and functions.

## 16. ADVANTAGES

- Saves documentation time.
- Makes source code easier to understand.
- Improves project maintenance.
- Creates navigable documentation.
- Helps developers understand large projects.
- Supports multiple programming languages.

## 🎯 LEARNING OUTCOME

Through Doxygen, I learned how to write structured documentation comments, document functions and classes, configure a project using Doxyfile and generate professional HTML and LaTeX documentation from source code.

---

**END OF MODULE 03 | DOXYGEN**
