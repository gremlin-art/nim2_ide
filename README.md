# nim2_ide

Notepad++ plug-in IDE for Nim v2 programming language

## Features

Features can be temporarily disabled via Notepad++ Plugins menu.

  * Full syntax highlighting lexer
  * Unicode lexer
  * Code folding
  * Indentation guides
  * Multi-threading
  * Project aware - using `nimsuggest` "project"
  * Context aware auto-completion
  * Call tips
  * Real-time code analysis
  * Detailed code analysis - on file save
  * Hover (with mouse) for definition
  * Go to definition - on mouse click or key combo
  * Symbol usages - aka. references
  * Pretty format
  * Compile project
  * Compile current file

## Requirements

  * Notepad++ x64 (8.6.4 to 8.7.9)
  * Nim v2 (2.0.2 to 2.2.4) IDE tools in your path - ie. `nim`, `nimpretty`, `nimsuggest`

### Compatibility

  * Not compatible with other Notepad++ plug-in's written in Nim.
  * Some features not compatible with Notepad++ "Other view".

## Known Issues

  * Some features degraded in current Tab after "Save As..." to different file.
    - RCA: Notepad++ returns old filename for "buffer id" of Tab.
    - Workaround: close and re-open Tab.

## Installation

  1. Download from [GitHub](https://github.com/gremlin-art/nim2_ide/releases "Releases")
  2. Extract and copy files to your Notepad++ plugins directory:
  
	> cd "C:\Program Files\Notepad++\plugins"
	> mkdir nim2_ide
	> copy nim2_ide.dll nim2_ide\nim2_ide.dll
	> copy nim2_ide.xml Config\nim2_ide.xml

  3. Restart Notepad++

## Notepad++ Configuration

  1. Disable *native autocomplete* in Settings > Preferences... > Auto-Completion
  2. Switch to a *dark theme* in Settings > Style Configurator...
