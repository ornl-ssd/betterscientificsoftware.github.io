# Integrated Development Environments (IDEs) for Scientific Sofware Development

IDEs have been used extensively for software development for many years, and in most software engineering domains, 
are considered best practice. However, their uptake for scientific software development, and in particular, high
performance computing (HPC), has been much slower. Nevertheless, IDEs are quite widely used, particularly where software
engineering professionals are actively involved in the development of scientific software.

When choosing an IDE for scientific software development, some important considerations include:

- Provides support for multiple languages, in particular, C/C++, Fortran, and Python.
- Does not interfere with existing build practices and toolchains.
- Integrates simply and smoothly with existing tools and systems.
- Is easily customizable to suit individual or team requirements.
- Works on a variety of platforms (Windows, Mac, Linux).
- Allows remote development.

The following sections describe IDEs that meet one or more of the requirements for scientific code development. 

## Free IDEs

### [Eclipse CDT](https://eclipse.org/cdt/)

Eclipse is a professional quality integrated development environment and tool integration platform. It is built on the OSGI framework, which allows functionality to be added via plugin components. Eclipse was traditionally used for Java development, but C and C++ support has been available for many years. The [C/C++ Development Tools (CDT)](https://eclipse.org/cdt/) project adds support for developing and building C and C++ applications. Features include:

* Project and build support
* Full featured editor
* Source code navigation
* Refactoring
* Static code analysis
* Debugging
* Unit testing
* Autotools
* VCS integration

CDT can also be combined with the [LinuxTools project](https://eclipse.org/linuxtools/) to provide integration with a variety of Linux based tools, including:

* Callgraph
* Changelog
* Docker
* GProf
* Gcov
* Libhover
* Man page
* OProfile
* Perf
* Systemtap
* Valgrind
* RPM

The latest version of Eclipse CDT Neon.3 can be downloaded from [here](https://www.eclipse.org/downloads/packages/eclipse-ide-cc-developers/neon3).

### [Eclipse PTP](https://eclipse.org/ptp/)

The [Parallel Tools Platform (PTP)](https://eclipse.org/ptp/) project is an extension of Eclipse CDT that adds support for developing parallel and scientific programs. It includes most of the features found in Eclipse CDT, plus:

* Support for Fortran
* MPI/OpenMP/OpenACC/OpenSHMEM bindings
* Parallel debugging
* Synchronized projects
* Job scheduler integration

The latest version of Eclipse PTP Neon.3 can be downloaded from [here](https://www.eclipse.org/downloads/packages/eclipse-parallel-application-developers/neon3).

### [Netbeans IDE](https://netbeans.org)

Netbeans IDE is the offcial IDE for Java 8, and like Eclipse, is extensible via a plugin mechansim. Plugins are available to support for C, C++ and Fortran development. Features include:

* C and C++ projects
* C and C++ editor
* GNU gdb integration
* Code assistance
* Unit testing
* Source inspection
* Packaging

The latest version of Netbeans IDE 8.2 is available from [here](https://netbeans.org/downloads/)

### [Code::Blocks](http://www.codeblocks.org)

Unlike Eclipse and Netbeans, which started as Java IDEs and have C/C++/Fortran support added via plugins, Code::Blocks is designed primarily as a C, C++ and Fortran IDE. However, it is also extensible via plugins, and so new functionality can be added if required. Features include:

* Multi-target projects
* Parallel builds
* Imports MSVC and Dev-C++ projects
* Debugging using GNU GDB and MS CDB
* Syntax highlighting
* Code folding
* Code completion
* Class browser
* Smart indent
* VCS integration

The latest version of Code::Blocks can be downloaded from [here](http://www.codeblocks.org/downloads/26). Although cross-platform, support for Mac OS X is not as advanced as other platforms.

## Commercial/Proprietary IDEs

### [JetBrains CLion](https://www.jetbrains.com/clion/)

CLion is a commercial cross-platform IDE for C and C++ development. Features include:

* Smart customizable editor
* Navigation and search
* Code generation and refactorings
* On-the-fly code analysis
* Run and debug
* CMake support
* Unit testing
* VIM mode
* Python support

An evaluation version of CLion 2017.1.3 is available [here](https://www.jetbrains.com/clion/download/). Cost is $89 for an individual license for the first year, with discounts for future years.

### [XCode IDE](https://developer.apple.com/xcode/ide/)

The XCode IDE is primarily aimed at developing applications for Apple platoforms. It comes as part of Apple's proprietary XCode developer toolset. In addition to Apple's Objective-C and Swift languages, the XCode IDE provides support for C, C++, and Python, so is well suited for developing scientific applications. Features include:

* Fast structure-based editor
* Refactoroing
* Search
* Debugging
* Source control (navigation and inspection)
* Build system
* Documentation
* Testing

The latest version of XCode 9 is available from [here](https://developer.apple.com/download/) (requires login).

### [Visual Studio IDE](https://www.visualstudio.com/vs/)

Visual Studio IDE is Microsoft's proprietary integrated development environment, and the primary environment for developing Windows applications. It provides builtin support for C and C++, so is suited for scientific application development, although applications will only run on Windows without some additional work. It can be extended via plugins, and support for Fortran and Python are available this way. Features include:

* Application projects
* Syntax highlighting
* Code completion
* Code folding
* Incremental search
* Debugging (Visual Studio debugger only)
* VCS integration
* Database integration

The latest version of Visual Studio IDE is available from [here](https://www.visualstudio.com/downloads/).

## Supported Features

The following tables show which IDEs support important features for scientific code development.

### Language Support

| IDE               | C/C++ | Fortran | Python             |
|-------------------|:-----:|:-------:|:------------------:|
| Eclipse CDT       |   Y   |    N    |   Y<sup>1</sup>    |
| Eclipse PTP       |   Y   |    Y    |   Y<sup>1</sup>    |
| Visual Studio.NET |   Y   |    Y<sup>1</sup>    |   Y<sup>1</sup> |
| Netbeans          |   Y   |    N    |   Y (since 8.1)    |
| CLion             |   Y   |    N    |   Y                |
| XCode             |   Y   |    N    |   Y<sup>2</sup>    |
| Code::Blocks      |   Y   |    N    |   Y<sup>1</sup>    |

1. Requires 3rd party plugin
2. Requires manual configuration

### Build Systems

| IDE               | Makefile | CMake              | autotools          |
|-------------------|:--------:|:------------------:|:------------------:|
| Eclipse CDT       |   Y      |    Y               |   Y                |
| Eclipse PTP       |   Y      |    Y               |   Y                |
| Visual Studio.NET |   Y      |    Y (since 2017)  |   N                |
| Netbeans          |   Y      |    Y<sup>1</sup> (since 8.2)   |   Y<sup>2</sup>  |
| CLion             |   Y      |    N               |   Y<sup>1</sup>    |
| XCode             |   Y      |    N               |   Y<sup>2</sup>    |
| Code::Blocks      |   N      |    N<sup>3</sup>   |   N    |

1. [Requires manual configuration](http://www.frankliuao.com/blogs/how-to-work-with-cmake-and-netbeans-8-2-or-newer-on-os-x/)
2. Requires 3rd party plugin
3. CMake can be used to generate Code::Blocks project files

### Platforms

| IDE               | Windows | Linux | Mac OS X |
|-------------------|:-----:|:-------:|:--------:|
| Eclipse CDT       |   Y   |    Y    |   Y      |
| Eclipse PTP       |   Y   |    Y    |   Y      |
| Visual Studio.NET |   Y   |    N    |   Y      |
| Netbeans          |   Y   |    Y    |   Y      |
| CLion             |   Y   |    Y    |   Y      |
| XCode             |   N   |    N    |   Y      |
| Code::Blocks      |   Y   |    Y    |   Y<sup>1</sup> |

1. Current version not supported

