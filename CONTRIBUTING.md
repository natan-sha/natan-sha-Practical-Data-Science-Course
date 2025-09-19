# Contributing to Practical Data Science Course

We welcome contributions to make this course better! Whether you're fixing bugs, improving documentation, adding new content, or suggesting improvements, your help is appreciated.

## How to Contribute

### 1. Fork and Clone
1. Fork this repository
2. Clone your fork locally:
   ```bash
   git clone https://github.com/YOUR-USERNAME/Practical-Data-Science-Course.git
   cd Practical-Data-Science-Course
   ```

### 2. Set up Development Environment
```bash
# Create virtual environment
python -m venv ds_course
source ds_course/bin/activate  # On Windows: ds_course\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Install pre-commit hooks
pre-commit install
```

### 3. Make Your Changes
- Create a new branch for your feature/fix
- Make your changes following our guidelines below
- Test your changes thoroughly

### 4. Submit a Pull Request
1. Push your changes to your fork
2. Create a pull request with a clear description
3. Reference any related issues

## Contribution Guidelines

### Code Style
- Follow PEP 8 for Python code
- Use meaningful variable and function names
- Add docstrings to functions and classes
- Keep lines under 88 characters (Black formatter)

### Jupyter Notebooks
- Clear cell outputs before committing
- Use markdown cells for explanations
- Include cell numbers for easy reference
- Test all cells execute without errors

### Documentation
- Use clear, concise language
- Include code examples where helpful
- Update README files when adding new content
- Ensure all links work correctly

### Content Guidelines
- Make content accessible to beginners
- Include practical examples and projects
- Provide real-world applications
- Cite sources and references

## Types of Contributions

### 🐛 Bug Reports
- Use the issue template
- Include steps to reproduce
- Provide expected vs. actual behavior
- Include environment details

### 💡 Feature Requests
- Describe the problem you're solving
- Explain why this feature would be valuable
- Provide implementation suggestions if possible

### 📖 Content Improvements
- Fix typos or grammatical errors
- Improve explanations or examples
- Add missing topics or concepts
- Update outdated information

### 🔧 Code Contributions
- Bug fixes
- New features or algorithms
- Performance improvements
- Code refactoring

### 📊 Dataset Contributions
- Add new interesting datasets
- Improve existing dataset documentation
- Create synthetic datasets for examples

## Review Process

1. **Automated Checks**: Your PR will run automated tests
2. **Content Review**: Maintainers will review for accuracy and clarity
3. **Educational Value**: We assess the learning value of contributions
4. **Integration**: We ensure contributions fit well with existing content

## Recognition

Contributors will be acknowledged in:
- README.md contributors section
- Individual topic acknowledgments
- Course credits

## Questions?

- **General Questions**: Use GitHub Discussions
- **Bug Reports**: Create an issue
- **Direct Contact**: [course-email@domain.com]

## Code of Conduct

We are committed to providing a welcoming and inclusive environment. Please:

- Be respectful and professional
- Focus on constructive feedback
- Help create a positive learning environment
- Report any inappropriate behavior

Thank you for contributing to the Practical Data Science Course! 🎓
