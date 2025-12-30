# Mellea for GRC

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ethanolivertroy/mellea-for-grc/blob/main/grc-tutorial.ipynb)
[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)

Tutorial for building GRC automation with Mellea and LLMs. Covers SOC2/ISO 27001 compliance checking, policy validation, control testing, and policy-as-code.

## Quick Start

**Colab:** Click badge above, run cells top-to-bottom. First cell installs everything.

**Local:**
```bash
# Install Ollama
curl -fsSL https://ollama.com/install.sh | sh

# Get models
ollama serve &
ollama pull granite3.3:8b
ollama pull llama3.2:3b

# Install Mellea
pip install "mellea[all] @ git+https://github.com/generative-computing/mellea@v0.0.5"

# Run
jupyter notebook grc-tutorial.ipynb
```

First run downloads ~4GB model weights.

## Labs

1. **SOC2 Compliance Checking** - Query requirements, generate access policies
2. **IVR Policy Validation** - Password policy generation with automated validation
3. **Evidence Analysis** - Composable assessment pipelines with `@generative`
4. **Document Processing** - Extract/analyze compliance tables from PDFs
5. **Policy-as-Code** - Version-controlled SOC2 control database with MObjects

## Use Cases

- Compliance checking (SOC2, ISO 27001)
- Risk assessment and identification
- Control testing automation
- Policy generation from requirements
- GitOps workflows for GRC

## Stack

- **Mellea** - LLM framework with IVR pattern
- **Ollama** - Local LLM runtime
- **Granite 3.3 (8B)** - IBM's open-source model
- **Docling** - Document/table processing

## Validation

All code cells syntax-checked. 37/37 validation checks passed. Ready for use.

## Resources

- [Mellea Documentation](https://docs.mellea.ai)
- [Mellea GitHub](https://github.com/generative-computing/mellea)
- [Ollama](https://github.com/ollama/ollama)
- [SOC2 Framework](https://www.aicpa-cima.com/topic/audit-assurance/audit-and-assurance-greater-than-soc-2)

## License

Educational use. Mellea subject to its own license.
