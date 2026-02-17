# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Gauntlet is an open-source library for testing and red-teaming conversational AI agents before production deployment.

## Development Setup

This project uses **uv** for Python dependency management with Python 3.12.

```bash
# Install dependencies
uv sync

# Install with dev dependencies (Jupyter support)
uv sync --group dev

# Run the main entry point
uv run python main.py

# Run Jupyter notebooks
uv run jupyter notebook
```

## Project Structure

- `main.py` - Main entry point
- `steering.py` - Steering vector utilities (in development)
- `notebooks/` - Jupyter notebooks for experimentation
- `gauntlet/` - Main package directory (to be developed)

## Key Dependencies

- PyTorch and torchvision for ML operations
- Transformers and Hugging Face Hub for model loading
- Accelerate for distributed training support
