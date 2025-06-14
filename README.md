# Agentic CAPTCHA Solver

<div align="center">

🤖 **AI-Powered CAPTCHA Solving Extension** 🤖

</div>

## 🔓 Agentic CAPTCHA Solver

Agentic CAPTCHA Solver is an intelligent Chrome extension that automatically solves various types of CAPTCHAs using advanced AI technology. Built on a robust multi-agent architecture, it can handle text-based CAPTCHAs, image recognition challenges, and other verification systems.

## 🔥 Why Agentic CAPTCHA Solver?

Tired of manually solving CAPTCHAs that interrupt your browsing experience? **Agentic CAPTCHA Solver** delivers intelligent automation while keeping you in complete control:

- **100% Free** - No subscription fees or hidden costs. Just install and use your own API keys.
- **Privacy-Focused** - Everything runs in your local browser. Your data stays with you, never shared with any cloud service.
- **Flexible LLM Options** - Connect to your preferred LLM providers with the freedom to choose different models for different agents.
- **Fully Open Source** - Complete transparency in how CAPTCHAs are solved. No black boxes or hidden processes.

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
- **Planner & Validator**: Claude 3.7 Sonnet
  - Better reasoning and planning capabilities
  - More reliable CAPTCHA analysis
- **Navigator**: Claude 3.5 Haiku
  - Efficient for web navigation tasks
  - Good balance of performance and cost

### Cost-Effective Configuration
- **Planner & Validator**: Claude Haiku or GPT-4o
  - Reasonable performance at lower cost
  - May require more iterations for complex CAPTCHAs
- **Navigator**: Gemini 2.0 Flash or GPT-4o-mini
  - Lightweight and cost-efficient
  - Suitable for basic navigation tasks

### Local Models
- **Setup Options**:
  - Use Ollama or other custom OpenAI-compatible providers to run models locally
  - Zero API costs and complete privacy with no data leaving your machine

- **Recommended Models**:
  - **Qwen3 14B**
  - **Falcon3 10B**
  - **Qwen 2.5 Coder 14B**
  - **Mistral Small 24B**

## 💡 Supported CAPTCHA Types

The extension can handle various CAPTCHA challenges:

1. **Text-based CAPTCHAs**:
   - Distorted text recognition
   - Mathematical problems
   - Simple questions

2. **Image Recognition**:
   - Object identification
   - Pattern matching
   - Visual puzzles

3. **Interactive Challenges**:
   - Click-based verification
   - Drag and drop puzzles

## 🔒 Security & Privacy

- **Local Processing**: All CAPTCHA solving happens in your browser
- **No Data Collection**: We don't collect or store any personal information
- **API Key Security**: Your LLM API keys are stored locally and never transmitted to our servers
- **Open Source**: Full transparency with publicly available source code
