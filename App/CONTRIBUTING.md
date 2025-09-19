# Contributing to Energy Consumption Forecasting

Thank you for your interest in contributing to our Energy Consumption Forecasting project! This document outlines the process for contributing to this project.

## 🤝 How to Contribute

### Reporting Issues

1. **Check existing issues** first to avoid duplicates
2. **Use issue templates** when available
3. **Provide detailed information** including:
   - Steps to reproduce
   - Expected vs actual behavior
   - Environment details
   - Screenshots if applicable

### Submitting Changes

1. **Fork the repository**
2. **Create a feature branch** from `main`
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **Make your changes** following our coding standards
4. **Write or update tests** as needed
5. **Update documentation** if required
6. **Commit your changes** with clear messages
7. **Push to your fork** and submit a pull request

## 🛠 Development Setup

### Prerequisites
- Python 3.11+
- Node.js 18+
- MongoDB
- Git

### Local Development
```bash
# Clone your fork
git clone https://github.com/your-username/energy-forecast-pro.git
cd energy-forecast-pro

# Backend setup
cd backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
cp .env.example .env  # Configure your environment

# Frontend setup
cd ../frontend
yarn install
cp .env.example .env  # Configure your environment

# Run the application
# Terminal 1 (Backend):
cd backend && uvicorn server:app --reload --port 8001

# Terminal 2 (Frontend):
cd frontend && yarn start
```

## 📝 Coding Standards

### Python (Backend)
- Follow **PEP 8** style guidelines
- Use **type hints** where appropriate
- Write **docstrings** for functions and classes
- Use **pytest** for testing
- Keep functions focused and small
- Use meaningful variable names

### JavaScript/React (Frontend)
- Use **ES6+** features
- Follow **React best practices**
- Use **functional components** with hooks
- Write **clear, descriptive component names**
- Use **TypeScript** where possible
- Follow **accessibility guidelines**

### General Guidelines
- **Write clear commit messages**
- **Keep changes focused** - one feature per PR
- **Add tests** for new functionality
- **Update documentation** as needed
- **Follow existing patterns** in the codebase

## 🧪 Testing

### Backend Testing
```bash
cd backend
python -m pytest tests/ -v
python -m pytest tests/ --cov=.
```

### Frontend Testing
```bash
cd frontend
yarn test
yarn test --coverage
```

### Integration Testing
```bash
# Run the full application and test all endpoints
python backend_test.py
```

## 📚 Documentation

- Update **README.md** for significant changes
- Add **docstrings** to new functions
- Update **API documentation** for endpoint changes
- Include **examples** in documentation
- Keep **changelog** updated

## 🐛 Bug Fixes

1. **Identify the issue** clearly
2. **Write a test** that reproduces the bug
3. **Fix the issue** with minimal changes
4. **Verify the fix** with existing tests
5. **Update documentation** if needed

## ✨ Feature Requests

1. **Discuss the feature** in an issue first
2. **Consider the scope** and impact
3. **Design the solution** before coding
4. **Implement incrementally** if possible
5. **Add comprehensive tests**
6. **Update documentation**

## 🔍 Code Review Process

### For Contributors
- **Self-review** your code before submitting
- **Write descriptive PR descriptions**
- **Respond to feedback** promptly
- **Keep discussions professional**

### For Reviewers
- **Be constructive** in feedback
- **Focus on code quality** and maintainability
- **Test the changes** locally
- **Check documentation** updates

## 🚀 Release Process

1. **Version bumping** follows semantic versioning
2. **Changelog** updates are required
3. **Testing** on staging environment
4. **Documentation** review
5. **Deployment** to production

## 📋 Pull Request Template

```markdown
## Description
Brief description of changes

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Breaking change
- [ ] Documentation update

## Testing
- [ ] Tests pass locally
- [ ] New tests added
- [ ] Manual testing completed

## Checklist
- [ ] Code follows style guidelines
- [ ] Self-review completed
- [ ] Documentation updated
- [ ] No new warnings introduced
```

## 🎯 Areas for Contribution

### High Priority
- **Performance optimizations**
- **Additional ML models**
- **Enhanced AI insights**
- **Mobile responsiveness**
- **Error handling improvements**

### Medium Priority
- **Data export features**
- **Advanced filtering**
- **Real-time updates**
- **Notification system**
- **Accessibility improvements**

### Low Priority
- **Theme customization**
- **Advanced charting options**
- **Batch operations**
- **Integration with external APIs**

## 💬 Communication

- **GitHub Issues** for bug reports and feature requests
- **Pull Request discussions** for code review
- **Documentation updates** for clarifications

## 📜 Code of Conduct

- **Be respectful** to all contributors
- **Welcome newcomers** and help them learn
- **Focus on constructive feedback**
- **Maintain professional communication**
- **Respect different viewpoints**

## 🙏 Recognition

Contributors will be recognized in:
- **README.md** contributors section
- **Release notes** for significant contributions
- **Documentation** where appropriate

## 📞 Getting Help

If you need help with contributing:
1. Check existing **documentation**
2. Search **closed issues** for similar problems
3. Open a **new issue** with the "help wanted" label
4. Join our **community discussions**

Thank you for contributing to Energy Consumption Forecasting! 🚀
