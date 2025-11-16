# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**DiagnosticTool** is a Python-based Streamlit application for gathering, validating, and displaying application diagnostics through a web dashboard. The project is licensed under Apache 2.0.

**Current Status**: Initial project setup phase. The repository contains documentation and configuration, but the main source code has not yet been implemented.

## Architecture

The system follows a **modular, plugin-based architecture** with these core components:

1. **Data Collection Layer**: Pluggable collectors for gathering system and application metrics
2. **Validation Pipeline**: Configurable rules engine with threshold management for validating collected data
3. **Logging & Audit Layer**: Structured logging with rollback hooks for tracking and auditing
4. **Presentation Layer**: Streamlit-based web dashboard for displaying diagnostics

**Configuration**: YAML-based system for managing component naming, validation thresholds, and plugin registration.

The main application code should reside in a `diagnostic_tool` folder (not yet created).

## Development Commands

**Note**: Build, test, and lint configurations have not yet been established. When setting up the development workflow, typical Python/Streamlit projects use:

- **Run Streamlit app**: `streamlit run <app_file>.py`
- **Package management**: Consider Poetry, pip, or PDM (`.gitignore` is configured for all three)
- **Testing**: pytest (`.gitignore` includes pytest cache patterns)
- **Linting**: Ruff (`.gitignore` includes Ruff cache)
- **Type checking**: MyPy or Pyre (`.gitignore` configured for both)

## Key Files

- `README.md`: Project description and intended architecture
- `.gitignore`: Comprehensive Python project ignore patterns including virtual environments, build artifacts, IDE configs, and tool caches

## Git Workflow

This project uses feature branches with the naming pattern `claude/*`. The main development branch should be confirmed before creating pull requests.
