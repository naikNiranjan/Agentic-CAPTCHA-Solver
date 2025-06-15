# Agentic CAPTCHA Solver

<div align="center">

🤖 **AI-Powered CAPTCHA Solving Extension** 🤖

</div>

## 🔓 Agentic CAPTCHA Solver

Agentic CAPTCHA Solver is an intelligent Chrome extension that automatically solves various types of CAPTCHAs using advanced AI technology. Built on a robust multi-agent architecture, it can handle text-based CAPTCHAs, image recognition challenges, and other verification systems.

## 🔥 Why Agentic CAPTCHA Solver?

Tired of manually solving CAPTCHAs that interrupt your browsing experience? **Agentic CAPTCHA Solver** delivers intelligent automation while keeping you in complete control:

- **Privacy-Focused** - Everything runs in your local browser. Your data stays with you, never shared with any cloud service.
- **Flexible LLM Options** - Connect to your preferred LLM providers with the freedom to choose different models for different agents.

> **Note:** We currently support OpenAI, Anthropic, Gemini, Ollama, Groq, Cerebras and custom OpenAI-Compatible providers.

## 📊 Key Features

- **Multi-agent System**: Specialized AI agents collaborate to solve complex CAPTCHA challenges
- **Interactive Side Panel**: Intuitive interface with real-time solving status updates
- **CAPTCHA Automation**: Seamlessly solve various CAPTCHA types across websites
- **Multiple LLM Support**: Connect your preferred LLM providers and assign different models to different agents
- **Privacy Protection**: All processing happens locally in your browser

## 🌐 Browser Support

**Officially Supported:**
- **Chrome** - Full support with all features
- **Edge** - Full support with all features

**Not Supported:**
- Firefox, Safari, and other Chromium variants (Opera, Arc, etc.)

> **Note**: While Agentic CAPTCHA Solver may function on other Chromium-based browsers, we recommend using Chrome or Edge for the best experience and guaranteed compatibility.

## 🚀 Quick Start

1. **Build from Source** (Required):
   * Follow the build instructions below to create the extension
   * Load the built extension into your browser

2. **Configure Agent Models**:
   * Click the extension icon in your toolbar to open the sidebar
   * Click the `Settings` icon (top right)
   * Add your LLM API keys
   * Choose which model to use for different agents (Navigator, Planner, Validator)

## 🛠️ Build from Source

1. **Prerequisites**:
   * [Node.js](https://nodejs.org/) (v22.12.0 or higher)
   * [pnpm](https://pnpm.io/installation) (v9.15.1 or higher)

2. **Clone the Repository**:
   ```bash
   git clone <your-repository-url>
   cd agentic-captcha-solver
   ```

3. **Install Dependencies**:
   ```bash
   pnpm install
   ```

4. **Build the Extension**:
   ```bash
   pnpm build
   ```

5. **Load the Extension**:
   * The built extension will be in the `dist` directory
   * Open `chrome://extensions/` in Chrome
   * Enable `Developer mode` (top right)
   * Click `Load unpacked` (top left)
   * Select the `dist` folder

6. **Development Mode** (optional):
   ```bash
   pnpm dev
   ```

## 🤖 Choosing Your Models

Agentic CAPTCHA Solver allows you to configure different LLM models for each agent to balance performance and cost. Here are recommended configurations:

### Better Performance
- **Planner & Validator**: 
  - Better reasoning and planning capabilities
  - More reliable CAPTCHA analysis
- **Navigator**: 
  - Efficient for web navigation tasks
  - Good balance of performance and cost

### Cost-Effective Configuration
- **Planner & Validator**: 
  - Reasonable performance at lower cost
  - May require more iterations for complex CAPTCHAs
- **Navigator**: 
  - Lightweight and cost-efficient
  - Suitable for basic navigation tasks

### Local Models
- **Setup Options**:
  - Use Ollama or other custom OpenAI-compatible providers to run models locally
  - Zero API costs and complete privacy with no data leaving your machine



## 🎯 Core Modules and Functional Flow

### 1. CAPTCHA Input Module
**Function**: Accepts CAPTCHA inputs from real-world applications or manually uploaded samples.

**Types Supported**:
- **Text-based CAPTCHAs**: Distorted alphanumeric images, mathematical problems, simple questions
- **Image-based CAPTCHAs**: Object identification (e.g., "click all bicycles"), pattern matching, visual puzzles
- **Audio-based CAPTCHAs**: Speech-to-text decoding, audio pattern recognition
- **Interactive CAPTCHAs**: Click-based verification, drag and drop puzzles, slider challenges

### 2. AI-Based Solver Engine
**Function**: Uses LLMs and specialized AI tools to attempt solving CAPTCHAs.

**Approach**:
- **OCR APIs and custom models** for text CAPTCHAs
- **Computer vision models** (CLIP, SAM, YOLO) for image CAPTCHAs
- **Speech-to-text models** (Whisper, Google Speech API) for audio CAPTCHAs
- **LLMs** for understanding CAPTCHA instructions and complex reasoning

### 3. Logging & Evaluation System
**Function**: Tracks each CAPTCHA solving attempt and records:
- Input type and complexity level
- Solved/failed status with detailed analysis
- Time taken and confidence metrics
- CAPTCHA characteristics (distortion, complexity, security features)
- **Outcome**: Transparent tracking of AI performance across CAPTCHA types

### 4. Security Analysis Engine
**Function**: Assesses CAPTCHA resilience using AI-solving results and security metrics.

**Analysis Metrics**:
- Success rate vs complexity correlation
- Time-to-break analysis and performance benchmarks
- False positive/negative behavior patterns
- Entropy and variation in challenge generation
- **AI Assist**: LLMs generate natural language analysis and risk commentary

### 5. Security Scoring System
**Function**: Assigns numeric security scores (0–100) based on:
- Resistance to AI solving attempts
- Variation and unpredictability in generation
- Multimodal complexity and security features
- **Method**: Weighted scoring using solving statistics and security heuristics

### 6. Recommendations Generator
**Function**: Automatically suggests CAPTCHA design improvements using LLM analysis.

**Examples**:
- "Use randomized word distortions with noise overlays"
- "Replace static audio with dynamically generated speech including accents"
- "Increase object diversity in image-based CAPTCHAs"
- "Implement partial object occlusion and ambiguous boundaries"

## 🔐 Real-World Application Testing & Ethics

**Scope**: Test publicly available CAPTCHAs in sandboxed environments or controlled research settings.

**Ethics**:
- Follow responsible disclosure guidelines for any vulnerabilities discovered
- Focus on academic security analysis and research, not exploitation
- Respect website terms of service and implement appropriate rate limiting
- Contribute findings to the security research community for CAPTCHA improvements

## 📊 Security Analysis Outputs

The extension generates comprehensive security analysis reports including:

- **Security scorecards** per CAPTCHA type with detailed metrics
- **PDF/CSV reports** summarizing analysis findings and recommendations
- **AI-generated design recommendations** for enhanced CAPTCHA security
- **Performance benchmarks** comparing AI solving effectiveness across CAPTCHA types
- **Vulnerability assessments** with specific improvement suggestions

## 🔒 Security & Privacy

- **Local Processing**: All CAPTCHA solving and analysis happens in your browser
- **No Data Collection**: We don't collect or store any personal information or CAPTCHA data
- **API Key Security**: Your LLM API keys are stored locally and never transmitted to our servers
- **Research Ethics**: Built-in safeguards ensure responsible security research practices
