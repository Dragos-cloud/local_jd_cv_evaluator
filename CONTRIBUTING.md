# Contributing to Local CV-JD Evaluator

First off, thank you for considering contributing to Local CV-JD Evaluator! 🎉

The following is a set of guidelines for contributing to this project. These are mostly guidelines, not rules. Use your best judgment, and feel free to propose changes to this document in a pull request.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Development Setup](#development-setup)
- [Coding Guidelines](#coding-guidelines)
- [Pull Request Process](#pull-request-process)
- [Issue Reporting](#issue-reporting)

## Code of Conduct

This project and everyone participating in it is governed by our commitment to creating a welcoming, inclusive, and harassment-free environment for everyone. By participating, you are expected to uphold these standards.

## How Can I Contribute?

### 🐛 Reporting Bugs

Before creating bug reports, please check existing issues to avoid duplicates. When you create a bug report, include as many details as possible:

- **Use a clear and descriptive title**
- **Describe the exact steps to reproduce the problem**
- **Provide specific examples** (input text, model used, etc.)
- **Describe the behavior you observed and what you expected**
- **Include screenshots** if applicable
- **Specify your environment**: OS, browser, LM Studio version, model used

### 💡 Suggesting Enhancements

Enhancement suggestions are welcome! Please:

- **Use a clear and descriptive title**
- **Provide a step-by-step description** of the suggested enhancement
- **Explain why this enhancement would be useful**
- **Consider the project's scope** (privacy-first, standalone, offline-capable)

### 📝 Improving Documentation

Documentation improvements are always appreciated:

- Fix typos or clarify confusing sections
- Add missing information or examples
- Improve setup instructions
- Add troubleshooting guides

### 💻 Code Contributions

We welcome code contributions! Areas that need help:

- **UI/UX Improvements**: Better responsive design, accessibility features
- **Analysis Features**: New analysis types or improved prompts
- **Export Functionality**: Additional export formats or better formatting
- **Performance**: Optimization for large inputs or slower devices
- **Browser Compatibility**: Ensuring compatibility across different browsers
- **Error Handling**: Better error messages and recovery

## Development Setup

### Prerequisites

1. **Text Editor/IDE**: VS Code, Sublime Text, or any editor with HTML/CSS/JavaScript support
2. **LM Studio**: For testing the application
3. **Modern Browser**: For testing functionality
4. **Git**: For version control

### Local Development

1. **Fork and Clone**
   ```bash
   git clone https://github.com/yourusername/local_jd_cv_evaluator.git
   cd local_jd_cv_evaluator
   ```

2. **Open the HTML File**
   - Open `standalone_cv_jd_evaluator.html` in your browser
   - Or use a local server for development:
     ```bash
     # Python 3
     python -m http.server 8000
     
     # Python 2
     python -m SimpleHTTPServer 8000
     
     # Node.js (with http-server)
     npx http-server
     ```

3. **Setup LM Studio**
   - Install and configure LM Studio
   - Load a test model
   - Start the local server

4. **Test Your Changes**
   - Test all functionality thoroughly
   - Try different models and input types
   - Verify export functions work correctly
   - Test error scenarios

## Coding Guidelines

### HTML Structure

- Use semantic HTML elements where appropriate
- Maintain accessibility standards (alt text, ARIA labels)
- Keep the single-file structure intact

### CSS Standards

- Use CSS custom properties (variables) for consistency
- Follow the existing naming convention
- Ensure responsive design principles
- Test across different screen sizes

### JavaScript Guidelines

- Use ES6+ features consistently
- Follow existing code style and patterns
- Add comprehensive error handling
- Include JSDoc comments for new functions
- Maintain the class-based architecture

#### Code Style

```javascript
// ✅ Good
async function analyzeText(inputText, options) {
    if (!inputText?.trim()) {
        throw new Error('Input text is required');
    }
    
    try {
        const result = await this.processAnalysis(inputText, options);
        return result;
    } catch (error) {
        console.error('Analysis failed:', error);
        throw error;
    }
}

// ❌ Avoid
function analyzeText(inputText,options){
    var result=this.processAnalysis(inputText,options);
    return result;
}
```

### Performance Considerations

- Optimize for large text inputs
- Implement proper loading states
- Use efficient DOM manipulation
- Consider memory usage with large responses

### Privacy & Security

- Never add external tracking or analytics
- Ensure all processing remains local
- Don't log sensitive user data
- Validate and sanitize user inputs

## Pull Request Process

### Before Submitting

1. **Test thoroughly** on multiple browsers and screen sizes
2. **Verify LM Studio integration** works correctly
3. **Check for console errors** and fix any issues
4. **Update documentation** if your changes affect usage
5. **Follow the existing code style** and patterns

### Pull Request Template

When submitting a pull request, please:

1. **Use a clear title** that describes the change
2. **Reference related issues** using GitHub's syntax (`fixes #123`)
3. **Describe your changes** in detail
4. **Include screenshots** for UI changes
5. **List testing steps** you performed

### Review Process

1. **Automated checks** will run (when available)
2. **Manual review** by maintainers
3. **Testing** of functionality
4. **Discussion** and potential revision requests
5. **Merge** once approved

## Issue Reporting

### Bug Reports

Use the bug report template and include:

- **Environment details** (OS, browser, LM Studio version)
- **Steps to reproduce** the issue
- **Expected vs actual behavior**
- **Screenshots or error messages**
- **Input examples** that caused the issue

### Feature Requests

Use the feature request template and include:

- **Clear description** of the proposed feature
- **Use case** and benefits
- **Mockups or examples** if applicable
- **Implementation considerations**

### Questions and Discussions

For questions about usage or general discussions:

- Use GitHub Discussions for broader topics
- Use Issues for specific problems or requests
- Check existing issues and discussions first

## Recognition

Contributors will be recognized in the project documentation. Significant contributors may be invited to become maintainers.

## Getting Help

If you need help with contributing:

- Check existing issues and discussions
- Create a new discussion for questions
- Reach out through GitHub issues for specific problems

## Development Tips

### Testing Different Scenarios

Always test with:
- **Various model sizes** (7B, 13B, etc.)
- **Different input lengths** (short, medium, very long)
- **Edge cases** (empty inputs, special characters)
- **Different browsers** and devices
- **Network scenarios** (offline mode)

### Common Pitfalls

- **CORS issues**: Test with actual file:// URLs, not just local servers
- **Model compatibility**: Different models may respond differently
- **Performance**: Large inputs can cause browser slowdowns
- **Memory management**: Clean up resources properly

### Useful Resources

- [LM Studio Documentation](https://lmstudio.ai/docs)
- [OpenAI API Reference](https://platform.openai.com/docs/api-reference)
- [MDN Web Docs](https://developer.mozilla.org/en-US/)
- [HTML Living Standard](https://html.spec.whatwg.org/)

## Thank You! 🙏

Your contributions help make this tool better for everyone while maintaining our commitment to privacy and offline functionality.

---

Happy contributing! 🚀