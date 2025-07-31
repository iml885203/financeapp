# 資產配置 APP (Finance App)

A comprehensive personal finance application for tracking and managing asset allocation across different time periods.

## 🌟 Features

### Core Functionality
- **Time-based Asset Tracking**: Record and manage assets at specific time points
- **Batch Asset Entry**: Add multiple assets efficiently in a single session
- **Smart Templates**: Reuse previous asset structures for faster data entry
- **Chat-style Quick Input**: Natural language asset entry (e.g., "新增永豐投資美股 50000")

### Asset Management
- **Multiple Asset Types**: Cash, Investments, Debts with risk classifications
- **Custom Categories**: Create and manage personalized asset categories
- **Investment Tags**: Organize investments by type (台股, 美股, ETF, etc.)
- **Risk Analysis**: Automatic risk level assessment and warnings

### Analytics & Visualization
- **Asset Distribution**: Interactive pie charts showing allocation percentages
- **Trend Analysis**: Historical asset growth and performance tracking
- **Financial Alerts**: Customizable warnings for debt levels and risk exposure
- **Export Options**: Excel spreadsheets and PDF reports

### User Experience
- **Responsive Design**: Optimized for both desktop and mobile devices
- **Offline Support**: View data without internet connection
- **Google OAuth**: Secure authentication and data backup
- **Timeline View**: Easy navigation through historical records

## 📋 User Stories

Comprehensive user stories are documented in [user-stories.md](./user-stories.md), covering:

- 🏠 Dashboard and navigation
- 📅 Timeline management
- ➕ Asset addition workflows
- ✏️ Asset editing capabilities
- 📊 Data visualization and analysis
- ⚙️ Settings and personalization
- 🔐 Authentication and security
- 📱 Mobile optimization
- 🌐 Offline functionality

## 🚀 Development Workflow

This project uses the **Claude Code Spec Workflow** for structured development:

### Available Commands

**Feature Development:**
```bash
/spec-create <feature-name>    # Create new feature specification
/spec-execute <task-id>        # Execute implementation tasks
/spec-status                   # Show development status
/spec-list                     # List all specifications
```

**Bug Fixing:**
```bash
/bug-create <bug-name>         # Start bug fix workflow
/bug-analyze                   # Analyze root cause
/bug-fix                       # Implement fix
/bug-verify                    # Verify fix works
```

### Development Process

1. **Requirements Phase** → Define user needs and acceptance criteria
2. **Design Phase** → Architecture planning and component design
3. **Tasks Phase** → Break down into atomic implementation tasks
4. **Implementation** → Execute using generated task commands

Each phase requires explicit approval before proceeding to ensure quality and alignment.

## 🏗️ Project Structure

```
financeapp/
├── .claude/                    # Claude Code spec workflow configuration
│   ├── templates/             # Document templates for specs
│   ├── commands/              # Workflow command definitions
│   └── agents/                # Validation agents
├── user-stories.md            # Comprehensive BDD-style user stories
├── CLAUDE.md                  # Claude Code guidance document
└── README.md                  # This file
```

## 🎯 Key Design Principles

- **Mobile-First**: Responsive design optimized for touch interfaces
- **Batch Operations**: Efficient multi-asset management
- **Data Security**: Secure handling of sensitive financial information
- **User Experience**: Intuitive workflows with clear visual feedback
- **Internationalization**: Traditional Chinese UI with potential for expansion

## 🔧 Technology Stack

*Note: Technology stack will be determined during the design phase of feature development.*

## 📊 Data Model Concepts

- **Snapshots**: Time-based groupings of assets (snapshot_id)
- **Asset Types**: Cash, Investment, Debt categories
- **Risk Levels**: High, Medium, Low risk classifications
- **Templates**: Reusable asset structure patterns
- **Tags**: Flexible categorization system

## 🚦 Getting Started

1. **Planning Phase**: Review user stories and define your first feature
2. **Spec Creation**: Use `/spec-create <feature-name>` to begin structured development
3. **Implementation**: Follow the approved specifications and task breakdown

## 📈 Financial Features

### Alert System
- Credit card debt thresholds
- High-risk investment warnings
- Negative net worth alerts
- Custom financial targets

### Analysis Tools
- Asset allocation visualization
- Investment risk distribution
- Historical trend analysis
- Debt-to-asset ratios

### Export Capabilities
- Excel format with multiple worksheets
- PDF reports with charts and summaries
- Custom date range selections
- Automated backup options

## 🛡️ Security Considerations

- Secure authentication via Google OAuth
- No sensitive data in logs or commits
- Encrypted data storage
- Regular backup reminders
- Offline data protection

## 📱 Mobile Features

- Bottom navigation for easy thumb access
- Touch-optimized form inputs
- Swipe gestures for chart navigation
- Offline viewing capabilities
- Native mobile keyboard support

## 🤝 Contributing

This project follows a structured spec-driven development approach. To contribute:

1. Create feature specifications using the Claude Code workflow
2. Follow the established templates and validation processes
3. Ensure all phases are properly approved before implementation
4. Maintain consistency with existing user stories and design patterns

---

*This README will be updated as the project develops and more technical details are established during the implementation phases.*