# Laser Stuff

A monorepo for laser cutter projects, documentation, and guides.

## Overview

This repository contains documentation and resources for various laser cutting projects, primarily focused on CO2 laser cutters. Each project is self-contained with its own documentation, design files, and instructions.

## Projects

- **[Elegoo Saturn 4 Ultra Fresnel Lens](./projects/elegoo-saturn-4-ultra-fresnel-lens/)** - Guide for cutting a replacement fresnel lens for the Elegoo Saturn 4 Ultra 3D printer using a CO2 laser cutter

## Quick Start

### For Users
Browse the [projects directory](./projects/) to find guides and documentation for specific laser cutting projects.

### For Developers

1. **Clone the repository**
   ```bash
   git clone https://github.com/sayhiben/laser-stuff.git
   cd laser-stuff
   ```

2. **Install development tools**
   ```bash
   pip install ruff pre-commit
   ```

3. **Set up pre-commit hooks** (optional but recommended)
   ```bash
   pre-commit install
   ```

4. **Lint and format code**
   ```bash
   # Check code with ruff
   ruff check .
   
   # Format code with ruff
   ruff format .
   ```

## Repository Structure

```
laser-stuff/
├── projects/              # Individual laser cutting projects
│   └── elegoo-saturn-4-ultra-fresnel-lens/
├── reference/            # Reference materials and index
│   └── INDEX.md         # Master index of all files
├── .github/workflows/    # CI/CD workflows
└── README.md            # This file
```

For a detailed description of all files and when to read them, see the [Reference Index](./reference/INDEX.md).

## Contributing

Contributions are welcome! When adding new projects:

1. Create a new directory under `projects/`
2. Include a comprehensive `README.md` in your project directory
3. Update the [Reference Index](./reference/INDEX.md)
4. Ensure code passes ruff linting and formatting
5. Add your project to the test matrix in `.github/workflows/test.yml` if applicable

## Development Tools

This repository uses:
- **[Ruff](https://github.com/astral-sh/ruff)** - Fast Python linter and formatter
- **[pre-commit](https://pre-commit.com/)** - Git hook framework for running checks before commits
- **GitHub Actions** - Automated testing and linting on pull requests

## License

See [LICENSE](./LICENSE) for details.
