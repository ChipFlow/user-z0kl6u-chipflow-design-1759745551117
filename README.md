# chipflow-design-1759745551117

ChipFlow design generated from configurator.

## Design Configuration

- **Template**: ChipFoundry OpenFrame
- **Generated**: 2025-10-06T10:12:31.720Z
- **Enabled Blocks**: 4

## Project Structure

- `design/design.py` - Generated Amaranth HDL design
- `design/software/` - Embedded software for the SoC
- `chipflow.toml` - ChipFlow project configuration  
- `pyproject.toml` - Python dependencies (PDM)
- `.devcontainer/` - Codespaces and dev container configuration
- `Makefile` - Build automation

## Quick Start

This project is optimized for **GitHub Codespaces** with automatic environment setup.

**In a Codespace** (recommended):
```bash
make simulate    # Run ChipFlow simulation
make build       # Generate Verilog
```

**Local development**:
```bash
pip install pdm
pdm install
make simulate
```

## Development Environment

This project uses **PDM** (Python Dependency Manager) and is configured for **GitHub Codespaces** with a devcontainer.

### Codespaces (Recommended)

The project includes a `.devcontainer/devcontainer.json` configuration that:
- Pre-installs Python 3.11, PDM, and development tools
- Sets up VS Code extensions for Python development  
- Automatically installs project dependencies
- Configures the development environment

### Local Development

1. Install PDM:
   ```bash
   pip install pdm
   ```

2. Install dependencies:
   ```bash
   pdm install
   ```

3. Run ChipFlow commands:
   ```bash
   pdm run chipflow sim    # Run simulation
   pdm run chipflow build  # Generate Verilog
   ```

## Available Commands

- `make simulate` - Run ChipFlow simulation
- `make build` - Generate Verilog for synthesis
- `make clean` - Clean build artifacts  
- `make help` - Show all available commands
- `make info` - Show design information

## Enabled IP Blocks

- **Bandgap** (analog)\n- **LDO** (analog)\n- **POR** (analog)\n- **SoC ID** (digital)
