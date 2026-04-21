# nim2_ide

Notepad++ plug-in IDE for Nim v2 programming language

## Features

  * Multi-pass highlighting
  
    Syntax highlighting superimposed with compiler symbols.
  
  * Full syntax highlighting
  
    Highlight more Nim features than other lexers.
  
  * Unicode lexer
  
    Highlight Nim unicode operators.
  
  * Zero-config multi-thread backend
  
    No LSP bloat. Managed thread pool and _nimsuggest_ processes.
  
  * One nimsuggest per project
  
    Efficiently share _nimsuggest_ in a project and its directory tree.
  
  * Advanced features - using **nimsuggest**
    - Project aware
    - Context aware, intelligent code completion
    - Call tips
    - Real-time code analysis / linting
    - Detailed code analysis (on file save)
    - Highlight symbols (on scroll)
    - Hover (with mouse) for definition
    - Go to definition (on click)
    - Symbol usages / references
  
  * Pretty format - using **nimpretty**
  * Code folding
  * Compile project
  * Compile current file
  * Toggle features on/off

## Requirements

  * Notepad++ x64 v8 (8.9.3 - 8.9.4)
  * Nim v2 (2.0.16, 2.2.6 - 2.2.10) IDE tools in your path
  * Disk space
    * Notepad++ "plugins" directory: 124 KB
    * Temporary directory: 4 KB (minimum)
  * Memory
    * plug-in only: 0.6 MB (minimum)

### Compatibility

  * Not compatible with other plug-in's written in Nim
  * Some features not compatible with Notepad++ auto-completion
  * No code analysis while using "Search > Replace..."
  * Limited features when using "File > New" until saved to file
  * Limited features in split-view until Tab is active

## Installation

nim2_ide is available for personal use under [the NPUL license](https://github.com/gremlin-art/nim2_ide/LICENSE.md).

By downloading, you agree to the terms and conditions of the respective license.

  1. Download from [GitHub "Releases"](https://github.com/gremlin-art/nim2_ide/releases)
  2. Extract and copy files to your Notepad++ plugins directory:
  
```batchfile
cd "C:\Program Files\Notepad++\plugins"
mkdir nim2_ide
copy nim2_ide.dll nim2_ide\nim2_ide.dll
copy nim2_ide.xml Config\nim2_ide.xml
```

  3. Restart Notepad++

## Uninstallation

  1. Exit Notepad++
  2. Remove files from Notepad++ plugins directory:
  
```batchfile
cd "C:\Program Files\Notepad++\plugins"
del nim2_ide\nim2_ide.dll Config\nim2_ide.xml
```

## Notepad++ Configuration

  1. Disable **auto-completion** in *Settings > Preferences... > Auto-Completion*
  2. Switch to a **dark theme** in *Settings > Style Configurator...*
  3. Select **Nim 2** in *Language > N...* to activate plug-in for current tab

### Optional

  1. Toggle **features** by un/checking items in *Plugins > Nim2 IDE*
  2. Customize shortcuts in *Macros > Modify Shortcut/Delete Macro... > Plugin commands*