# Contributing to Michal's Home Assistant Add-ons

Thank you for your interest in contributing to this repository! This document provides guidelines for contributing to the add-ons.

## 🚀 Getting Started

### Prerequisites

- Git
- Docker
- Basic knowledge of Home Assistant add-on development
- Python 3.8+ (for Python-based add-ons)

### Development Setup

1. Fork this repository
2. Clone your fork locally:
   ```bash
   git clone https://github.com/YOUR_USERNAME/ha-repository.git
   cd ha-repository
   ```
3. Create a feature branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```

## 📝 Development Guidelines

### Add-on Structure

Each add-on should follow this structure:

```
addon-name/
├── config.yaml          # Add-on configuration
├── build.yaml           # Build configuration
├── Dockerfile           # Container definition
├── README.md            # Add-on documentation
├── CHANGELOG.md         # Version history
├── DOCS.md              # Technical documentation
├── LICENSE              # License file
├── icon.png             # Add-on icon (128x128px)
├── logo.png             # Add-on logo (512x512px)
├── apparmor.txt         # AppArmor profile (if needed)
├── translations/        # Translation files
│   └── en.yaml
└── rootfs/              # Root filesystem
    ├── etc/
    │   └── services.d/
    │       └── addon-name/
    │           ├── run
    │           ├── finish
    │           └── type
    └── usr/
        └── bin/
            └── your-scripts
```

### Code Style

- **Python**: Follow PEP 8 guidelines
- **Shell scripts**: Use bash with proper error handling
- **YAML**: Use consistent indentation (2 spaces)
- **Documentation**: Write clear, concise documentation

### Testing

Before submitting a pull request:

1. **Build the add-on**:
   ```bash
   cd addon-name
   docker build -t test-addon .
   ```

2. **Test locally**:
   ```bash
   docker run -p 8124:8124 -e TV_IP=192.168.1.150 test-addon
   ```

3. **Test on different architectures** (if possible):
   - amd64
   - armhf
   - armv7
   - aarch64

### Documentation

Each add-on must include:

- **README.md**: User-facing documentation
- **DOCS.md**: Technical documentation
- **CHANGELOG.md**: Version history
- **Example configurations**: Show how to use the add-on

## 🔄 Pull Request Process

1. **Create a feature branch** from `main`
2. **Make your changes** following the guidelines above
3. **Test thoroughly** on your local setup
4. **Update documentation** if needed
5. **Commit your changes** with clear commit messages
6. **Push to your fork** and create a pull request

### Commit Message Format

Use conventional commit format:

```
type(scope): description

[optional body]

[optional footer]
```

Examples:
- `feat(nec-tv): add power status checking`
- `fix(nec-tv): resolve connection timeout issue`
- `docs(nec-tv): update installation instructions`

### Pull Request Template

When creating a pull request, include:

- **Description**: What does this PR do?
- **Type of change**: Bug fix, feature, documentation, etc.
- **Testing**: How was this tested?
- **Breaking changes**: Any breaking changes?
- **Screenshots**: If applicable

## 🐛 Bug Reports

When reporting bugs, include:

- **Home Assistant version**
- **Add-on version**
- **Operating system**
- **Steps to reproduce**
- **Expected behavior**
- **Actual behavior**
- **Error logs**

## 💡 Feature Requests

When requesting features:

- **Describe the feature** in detail
- **Explain the use case**
- **Provide examples** if possible
- **Consider implementation complexity**

## 📋 Code Review

All contributions require review before merging. Reviewers will check:

- **Code quality** and style
- **Functionality** and testing
- **Documentation** completeness
- **Security** considerations
- **Performance** impact

## 📄 License

By contributing to this repository, you agree that your contributions will be licensed under the Apache License 2.0.

## 🆘 Getting Help

If you need help:

1. Check the [Home Assistant Add-on Development Documentation](https://developers.home-assistant.io/docs/add-ons/)
2. Search existing issues and pull requests
3. Create a new issue with the `question` label
4. Ask in the [Home Assistant Community](https://community.home-assistant.io/)

## 🙏 Acknowledgments

Thank you for contributing to the Home Assistant ecosystem! Your contributions help make home automation more accessible to everyone. 