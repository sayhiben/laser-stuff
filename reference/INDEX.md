# Reference Index

This index describes the contents of the laser-stuff monorepo, including what each file does and when you might want to read it.

## Repository Structure

```
laser-stuff/
├── projects/              # Individual laser cutting projects
├── reference/            # Reference materials and this index
├── .github/workflows/    # GitHub Actions CI/CD workflows
├── pyproject.toml       # Python project configuration and ruff settings
├── .pre-commit-config.yaml  # Pre-commit hooks configuration
└── README.md            # Main repository README
```

## Core Files

### `README.md`
**What it is**: Main repository overview and getting started guide

**When to read it**: 
- First time visiting this repository
- Want to understand the overall purpose and structure
- Looking for quick links to specific projects

### `pyproject.toml`
**What it is**: Python project configuration file containing ruff linter and formatter settings

**When to read it**:
- Setting up development environment
- Configuring your IDE for linting/formatting
- Understanding code style rules for this repository
- Adding new Python dependencies

### `.pre-commit-config.yaml`
**What it is**: Configuration for pre-commit hooks that run automated checks before commits

**When to read it**:
- Setting up pre-commit hooks locally
- Understanding what checks run before commits
- Adding new pre-commit hooks
- Troubleshooting commit issues

### `.gitignore`
**What it is**: Specifies which files Git should ignore (build artifacts, cache files, etc.)

**When to read it**:
- Files aren't being tracked that should be
- Files are being tracked that shouldn't be
- Adding new types of generated files

## GitHub Actions Workflows

### `.github/workflows/test.yml`
**What it is**: GitHub Actions workflow that runs linting and tests on all projects

**When to read it**:
- Understanding what checks run on pull requests
- Setting up similar CI/CD for your own projects
- Troubleshooting workflow failures
- Adding new test jobs for new projects

**What it does**:
- Runs ruff linting on all Python code
- Runs ruff format check to ensure code is properly formatted
- Tests each project in the monorepo (if tests exist)
- Automatically installs project dependencies

## Projects

### `projects/elegoo-saturn-4-ultra-fresnel-lens/`
**What it is**: Documentation and guide for cutting a replacement fresnel lens for the Elegoo Saturn 4 Ultra 3D printer

**When to read it**:
- You have an Elegoo Saturn 4 Ultra with a damaged lens
- You want to learn how to cut acrylic/PMMA with a CO2 laser
- You're interested in 3D printer maintenance and repair
- You need laser cutter settings for fresnel lens material

**Key contents**:
- Material specifications and sourcing
- Laser cutter settings (power, speed, frequency)
- Step-by-step cutting process
- Safety considerations
- Troubleshooting guide
- Installation instructions

## Reference Materials

### `reference/INDEX.md` (this file)
**What it is**: Master index describing all files in the repository

**When to read it**:
- Looking for something specific but don't know where it is
- Want to understand the overall repository organization
- Need to know what a specific file is for
- Contributing to the repository and need context

## Getting Started

1. **For general users**: Start with the main `README.md`
2. **For developers**: Read `pyproject.toml` and `.pre-commit-config.yaml` to set up your environment
3. **For project-specific information**: Navigate to the relevant project folder and read its README
4. **For CI/CD**: Check `.github/workflows/test.yml` to understand automated checks

## Contributing

When adding new projects:
1. Create a new directory under `projects/`
2. Include a comprehensive README.md in the project directory
3. Update this index with information about your project
4. Add your project to the matrix in `.github/workflows/test.yml` if it has tests
5. Run pre-commit hooks or ruff locally before committing

## Maintenance

This index should be updated whenever:
- New projects are added
- New configuration files are added
- The repository structure changes significantly
- New workflows or automation is added
