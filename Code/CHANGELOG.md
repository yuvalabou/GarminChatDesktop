# Changelog - Garmin Chat Desktop

## [4.0.0] - 2025-02-10

### 🎉 Major Features
- **Multi-Provider AI Support**: Choose from 5 AI providers
  - xAI (Grok)
  - OpenAI (ChatGPT)
  - Azure OpenAI
  - Google Gemini
  - Anthropic (Claude)
- **Save Multiple API Keys**: Store credentials for all providers and switch anytime
- **Automatic Model Migration**: Deprecated models automatically updated to current versions

### ✨ Enhancements
- **Enhanced Settings Dialog**: 
  - Provider selection with radio buttons
  - Dynamic API key fields based on selected provider
  - Model dropdown per provider
  - Azure-specific configuration fields
  - Fixed dark mode hover text visibility
  - Consistent icon usage (gear icon)

- **Improved Error Handling**:
  - Provider-specific error messages
  - Rate limit guidance for each provider (especially Gemini)
  - Model deprecation detection with suggested replacements
  - API quota error messages with dashboard links
  - Helpful troubleshooting steps

- **Better User Experience**:
  - Provider switching without losing credentials
  - Clear indication of active provider
  - Help text with API key URLs
  - Scrollable settings for better organization

### 🔧 Technical Improvements
- **Unified AI Client** (`ai_client.py`):
  - Single interface for all providers
  - Native SDK support for Anthropic and Gemini
  - OpenAI-compatible interface for xAI, OpenAI, Azure
  - Centralized conversation history management
  - Provider-specific error handling

- **Configuration Management**:
  - Stores all provider credentials
  - Auto-migration for deprecated models
  - Backward compatible with v3.x configs

- **Build System**:
  - Updated PyInstaller spec with all AI provider dependencies
  - Version bumped to 4.0.0.0
  - Updated Inno Setup installer with multi-provider messaging

### 🐛 Bug Fixes
- Fixed Settings dialog icon (was showing feather, now shows gear)
- Fixed dark mode text visibility on radio button hover
- Fixed provider API keys being lost when switching providers
- Fixed Gemini model naming (removed deprecated experimental models)

### 📚 Documentation
- Updated Setup.bat with multi-provider information
- Updated build.bat with v4.0 messaging
- Enhanced installer post-install message
- Added comprehensive README for release

### 🔄 Migrations
Automatic migrations for deprecated models:
- `grok-beta` → `grok-3`
- `grok-2-1212` → `grok-3`
- `gemini-2.0-flash-exp` → `gemini-1.5-flash`
- `gemini-exp-1206` → `gemini-1.5-flash`
- `gemini-1.5-pro-latest` → `gemini-1.5-pro`

### 📦 Dependencies Added
- `anthropic>=0.18.0` - For Claude support
- `google-generativeai>=0.3.0` - For Gemini support

---

## [3.1.0] - 2025-01-XX

### Added
- 14 comprehensive health metrics
- Enhanced nutrition tracking with 3-tier fallback
- Improved date range detection
- Body Battery, stress, HRV, VO2 Max support

### Fixed
- 403 errors with display_name helper
- Syntax errors in health metrics
- Date range parsing for "last month" queries

---

## [3.0.0] - 2024-12-XX

### Added
- Desktop GUI application
- Dark mode support
- Auto-login functionality
- Professional Windows installer

### Changed
- Migrated from Gradio to Tkinter
- Improved UI/UX with modern design
- Enhanced credential management

---

## [2.0.0] - 2024-11-XX

### Added
- xAI (Grok) integration
- Gradio web interface
- Activity analysis features

---

## [1.0.0] - 2024-10-XX

### Added
- Initial release
- Basic Garmin Connect integration
- Simple chat interface
