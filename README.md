# James Cameron ASCII Art Generator 
This project generates a 29×55 ASCII art portrait of James Cameron using pure Python logic.
Instead of storing the artwork as text, the image is drawn pixel-by-pixel using row and column conditions.

# Overview
The ASCII art is generated using nested loops
Each character is placed based on its (row, column) position
No external libraries are used
The output is printed directly to the terminal
This approach treats ASCII art like a 2D grid, similar to how images are rendered at the pixel level.

# How It Works
1.The canvas size is defined:
height = 29
width = 55
2.Two nested loops iterate over each position:
for row in range(height):
    for column in range(width):
3.Each position starts as a blank space:
    char = " "
4.A large if / elif block assigns characters based on the current row and column:
    if row == 0:
    if column == 17:
        char = "."
    elif column == 18:
        char = "#"
5.Characters such as:
'@' → high density / darkest areas
'#' → medium density
'-' → light structure
'.' → fine detail
are used to shape the portrait.
6.Each completed row is printed to the terminal.

# Features

 No ASCII strings stored in variables
 No libraries or external dependencies
 Fully deterministic output
 Easy to modify individual pixels
 Works in any standard Python environment

# Customization Ideas

Change height and width to scale the canvas
Replace characters (@, #, -, .) for different visual styles
Animate the drawing by printing with delays
Convert the logic into data-driven patterns

# Why This Approach?

Most ASCII art uses static strings.
This project instead constructs the image algorithmically, which is useful for:
  Learning grid-based rendering
  
  Understanding low-level graphics logic
  
  Obfuscation-safe academic projects

  Procedural ASCII art generation
