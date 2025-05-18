# Contributing to Air-Smart Controller

First off, thank you for considering contributing to the Air-Smart Controller project! 🎉 Your contributions help advance research in indoor air quality prediction and smart home automation.

## 📋 Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Development Setup](#development-setup)
- [Contributing Guidelines](#contributing-guidelines)
- [Pull Request Process](#pull-request-process)
- [Issue Reporting](#issue-reporting)
- [Research & Academic Contributions](#research--academic-contributions)
- [Community Guidelines](#community-guidelines)

## 🤝 Code of Conduct

This project adheres to a Code of Conduct. By participating, you are expected to uphold this code:

- Use welcoming and inclusive language
- Be respectful of differing viewpoints and experiences
- Gracefully accept constructive criticism
- Focus on what is best for the community and research advancement
- Show empathy towards other community members

## 🛠️ How Can I Contribute?

### Types of Contributions We Welcome

- **🐛 Bug Reports**: Help us identify and fix issues
- **💡 Feature Requests**: Suggest new functionality or improvements
- **📊 Model Improvements**: Enhance prediction accuracy or efficiency
- **📖 Documentation**: Improve clarity, add examples, or translate content
- **🧪 Test Coverage**: Add tests for existing or new functionality
- **🔬 Research Extensions**: Contribute new datasets, models, or analysis methods
- **🎨 UI/UX Enhancements**: Improve the Streamlit interface
- **⚡ Performance Optimizations**: Make the system faster or more efficient

## 🖥️ Development Setup

### Prerequisites

- Python 3.8+ 
- Git
- Jupyter Notebook/JupyterLab
- A virtual environment tool (venv, conda, etc.)

### Local Development Environment

1. **Fork the repository**
   ```bash
   # Click 'Fork' on GitHub, then clone your fork
   git clone https://github.com/YOUR_USERNAME/air-smart-controller.git
   cd air-smart-controller
   ```

2. **Set up virtual environment**
   ```bash
   # Using venv
   python -m venv airquality-env
   source airquality-env/bin/activate  # Windows: airquality-env\Scripts\activate
   
   # OR using conda
   conda create -n airquality-env python=3.8
   conda activate airquality-env
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   pip install -r requirements-dev.txt  # If available
   ```

4. **Verify installation**
   ```bash
   # Test the Streamlit app
   streamlit run Smart-Air.py
   
   # Test Jupyter notebook
   jupyter notebook Air_Quality_Prediction.ipynb
   ```

### Development Dependencies

For development, you may need additional packages:
```bash
pip install pytest black flake8 isort jupyter-notebook mypy
```

## 📝 Contributing Guidelines

### Code Style

- **Python**: Follow PEP 8 guidelines
- **Formatting**: Use `black` for code formatting
  ```bash
  black --line-length 88 .
  ```
- **Linting**: Use `flake8` for linting
  ```bash
  flake8 --max-line-length=88 --extend-ignore=E203,W503 .
  ```
- **Import sorting**: Use `isort`
  ```bash
  isort --profile black .
  ```

### Jupyter Notebook Guidelines

- **Clear outputs** before committing:
  ```bash
  jupyter nbconvert --clear-output --inplace Air_Quality_Prediction.ipynb
  ```
- **Add markdown cells** to explain complex analysis steps
- **Include comments** in code cells for clarity
- **Use meaningful variable names** and avoid single-letter variables
- **Document model hyperparameters** and their rationale

### Data Handling Standards

- **Never commit large datasets** to the repository
- **Use relative paths** for data file references
- **Document data sources** and preprocessing steps
- **Include data validation checks** in your code
- **Respect data privacy** and licensing agreements

### Model Development Guidelines

1. **Baseline Comparison**: Always compare new models against existing baselines
2. **Reproducibility**: Set random seeds and document environment
3. **Performance Metrics**: Include comprehensive evaluation metrics
4. **Documentation**: Explain model architecture choices and hyperparameter decisions
5. **Validation**: Use proper train/validation/test splits

## 🔄 Pull Request Process

### Before Submitting

1. **Create a new branch** for your feature
   ```bash
   git checkout -b feature/your-feature-name
   # OR
   git checkout -b bugfix/issue-number
   ```

2. **Ensure your code follows our guidelines**
   - Run formatting tools
   - Clear notebook outputs
   - Update documentation if needed

3. **Test your changes**
   - Verify the Streamlit app runs correctly
   - Test all notebook cells execute without errors
   - Check that model performance hasn't degraded

### Pull Request Template

When creating a PR, please include:

```markdown
## Description
Brief description of changes and motivation

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Model improvement
- [ ] Documentation update
- [ ] Performance optimization

## Testing
- [ ] Streamlit app runs correctly
- [ ] All notebook cells execute successfully
- [ ] Model performance validated
- [ ] Tests pass (if applicable)

## Screenshots/Results
Include relevant visualizations or performance metrics

## Additional Notes
Any additional context or considerations
```

### Review Process

1. Automated checks must pass (if configured)
2. At least one maintainer review required
3. All conversations must be resolved
4. No conflicts with main branch

## 🐛 Issue Reporting

### Bug Reports

Use the bug report template and include:

- **Environment details** (Python version, OS, package versions)
- **Steps to reproduce** the error
- **Expected vs actual behavior**
- **Error messages or screenshots**
- **System specifications** if performance-related

### Feature Requests

- **Describe the problem** your feature would solve
- **Proposed solution** with implementation details if possible
- **Alternative solutions** you've considered
- **Impact assessment** on existing functionality

### Performance Issues

- **Benchmark results** showing the issue
- **Profiling information** if available
- **Hardware specifications**
- **Dataset characteristics** (size, complexity)

## 🔬 Research & Academic Contributions

### Adding New Models

1. **Literature review**: Ensure novelty and cite relevant papers
2. **Implementation**: Follow established patterns in the codebase
3. **Evaluation**: Compare against existing models using the same metrics
4. **Documentation**: Include theoretical background and implementation details

### Dataset Contributions

1. **Data licensing**: Ensure proper permissions for sharing
2. **Documentation**: Provide detailed metadata and collection methodology
3. **Quality assurance**: Include data validation and cleaning procedures
4. **Privacy compliance**: Remove or anonymize sensitive information

### Research Papers

If your contribution leads to publishable research:

1. **Cite the project** in your acknowledgments
2. **Share drafts** with maintainers before submission
3. **Update documentation** with new findings
4. **Consider co-authorship** for significant contributions

## 👥 Community Guidelines

### Communication Channels

- **GitHub Issues**: Technical discussions and bug reports
- **GitHub Discussions**: General questions and feature brainstorming
- **Email**: Direct contact with maintainers for sensitive matters

### Recognition

Contributors will be recognized in:
- README.md contributors section
- Academic publications (for research contributions)
- Release notes for significant contributions

### Getting Help

- **Documentation**: Check existing docs and README first
- **Search issues**: Your question might already be answered
- **Ask questions**: Don't hesitate to open a discussion or issue
- **Join the community**: Participate in discussions and help others

## 📊 Performance Benchmarks

When contributing model improvements, please include:

### Required Metrics
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Training/inference time
- Memory usage

### Evaluation Environment
- Hardware specifications
- Software versions (Python, dependencies)
- Dataset splits used
- Random seeds for reproducibility

## 📚 Additional Resources

- [Python Style Guide](https://pep8.org/)
- [Jupyter Best Practices](https://jupyter.readthedocs.io/en/latest/community/content-community.html)
- [Streamlit Documentation](https://docs.streamlit.io/)
- [Scientific Python Development Guide](https://learn.scientific-python.org/development/)

## 🙏 Acknowledgments

Thank you to all contributors who have helped improve this project! Your efforts advance the field of smart home automation and indoor environmental control.

---

For questions about contributing, please contact [kadirqokdeniz@hotmail.com](mailto:kadirqokdeniz@hotmail.com) or open a GitHub discussion.

**Happy Contributing! 🚀**
