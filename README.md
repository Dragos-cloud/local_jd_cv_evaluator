# Local CV-JD Evaluator 🔍

A **privacy-first**, standalone AI-powered CV and Job Description analysis tool that runs entirely offline using LM Studio.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub release](https://img.shields.io/github/release/yourusername/local_jd_cv_evaluator.svg)](https://GitHub.com/yourusername/local_jd_cv_evaluator/releases/)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/yourusername/local_jd_cv_evaluator/graphs/commit-activity)

## 🚀 Features

- **Complete Privacy**: All analysis happens locally - no data leaves your computer
- **No API Keys Required**: Uses LM Studio for local AI model inference
- **Comprehensive Analysis**:
  - Job Description Requirements Analysis
  - CV-Job Fit Assessment
  - Skills Gap Identification
  - CV Optimization Recommendations
  - Corporate Jargon Translation
- **Multiple Export Formats**: TXT, DOCX, JSON
- **User-Friendly Interface**: Clean, modern web interface
- **Standalone**: Single HTML file - no installation required

## 🔧 Prerequisites

1. **LM Studio**: Download and install from [lmstudio.ai](https://lmstudio.ai/)
2. **Compatible AI Model**: Any chat/completion model compatible with OpenAI API format
3. **Modern Web Browser**: Chrome, Firefox, Safari, or Edge

## 🏗️ Setup Instructions

### Step 1: Install LM Studio
1. Download LM Studio from [lmstudio.ai](https://lmstudio.ai/)
2. Install and launch the application
3. Download a compatible model (recommended: Llama 2 7B or similar)

### Step 2: Start LM Studio Server
1. In LM Studio, go to the "Local Server" tab
2. Load your chosen model
3. Start the server (default: `http://localhost:1234`)
4. Ensure the server is running before using the tool

### Step 3: Run the CV-JD Evaluator
1. Download `standalone_cv_jd_evaluator.html`
2. Open the file in your web browser
3. Click "Test Connection" to verify LM Studio connectivity
4. Select your model from the dropdown
5. Start analyzing!

## 📖 Usage Guide

### Basic Workflow
1. **Configure Connection**: Test and confirm LM Studio connection
2. **Select Model**: Choose from available models in the dropdown
3. **Input Data**:
   - **Job Description** (required): Paste the job posting
   - **CV/Resume** (optional): Paste your CV for matching analysis
   - **Additional Focus** (optional): Specify particular areas of interest
4. **Choose Analysis Options**:
   - ✅ JD Requirements Analysis
   - ✅ CV Fit Assessment (requires CV input)
   - ✅ Skills Gap Identification (requires CV input)
   - ✅ CV Optimization (requires CV input)
   - ✅ Corporate Jargon Translation
5. **Analyze**: Click "Analyze CV-Job Match"
6. **Export Results**: Save as TXT, DOCX, or JSON

### Analysis Types

#### 📋 JD Requirements Analysis
- Technical skills breakdown
- Soft skills requirements
- Experience and qualifications
- Role responsibilities analysis
- Red flags and concerns identification

#### 🎯 CV Fit Assessment
- Technical skills matching
- Experience alignment scoring
- Soft skills evidence evaluation
- Overall compatibility percentage

#### 🔍 Skills Gap Identification
- Missing technical skills
- Experience shortfalls
- Recommended certifications
- Improvement suggestions

#### ✨ CV Optimization
- Keyword incorporation advice
- Section reorganization tips
- Achievement highlighting
- Interview preparation questions

#### 🏢 Corporate Jargon Translation
- Buzzword decoding
- Risk assessment (scope creep, burnout potential)
- Realistic expectation setting
- Interview clarification questions

## 🔒 Privacy & Security

- **100% Local Processing**: All analysis happens on your computer
- **No Data Transmission**: Nothing is sent to external servers
- **No API Keys**: No cloud services or external dependencies
- **Offline Capable**: Works without internet connection (after initial model download)

## 🛠️ Technical Details

### System Requirements
- **Operating System**: Windows, macOS, or Linux
- **RAM**: Minimum 8GB (16GB+ recommended for larger models)
- **Storage**: ~4-20GB for AI models (varies by model size)
- **Browser**: Modern browser with JavaScript enabled

### Supported Model Types
- **LLaMA**: All variants (7B, 13B, 70B)
- **Mistral**: 7B and larger
- **Code Llama**: For technical analysis
- **Custom Models**: Any model compatible with OpenAI API format

### File Structure
```
local_jd_cv_evaluator/
├── standalone_cv_jd_evaluator.html    # Main application file
├── README.md                          # This documentation
├── LICENSE                           # MIT license
├── CONTRIBUTING.md                   # Contribution guidelines
├── CHANGELOG.md                      # Version history
└── .github/                         # GitHub templates and workflows
    ├── ISSUE_TEMPLATE/
    └── workflows/
```

## 🚧 Troubleshooting

### Common Issues

**"LM Studio: Not Connected" Error**
- Ensure LM Studio is running
- Verify the local server is started
- Check the base URL (default: `http://localhost:1234`)
- Confirm a model is loaded in LM Studio

**"No Models Found" Message**
- Load a model in LM Studio first
- Click "Refresh Models" button
- Restart LM Studio if necessary

**Analysis Takes Too Long**
- Use smaller models for faster results
- Reduce input text length
- Check LM Studio performance settings

**Export Features Not Working**
- Ensure modern browser with JavaScript enabled
- Check popup blockers for download restrictions
- For DOCX export, verify html-docx-js library loads correctly

## 🤝 Contributing

We welcome contributions! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

### Development Setup
1. Fork this repository
2. Make your changes to `standalone_cv_jd_evaluator.html`
3. Test thoroughly with different models and inputs
4. Submit a pull request with detailed description

### Reporting Issues
Please use the [issue templates](.github/ISSUE_TEMPLATE/) when reporting bugs or requesting features.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **LM Studio**: For providing excellent local model inference
- **OpenAI**: For the standardized API format
- **FontAwesome**: For icons
- **Google Fonts**: For Inter font family
- **html-docx-js**: For DOCX export functionality

## 📞 Support

- **Issues**: [GitHub Issues](../../issues)
- **Discussions**: [GitHub Discussions](../../discussions)
- **Documentation**: This README and inline help text

## 🔄 Version History

See [CHANGELOG.md](CHANGELOG.md) for detailed version history.

## 🌟 Star History

If you find this tool useful, please consider starring the repository!

---

**Made with ❤️ for privacy-conscious professionals**
