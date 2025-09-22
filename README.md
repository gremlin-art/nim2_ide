# nim2_ide

Notepad++ plug-in IDE for Nim v2 programming language

## Features

  * Multi-pass syntax and symbol highlighting
  
    Syntax highlighting superimposed with _nimsuggest_ symbols.
  
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

  * Notepad++ 8.8.5 x64
  * Nim v2 (2.0.2 to 2.2.4) IDE tools in your path - ie. `nim`, `nimpretty`, `nimsuggest`

### Compatibility

  * Not compatible with other Notepad++ plug-in's written in Nim
  * Not compatible with Notepad++ auto-completion
  * No real-time code linting when using Notepad++ "Search > Replace..."
  * IDE features target the editor tab (with focus) in Notepad++ "split view"

## Installation

  1. Download from [GitHub "Releases"](https://github.com/gremlin-art/nim2_ide/releases)
  2. Extract and copy files to your Notepad++ plugins directory:
  
```batchfile
cd "C:\Program Files\Notepad++\plugins"
mkdir nim2_ide
copy nim2_ide.dll nim2_ide\nim2_ide.dll
copy nim2_ide.xml Config\nim2_ide.xml
```

  3. Restart Notepad++

## Notepad++ Configuration

  1. Disable **auto-completion** in *Settings > Preferences... > Auto-Completion*
  2. Switch to a **dark theme** in *Settings > Style Configurator...*
  3. Select **Nim 2** in *Language > N...* to activate plug-in for current tab

### Optional

  1. Toggle plug-in **features** by un/checking items in *Plugins > Nim2 IDE*
  2. Customize shortcuts in *Macros > Modify Shortcut/Delete Macro... > Plugin commands*
  3. Workaround to prevent **tab key** from triggering _nimsuggest_ code completion
     1. Go to *Settings > Preferences... > Auto-Completion*
     2. Check "Enable auto-completion on each input"
     3. Check "Function completion" radio button
     4. Uncheck "TAB" under *Insert Selection*