# Contributing to BlueRoots 🌱

Thank you for your interest in contributing to BlueRoots! This document provides guidelines for contributing to the project.

## Code of Conduct

By participating in this project, you agree to abide by our Code of Conduct. Please treat all contributors with respect and create a welcoming environment for everyone.

## Getting Started

1. Fork the repository on GitHub
2. Clone your fork locally
3. Create a virtual environment and install dependencies
4. Create a new branch for your feature or bugfix
5. Make your changes and test them
6. Submit a pull request

## Development Setup

```bash
# Clone your fork
git clone https://github.com/YOUR_USERNAME/blue_roots.git
cd blue_roots

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
pip install -r requirements-dev.txt  # Development dependencies

# Install pre-commit hooks
pre-commit install
```

## How to Contribute

### Reporting Bugs

- Use the GitHub Issues page
- Follow the bug report template
- Include detailed steps to reproduce
- Provide environment information
- Add relevant screenshots or data samples

### Suggesting Features

- Use the GitHub Issues page
- Follow the feature request template
- Explain the use case and benefits
- Consider implementation complexity

### Code Contributions

#### Pull Request Process

1. **Branch naming**: Use descriptive names like `feature/satellite-data-api` or `fix/dashboard-loading-bug`

2. **Commit messages**: Write clear, descriptive commit messages
   ```
   feat: add Sentinel-2 data processing pipeline
   fix: resolve dashboard memory leak in image viewer
   docs: update API documentation for health classifier
   ```

3. **Code style**: Follow PEP 8 and use the provided linting tools
   ```bash
   # Run linting
   flake8 .
   black .
   isort .
   ```

4. **Testing**: Ensure all tests pass and add new tests for your changes
   ```bash
   # Run tests
   pytest tests/
   
   # Run specific test category
   pytest tests/test_models.py
   ```

5. **Documentation**: Update documentation for new features or API changes

#### Code Review Guidelines

- All pull requests require at least one review
- Address feedback promptly and respectfully
- Keep pull requests focused and reasonably sized
- Update your branch with the latest main branch changes

### Areas for Contribution

#### 🤖 Machine Learning
- Model improvements and optimizations
- New algorithms for mangrove health assessment
- Data augmentation techniques
- Model interpretability features

#### 📊 Dashboard & Visualization
- New chart types and visualizations
- UI/UX improvements
- Performance optimizations
- Mobile responsiveness

#### 🛠️ Data Processing
- New satellite data source integrations
- Preprocessing pipeline improvements
- Data validation and quality checks
- Automated data collection

#### 📚 Documentation
- API documentation improvements
- Tutorial creation
- Code examples and notebooks
- Translation to other languages

#### 🧪 Testing
- Unit test coverage improvements
- Integration tests
- Performance benchmarks
- Data validation tests

## Coding Standards

### Python Code Style

- Follow PEP 8 guidelines
- Use type hints where applicable
- Write docstrings for all public functions and classes
- Keep functions small and focused
- Use meaningful variable and function names

### Documentation Style

- Use Google-style docstrings
- Include examples in docstrings
- Update README.md for new features
- Add inline comments for complex logic

### Testing Standards

- Write tests for new functionality
- Maintain high test coverage (>80%)
- Use descriptive test names
- Include both positive and negative test cases
- Test edge cases and error conditions

## Data Guidelines

### Working with Satellite Data

- Always include data source attribution
- Document data preprocessing steps
- Validate data quality and completeness
- Consider privacy and usage restrictions
- Use efficient data formats (e.g., HDF5, zarr)

### Model Development

- Document model architecture decisions
- Include performance benchmarks
- Provide model validation results
- Consider computational efficiency
- Plan for model versioning and deployment

## Community

### Getting Help

- Join our GitHub Discussions for questions
- Use GitHub Issues for bug reports
- Check existing documentation and FAQ

### Communication

- Be respectful and constructive
- Ask questions if something is unclear
- Share knowledge and help others
- Participate in code reviews

## Recognition

Contributors will be recognized in:
- README.md contributors section
- Release notes for significant contributions
- GitHub contributor statistics

## License

By contributing, you agree that your contributions will be licensed under the same MIT License that covers the project.

---

Thank you for helping make BlueRoots better! 🌱