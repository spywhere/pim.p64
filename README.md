# pim.p64 - A vim-like editor for Picotron

## Milestone

- Core
  - Basic editor
  - Window
  - Buffer
  - Sign column
  - Status line
- Basic Functionality
  - Input handling
  - Operators
  - Motions
  - Commands
- Customization
  - Options
  - Key bindings

## Data Structure

- `tabpage.lua` A table of buffers, windows
  - `buffer.lua` A table of lines from a file

## UI Structure

- `ui`
  - `init.lua` UI for the whole editor
    - `bufferline.lua` UI for a top-most bar of the editor
    - `window.lua` UI for a window
      - `buffer.lua` UI for a buffer
        - `signcolumn.lua` UI for a column on the left of a buffer
      - `winbar.lua` UI for a top-most bar of a window
    - `statusline.lua` UI for a bottom-most bar of the editor
