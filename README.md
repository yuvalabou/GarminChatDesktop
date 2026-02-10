# Garmin Chat Desktop v4.0

**🎉 NEW: Multi-Provider AI Support! Choose from 5 AI providers!**

A standalone desktop application for querying your Garmin Connect data using natural language and AI.

[![Garmin Chat Desktop](https://github.com/rod-trent/GarminChatDesktop/raw/main/AppImages/DarkMode.jpg)](https://github.com/rod-trent/GarminChatDesktop/blob/main/AppImages/DarkMode.jpg)

---

## 🎯 What is Garmin Chat?

Garmin Chat transforms your fitness data from passive numbers into actionable insights through natural conversation. Instead of navigating through multiple screens in Garmin Connect, simply ask questions like "How did I sleep last night?" or "What was my last workout?" and get instant, AI-powered responses.

**New in v4.0:** Choose your preferred AI provider! Switch between xAI (Grok), OpenAI (ChatGPT), Azure OpenAI, Google Gemini, and Anthropic (Claude).

---

## 🆕 What's New in v4.0

### 🎉 Multi-Provider AI Support
**Choose from 5 AI providers:**
- **xAI (Grok)** - Fast, conversational AI
- **OpenAI (ChatGPT)** - Most popular, reliable
- **Azure OpenAI** - Enterprise-ready
- **Google Gemini** - Free tier available
- **Anthropic (Claude)** - Long context, high quality

### ✨ New Features
- ✅ **Save Multiple API Keys** - Store credentials for all providers
- ✅ **Switch Providers Anytime** - Change AI provider without losing settings
- ✅ **Automatic Model Migration** - Deprecated models updated automatically
- ✅ **Enhanced Error Messages** - Provider-specific guidance and troubleshooting
- ✅ **Rate Limit Guidance** - Smart handling of free tier limits
- ✅ **Better Dark Mode** - Fixed hover states in Settings dialog
- ✅ **Consistent Icons** - Proper gear icon everywhere

---

## ✨ Key Features

### **💬 Natural Language Interface**
- Ask questions in plain English about your fitness data
- Multi-line input field for complex queries
- Rich markdown formatting in responses
- Conversation history with timestamps
- Context-aware AI remembers previous conversations

### **🤖 Flexible AI Provider Selection**
- **5 providers to choose from** - Pick what works best for you
- **Cost flexibility** - Free tier (Gemini) to premium (Claude)
- **Easy switching** - Change providers in Settings without losing data
- **Smart fallbacks** - If one provider has issues, switch to another
- **Model selection** - Choose specific models per provider

### **🔐 Secure Credential Management**
- All API keys stored securely in the app
- Separate configuration for each provider
- Garmin credentials encrypted locally
- Show/hide toggles for sensitive information
- No .env files needed

### **🚀 Smart Auto-Connect**
- Optional auto-login on startup
- Persistent MFA token storage (authenticate once, works for ~30 days)
- Automatic token refresh when expired
- Graceful fallback to MFA when needed

### **🎨 Modern Fluent Design Interface**
- Windows 11-inspired Fluent Design aesthetic
- **🌙 Dark Mode** - Toggle between light and dark themes
- Provider indicator showing current AI
- Enhanced Settings dialog with provider selection
- Responsive layout with proper spacing

### **📊 Comprehensive Garmin Data Access**
- 14+ health metrics (Body Battery, stress, HRV, VO2 Max, etc.)
- Recent activities with detailed stats
- Sleep tracking and analysis
- Heart rate and training data
- Nutrition tracking
- All data types supported by Garmin Connect

---

## 🤖 AI Provider Comparison

| Provider | Best For | Free Tier | Paid Starting | Setup Difficulty |
|----------|----------|-----------|---------------|------------------|
| **xAI (Grok)** | Fast responses, casual use | No | ~$2/1M tokens | ⭐ Easy |
| **OpenAI (ChatGPT)** | Reliability, most tested | No | $0.15/1M tokens | ⭐ Easy |
| **Azure OpenAI** | Enterprise, compliance | No | Custom pricing | ⭐⭐ Moderate |
| **Google Gemini** | Budget-conscious, free tier | **Yes** | $0.15/1M tokens | ⭐⭐⭐⭐ Complex |
| **Anthropic (Claude)** | Long context, quality | No | $0.25/1M tokens | ⭐ Easy |

**Recommendation:**
- **New users**: Start with **OpenAI gpt-4o-mini** (cheap, reliable)
- **Free tier**: Try **Gemini** (but note rate limits)
- **Best quality**: Use **Anthropic Claude**
- **Enterprise**: Consider **Azure OpenAI**

---

## 📋 Requirements

- **Python 3.12 or 3.13** (recommended)
- **Tkinter** (usually included with Python)
- **An API key** from your chosen AI provider:
  - xAI: https://console.x.ai/
  - OpenAI: https://platform.openai.com/api-keys
  - Gemini: https://makersuite.google.com/app/apikey
  - Anthropic: https://console.anthropic.com/
  - Azure: https://portal.azure.com/
- **A Garmin Connect account** with MFA enabled

---

## 🚀 Quick Start (Windows)

### **First Time Setup:**

1. **Download Latest Release**
   - Go to [Releases](https://github.com/rod-trent/GarminChatDesktop/releases)
   - Download `GarminChatDesktop_Setup_v4.0.exe`
   - Run installer

   **OR download source code:**
   - Download `garmin-chat-v4.0-release.zip`
   - Extract to a folder

2. **Run Setup.bat**
   - Double-click `Setup.bat`
   - Installs all Python dependencies
   - Takes ~30 seconds

3. **Run Startup.bat**
   - Double-click `Startup.bat`
   - App opens and shows Settings dialog

4. **Configure Your AI Provider**
   - **Select a provider** (radio buttons)
   - **Enter API key** for your chosen provider
   - **Choose model** (dropdown)
   - **Enter Garmin credentials**
   - **Enable auto-login** (recommended)
   - Click **Save**

5. **Connect & Start Chatting**
   - Click "🔐 Connect to Garmin"
   - Enter MFA code if prompted
   - Start asking questions!

### **Every Time After:**
Just double-click **Startup.bat** - that's it!

---

## ⚙️ Settings & Configuration

### **AI Provider Settings:**

**Select Your Provider:**
- ⚪ xAI (Grok)
- ⚪ OpenAI (ChatGPT)
- ⚪ Azure OpenAI
- ⚪ Google Gemini
- ⚪ Anthropic (Claude)

**Enter API Key:**
- Get from provider's website (links in Settings)
- Keys are masked for security
- All keys are saved - switch providers anytime!

**Choose Model:**
- Each provider has multiple models
- Dropdown shows available options
- Current models auto-updated

**Azure-Specific:**
- Endpoint URL
- Deployment name
- API key

### **Garmin Connect Credentials:**
- Email and password
- Password masked with show/hide toggle
- Credentials encrypted locally

### **Application Preferences:**
- ☑ Auto-connect on startup
- 🌙 Dark mode toggle

### **Storage Locations:**
- **Settings**: `~/.garmin_chat/config.json`
- **Chat history**: `~/.garmin_chat/chat_history/`
- **Garmin tokens**: `~/.garmin_tokens/`

---

## 🎮 Using the App

### **Main Interface:**

**Header:**
- **AI Provider Badge** - Shows current provider (e.g., "xAI (Grok)")
- **🔍 Search** - Search saved chats
- **🌙 Dark Mode** - Toggle theme
- **⚙️ Settings** - Configure providers and credentials

**Controls:**
- **🔐 Connect** - Authenticate with Garmin
- **🔄 Refresh** - Sync latest data
- **🗑️ Reset** - Clear conversation
- **💾 Prompts** - Saved questions
- **📝 Save** - Save current chat
- **📂 History** - View past chats
- **📄 Export** - Export as PDF/Word/Text

**Example Questions:**
- "How many steps did I take today?"
- "What was my last workout?"
- "How did I sleep last night?"
- "What's my Body Battery status?"
- "Show me my recent activities"

---

## 🔄 Switching AI Providers

### **How to Switch:**
1. Open **⚙️ Settings**
2. Select a different **AI Provider** (radio button)
3. API key for that provider auto-loads (if saved)
4. **Choose model** from dropdown
5. Click **Save**

The app instantly switches to the new provider - conversation resets but Garmin data remains connected.

### **Why Switch?**
- **Provider down** - Use backup provider
- **Rate limited** - Switch to different provider temporarily
- **Cost** - Use cheaper provider for simple queries
- **Quality** - Use premium provider for complex analysis

---

## 🐛 Troubleshooting

### **Provider-Specific Issues:**

**Gemini Rate Limits:**
- Free tier: 15 requests/minute
- Solution: Wait 60 seconds or switch to another provider
- Or upgrade: https://console.cloud.google.com/

**OpenAI Quota Exceeded:**
- Add credits: https://platform.openai.com/account/billing
- Or switch to Gemini (free tier)

**Model Deprecated:**
- App auto-migrates to current models
- Check Settings → Choose updated model
- Save and retry

**xAI/Anthropic/Azure:**
- Check API key is valid
- Verify billing is set up
- Review provider dashboard

### **General Issues:**

**"Python is not installed"**
- Install Python 3.12+ from python.org
- Check "Add Python to PATH"

**"Configuration Required"**
- Open Settings
- Select AI provider
- Enter API key and Garmin credentials
- Save

**MFA Code Errors:**
- Enter 6-digit code within 30 seconds
- If CSRF error: Wait and retry
- Tokens valid for ~30 days

---

## 📦 Building from Source

### **Create Executable:**

```bash
# Install PyInstaller
pip install pyinstaller

# Build
pyinstaller --clean --noconfirm GarminChatDesktop.spec
```

**Result:** `dist\GarminChat.exe`

### **Create Installer:**

1. Install [Inno Setup](https://jrsoftware.org/isinfo.php)
2. Open `installer.iss` in Inno Setup Compiler
3. Click Build → Compile
4. Installer created: `installer\GarminChatDesktop_Setup_v4.0.exe`

See `BUILD-INSTRUCTIONS.md` in the release package for detailed steps.

---

## 🆚 Advantages Over Other Solutions

| Feature | Web Version | Desktop v3.x | **Desktop v4.0** |
|---------|-------------|--------------|------------------|
| Browser needed | ✅ Yes | ❌ No | ❌ No |
| AI Provider choice | ❌ No | ❌ No | ✅ **5 providers** |
| Switch providers | ❌ No | ❌ No | ✅ **Instant** |
| Provider fallback | ❌ No | ❌ No | ✅ **Yes** |
| Free AI option | ❌ No | ❌ No | ✅ **Gemini** |
| Auto model migration | ❌ No | ❌ No | ✅ **Yes** |
| Rate limit guidance | ❌ No | ❌ No | ✅ **Yes** |
| Dark mode | ❌ No | ✅ Yes | ✅ Yes |
| Chat history | ❌ No | ✅ Yes | ✅ Yes |
| Export reports | ❌ No | ✅ Yes | ✅ Yes |

---

## 📝 Version History

### **v4.0.0 (February 2025) - CURRENT**
🎉 **Multi-Provider AI Support**
- 5 AI providers to choose from
- Save multiple API keys
- Switch providers anytime
- Automatic model migration
- Enhanced error handling
- Provider-specific guidance
- Dark mode improvements

### **v3.1.0 (January 2025)**
- 14 health metrics
- Enhanced nutrition tracking
- Improved date range detection

### **v3.0.0 (December 2024)**
- Desktop GUI application
- Dark mode
- Chat history & search
- Export to PDF/Word/Text

---

## 🔒 Security & Privacy

- **Local storage only** - No cloud sync
- **Encrypted credentials** - Secure local storage
- **Multiple API keys** - All stored securely
- **No telemetry** - No usage tracking
- **No data sharing** - Your data stays private

---

## 📜 License

MIT License - See [LICENSE](LICENSE) file

---

## 🔗 Links

- **Latest Release**: [Releases](https://github.com/rod-trent/GarminChatDesktop/releases)
- **Source Code**: [Code](https://github.com/rod-trent/GarminChatDesktop/tree/main/Code)
- **Issues**: [Report Issues](https://github.com/rod-trent/GarminChatDesktop/issues)
- **FAQ**: [Frequently Asked Questions](FAQ.md)

---

## 🙏 Acknowledgments

- **Garmin Connect** - Fitness data platform
- **xAI, OpenAI, Anthropic, Google, Azure** - AI providers
- **garminconnect/garth** - Python libraries
- **Tkinter** - Python GUI framework

---

## 💡 Getting Help

1. Check [FAQ.md](FAQ.md)
2. Review this README
3. Check [Issues](https://github.com/rod-trent/GarminChatDesktop/issues)
4. Read `BUILD-INSTRUCTIONS.md` for build issues

---

**Ready to transform your fitness data into insights with your choice of AI?**

Download the latest release, pick your AI provider, and start chatting! 🏃‍♂️💪🤖

---

## ⭐ Star This Repo

If you find Garmin Chat Desktop useful, please consider starring the repository!
