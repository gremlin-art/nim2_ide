# nim2_ide

Notepad++ plug-in IDE for Nim v2 programming language

## Features

  * Full syntax highlighting lexer
  
    Highlight more Nim features than other lexers.
  
  * Unicode lexer
  
    Highlight Nim unicode operators.
  
  * Managed multi-thread backend
  
    No LSP bloat. Automatically prune threads and _nimsuggest_ processes.
  
  * One nimsuggest per project
  
    Efficiently share one _nimsuggest_ process among files in a directory tree.
  
  * Advanced features - using **nimsuggest**
    - Project aware
    - Context aware auto-completion
    - Call tips
    - Real-time code analysis
    - Detailed code analysis (on file save)
    - Highlight symbols (on scroll)
    - Hover (with mouse) for definition
    - Go to definition (on mouse click)
    - Symbol usages (references)
  
  * Pretty format - using **nimpretty**
  * Code folding
  * Compile project
  * Compile current file
  * Toggle features on/off

## Requirements

  * Notepad++ x64 (8.6.4 to 8.8.5)
  * Nim v2 (2.0.2 to 2.2.4) IDE tools in your path - ie. `nim`, `nimpretty`, `nimsuggest`

### Compatibility

  * Not compatible with other Notepad++ plug-in's written in Nim.
  * Some features not compatible with Notepad++ "Other view".

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

  1. Disable **native autocomplete** in *Settings > Preferences... > Auto-Completion*
  2. Switch to a **dark theme** in *Settings > Style Configurator...*
  3. Select **Nim 2** in *Language > N...* to activate plug-in for current tab.
  4. Optional: Toggle plug-in features by un/checking items in *Plugins > Nim2 IDE*
  5. Optional: Customize shortcuts in *Macros > Modify Shortcut/Delete Macro... > Plugin commands*
