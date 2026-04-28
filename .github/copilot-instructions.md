# Copilot Instructions for PyTorch Tutorial Basics

## Project Overview
This repository contains educational Jupyter notebooks for learning PyTorch and neural networks from first principles. The project includes:

- **Lab notebooks**: Hands-on exercises teaching neural network concepts (forward propagation, tensor operations, autograd)
- **Reference materials**: Tutorial notebooks demonstrating PyTorch basics
- **Tutorial format**: Markdown explanations paired with progressive code cells designed for learning

## Key Architecture & Patterns

### Notebook Structure
- **Mixed cell types**: Markdown cells provide explanations, theory, and mathematical formulas; Python cells contain executable code
- **Progressive learning**: Each notebook builds incrementally—early cells establish foundational concepts, later cells apply them
- **Intentional gaps**: Some code cells are left blank (`### type your answer here`) for students to complete as exercises
- **Solution hints**: Markdown cells contain collapsed HTML comments with solutions that can be revealed

### PyTorch/NumPy Usage
- **NumPy for math basics**: Early labs use NumPy to demonstrate neural network calculations from scratch (see `c01b-m01h-Lab1--Forward-Propgat-py-v1.jupy.ipynb`)
- **PyTorch for production**: `01_pytorch_basics.ipynb` shows proper PyTorch patterns including:
  - Tensor creation and shape manipulation (reshape, view, unsqueeze, squeeze)
  - Autograd for automatic differentiation (requires_grad=True)
  - GPU/device management

### Neural Network Concepts Covered
- Forward propagation: Computing weighted sums (z) and activations through network layers
- Weight/bias initialization: Random uniform initialization, then manual assignment
- Node computation: Weighted sums at hidden and output layers using linear algebra

## Critical Developer Workflows

### Running & Viewing Notebooks
- Use VS Code's Jupyter extension to open `.ipynb` files
- Execute cells individually (Ctrl+Enter) or sequentially
- Use "Run All" carefully—some notebooks have intentional blank cells students should fill

### Adding or Modifying Content
- Maintain the teaching flow: conceptual explanation → code demonstration → exercise
- When adding formulas, use LaTeX math syntax (wraps in `$...$` for inline, `$$...$$` for blocks)
- Keep exercise cells intentionally blank with clear comments
- Add solution hints as HTML comments in following markdown cells

## Project-Specific Conventions

### File Organization
- `.github/`: Contains all notebook files, step guides, and workflows
- Notebook naming: Descriptive with course codes (e.g., `c01b-m01h-Lab1--Forward-Propgat-py-v1.jupy.ipynb`)

### Code Style
- Use descriptive variable names matching mathematical notation when possible (e.g., `z_11` for $z_{1,1}$)
- Always include print statements for verification/debugging
- Initialize weights and biases explicitly; document why (teaching tool)

### Testing & Validation
- Verify notebooks execute from top to bottom without errors
- Confirm exercise cells are properly marked and solvable with reasonable effort
- Check that all LaTeX formulas render correctly in the notebook viewer

## Dependencies
- **NumPy**: For numerical computations and tensor operations
- **PyTorch**: For deep learning frameworks and autograd
- **Python 3.x**: Standard library

Notebooks include pip install comments (commented out) for environments where packages aren't pre-installed (e.g., local development vs. IBM Skills Network).

## Common Tasks

**Add a new exercise**: Create markdown cells with theory, then a blank code cell with `### type your answer here`, followed by a hint cell with collapsed HTML solution.

**Extend a tutorial**: Follow the progressive pattern—explain new concept in markdown, implement in code cell, add verification print statements.

**Debug exercise completion**: Check that student solutions logically follow from earlier cells and match the mathematical concepts explained in preceding markdown.
