---
title: Designing Grid Systems For The Web, Mark Boulton — my notes
category: talks
---
# Introduction
- Cannot design a grid system without understanding what you're designing with.
- Odd numbers feel 'right' and have a nice, natural tension. Even numbers can feel boring and safe.
- Lots of print design has a odd number of columns with the first column blank. This is an example of 'active' whitespace which is intentional and has a purpose.
- On the web there is no 'page' from which we can subdivide into columns, so we can't work page-in. Therefore need to work content-out.
- Grid types (you can have one or more, but often will have one primary):
  - Columnar: just columns. Good for when we don't know how long the page is.
  - Hiearchical: horizontal 'layer'-like columns. Smallest sizes of mobile will be almost exclusively hiearchical.
  - Modular: a combination of horizontal and vertical lines creating a split-up page of cells, or 'modules'.
  - Baseline: these follow the baseline of type. Pretty hard on the web!
- Layer up these grids for different devices.
- Don't set up your grid and then set them in stone. They are tools and you should iterate on them.
- Anatomy of grids:
  - Space around grid are margins
  - Space between modules are gutters
  - A 'cell' of content is a module
  - A vertical stack of modules is a column
  - A horizontal line dividing your content is a hanging line, and content is hung off of these. On the web these are the points where you have something like a <div>
  - Fields are a collection of modules, or at least modules spaces
- Creating grids requires a balance between few columns (inflexible but very connected) and lots of columns (flexible but there's much less 'connectedness')
- Breaking out of a global grid is OK, but be careful of finding disconnectedness. Try aligning objects with their closest neighbour. When designing a widget, consider the module/column, when designing a column consider the whole page.
- The concept behind designing a grid is to embed it with the intelligence of our design so we can use it as a tool.

# Designing grids on the web
- Start from the content and work out
  - Find knowable, fixed content sizes (or make them up) and create the grid from that
- Create connectedness
  - Use Ems, not pixels, because pixels are related to the device, not the content
  - Relate *everything* back to the module
  - Use repeated ratios
- Bind the content to the device

# Designing a grid
- Process: understand the content, design your grid, develop typography, then do layouts (and homepage last!)
- Use a content size (eg. an advert or image)
- Make your gutters a division of the module size (eg. 1/4). 
  - Gutters should be wider than you think. 20px is too narrow!
  - They should be an odd number so we can divide them in half with a line whilst still retaining symmetry
- If you have type in a visible box (eg. spanning 3 columns. A 'box out') take the gutter, split it in half to find the middle point, and use that half-width as the indenting for the type in that box.
- Hanging lines should also be defined from the module sizes so they are connected
  - After getting some columns you can start working on zoning and splitting modules up into pieces.
