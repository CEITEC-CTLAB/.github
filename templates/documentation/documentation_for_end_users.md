<!--
This template is suitable for submitting code packages bundled with executables.
Its main focus is providing the reader with a guide on how to use the code and executables based on it.
-->

<!--
Recommended VS Code extensions for working with Markdown:
    Markdown All in One - some Markdown perks (table of contents, auto completions, HTML export, ...)
    Markdown Extended - support for extended markdown syntax
    Markdownlint - linting & style checking
    PlantUML - Support for WSD diagrams
    Markdown PlantUML Preview - Support for PlantUML inside Markdown
For more info on Markdown, go to https://www.markdownguide.org/
-->

# >Project Name<: Manual & Documentation

- [\>Project Name\<: Manual \& Documentation](#project-name-manual--documentation)
  - [Introduction](#introduction)
  - [Manual](#manual)
    - [Data Input and Output](#data-input-and-output)
      - [Input](#input)
      - [Output](#output)
    - [Settings](#settings)
      - [Setting 1](#setting-1)
      - [Setting 2](#setting-2)
    - [Graphical User Interface](#graphical-user-interface)
      - [GUI Components](#gui-components)
    - [Command Line Interface](#command-line-interface)
      - [Command Line Inputs](#command-line-inputs)
      - [Usage](#usage)
  - [Code Documentation](#code-documentation)
    - [Requirements \& Dependencies](#requirements--dependencies)
    - [Class Diagram](#class-diagram)
    - [Methodology Flowcharts](#methodology-flowcharts)
  - [Code Examples](#code-examples)
    - [Example of running the code/launching the GUI, etc.](#example-of-running-the-codelaunching-the-gui-etc)
  - [Code Reference](#code-reference)
  - [Notes](#notes)
    - [Note 1](#note-1)
    - [Note 2](#note-2)
  - [Contacts](#contacts)

## Introduction

Describe the background/motivation and purpose of >Project Name<, along with anything else the reader should know about >Project Name< as a whole. Be as concise as possible.

Tell the reader what they can expect in this text. A methodology? Code documentation? A manual?. Are there different types of interfaces accessible to the user (GUI/CLI/API/Scripting interface/...)?

## Manual

>Project Name< is packaged into an executable, which provides both a graphical and command-line interface. The basic usage of both is introduced below.

### Data Input and Output

#### Input

What input data is the >Project Name< package designed to process? What are the proper/valid data formats and other requirements?

#### Output

What can the user expect the >Project Name< package to produce as outputs? Will the package produce data on disk? In what format? Are there any secondary outputs like a log file? Is anything printed on the command line?

### Settings

What settings of the >Project Name< package are accessible to the user? What can the user influence about the processing?

#### Setting 1

- `value 1`: describe what the setting does.
- `value 2`: describe what the setting does. Provide any additional info/[links](https://www.wikipedia.org/) you deem necessary.

#### Setting 2

- `value 3`: describe what the setting does.
- `value 4`: describe what the setting does.

### Graphical User Interface

Introduce the GUI and what the user can expect from it. Include graphics:

![placeholder image](graphics/placeholder.svg)
<!-- ![placeholder image](graphics/placeholder.png) -->

#### GUI Components

1. **GUI component 1**:
   - What does the component do?
   - How can it be used?
   - What options does it offer to the user?

2. **GUI component 2**:
   - What does the component do?
   - How can it be used?
   - What options does it offer to the user?

### Command Line Interface

Introduce the CLI and what the user can expect from it. Add any notes you think might be important/useful for the user. Include clear instructions for how to provide inputs

#### Command Line Inputs

| Input | Options | Note |
| - | - | - |
| --input_path | Path to input file | Enclose in "quotes" if path contains spaces. |
| --output_path | Path to output file | Enclose in "quotes" if path contains spaces. Defaults to the same path and name as the input file. |
|--setting1 | `value1` (default), `value2` | Sets setting 1. |
|--setting2 | `value3` (default), `value4` | Sets setting 2. |

#### Usage

```shell
>provide a couple examples for using the CLI
```

## Code Documentation

### Requirements & Dependencies

>Project Name< is implemented in `Python 3.XX`, and uses the following third-party packages:

| Package  | License  | Note |
| - | - | - |
| [NumPy](https://numpy.org/) | [BSD-style license](https://github.com/numpy/numpy/blob/main/LICENSE.txt) | Used for image data handling and mathematical operations|
| [SciPy](https://scipy.org/) | [BSD 3-clause license](https://github.com/scipy/scipy/blob/main/LICENSE.txt) | Used for signal/image processing [Bundled software list](https://github.com/scipy/scipy/blob/main/LICENSES_bundled.txt) |

Additionally, the following auxiliary packages were used:

| Package | License | Note |
| - | - | - |
| [PyInstaller](https://pyinstaller.org/en/stable/#) | [GNU-GPL license](https://github.com/pyinstaller/pyinstaller?tab=License-1-ov-file#readme) with an Bootloader Exception, which provides unlimited permission for the use of the packaged executable | Used to package code into an executable |
| [markdown-pdf](https://github.com/vb64/markdown-pdf) | [MIT license](https://github.com/vb64/markdown-pdf/blob/main/LICENSE) | Used for creating documentation |
| [doxygen](https://doxygen.nl/index.html) | [GPL-2.0 license](https://github.com/doxygen/doxygen/blob/master/LICENSE) | Used for generating code documentation |

The complete list of requirements including secondary dependencies is as follows:
<!-- include the packages you used and their versions. you can use the outputs of `pip freeze` -->

```cmd
package1==0.1.0
package2==0.2.1
```

### Class Diagram

The following figure provides an overview of classes used in >Project Name<

### Methodology Flowcharts

The >Project Name< workflow is split into the following subprocesses:

- Subprocess 1
- Subprocess 2
  - Subsubprocess a
  - Subsubprocess b

The overall workflow and the interaction of its subprocesses is illustrated in the flowchart/s below.

![placeholder image](graphics\placeholder_chart.svg)

## Code Examples

The following snippets show basic usage of the >Project Name< package.
For more information on the contents of the codebase, see the [reference below](#code-reference).

### Example of running the code/launching the GUI, etc.

```python
import sys

print('This is an example code block.')

# Show the reader how to get started with using the code

sys.exit('See ya!')

```

## Code Reference

[View Documentation](html/index.html) (If the link is not working, access the documentation by going to the *html* subfolder and opening `index.html`)

## Notes

### Note 1

Describe something that you feel should be mentioned in this text, but does not fit into the main body. Notes on external packages used in the code, example data, or suggestions for future development can all go in this section.

### Note 2

Add something else you would like to mention

## Contacts

Software created in the [CT Lab](https://ctlab.ceitec.cz/), Central European Institute of Technology, Brno University of Technology.

For questions, suggestions, etc., contact:

- Contributor 1: [name1.surname1@email.cz](name1.surname1@email.cz)
- Contributor 2: [name2.surname2@email.cz](name2.surname2@email.cz)
