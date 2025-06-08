# Exercise 1: LaTeX Basics

## Task
Create a simple 1-page document that includes:

1. A title, author, and date
2. At least one section and one subsection
3. A paragraph with both **bold** and *italic* text
4. A numbered list and a bullet-point list
5. A simple table with at least 3 columns and 3 rows

## Requirements
- Use the article document class
- Include appropriate packages in the preamble
- Make the title with \maketitle command
- Ensure your document compiles without errors

## Tips
- Start with the minimal document structure we discussed
- Add elements one at a time and compile frequently
- Remember to use proper LaTeX commands for formatting



# Exercise 2: Mathematical Typesetting

## Task
Create a LaTeX document demonstrating various mathematical typesetting features including:

1. A paragraph that includes inline math expressions
2. At least two displayed equations (one numbered, one unnumbered)
3. An equation with fractions, superscripts, subscripts, and Greek letters
4. A piecewise function using the cases environment
5. A matrix equation
6. A multi-line derivation with proper alignment

## Requirements
- Use the article document class
- Include amsmath and amssymb packages
- Use proper math environments for displayed equations
- Ensure consistent spacing in your equations

## Tips
- Use \$ for inline math and \begin{equation} or \[ for displayed math
- Remember to use \left and \right for auto-scaling delimiters
- For alignment, use the align or align* environments
- Test complex expressions separately before combining



# Exercise 3: Document Structure

## Task
Create a structured mathematical document that includes:

1. At least one theorem, one definition, and one example
2. A figure with caption and label
3. A table with caption and label
4. Proper cross-references to all elements (theorems, figures, tables)
5. A table of contents
6. At least two sections with mathematical content

## Requirements
- Use the article document class
- Include necessary packages (amsmath, amsthm, graphicx, etc.)
- Define theorem-like environments in the preamble
- Use \label and \ref for cross-referencing
- Add \tableofcontents at the beginning

## Tips
- Run LaTeX multiple times to resolve references and TOC
- For the figure, you can use a simple image or create one with TikZ
- Make sure all elements are properly labeled
- Organize your document into logical sections before adding content



# Exercise 4: Advanced Topics

## Task
Create a complete mathematical article that includes:

1. Title, author, and abstract
2. Table of contents
3. Mathematical content with properly typeset equations
4. At least one theorem and its proof
5. A figure or diagram (ideally created with TikZ)
6. A table with caption
7. Cross-references to all elements
8. A bibliography with at least two references
9. A custom macro that you define and use

## Requirements
- Use the article document class
- Include appropriate packages for all features
- Define at least one custom command in the preamble
- Include a proper bibliography (manual or using BibTeX)
- Use cross-references throughout the document

## Bonus Goals
- Create a diagram using TikZ
- Format the document according to a journal style
- Use cleveref for enhanced references
- Include an algorithm using algorithm2e or algorithmicx

## Tips
- Start with a template that includes all required sections
- Define your custom macros early in the document
- Test complex elements (like TikZ diagrams) separately
- Don't forget to run BibTeX if you're using it



# Exercise 5: Advanced Figures

## Task
Create a document that demonstrates advanced figure techniques including:

1. Side-by-side figures using minipage (at least 2 figures with separate captions)
2. A 2×2 grid of figures with captions
3. A figure with overlays and annotations using TikZ
4. Text wrapping around a figure (using the wrapfig package)

## Requirements
- Use the article document class
- Include necessary packages (graphicx, tikz, wrapfig, etc.)
- Ensure all figures have proper captions and labels
- Include explanatory text that references the figures

## Tips
- Test each figure arrangement separately before combining them
- Use consistent sizing conventions as percentages of \textwidth
- For placeholder images, you can use "example-image-a" if available
- The TikZ overlay should include arrows, text boxes, or other annotations
