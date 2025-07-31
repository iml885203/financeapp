# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a personal finance application for asset allocation tracking. The application allows users to:
- Track assets across different time points
- Manage various asset types (cash, investments, debts)
- View analytics and charts of asset distribution
- Export data and generate reports
- Set financial alerts and customizations

The project includes comprehensive user stories in Chinese, detailing end-to-end scenarios with BDD-style acceptance criteria.

## Claude Code Spec Workflow

This project is configured with the Claude Code spec-driven development workflow. Key commands:

**Feature Development:**
- `/spec-create <feature-name>` - Create new feature specification
- `/spec-execute <task-id>` - Execute implementation tasks  
- `/spec-status` - Show development status
- `/spec-list` - List all specifications

**Bug Fixing:**
- `/bug-create <bug-name>` - Start bug fix workflow
- `/bug-analyze` - Analyze root cause
- `/bug-fix` - Implement fix
- `/bug-verify` - Verify fix works

**Workflow Process:**
1. Requirements Phase → Design Phase → Tasks Phase → Implementation
2. Each phase requires explicit user approval before proceeding
3. All phases follow templates in `.claude/templates/`
4. Sub-agents validate quality at each phase if available

## Project Architecture

**Core Asset Management:**
- Time-based snapshots: Each asset record belongs to a specific date/time point
- Batch operations: Users can add multiple assets for the same time point
- Asset categorization: Cash, Investment, Debt types with risk levels
- Template system: Reuse previous asset structures

**Key Features from User Stories:**
- Dashboard with asset overview and alerts
- Timeline view for historical asset tracking  
- Batch asset entry with chat-style quick input
- Responsive mobile design with offline support
- Data visualization with charts and trend analysis
- Export capabilities (Excel, PDF reports)
- Google OAuth authentication
- Financial alert system with customizable thresholds

**Data Structure:**
- Assets grouped by snapshot_id (time point)
- Support for custom categories and investment tags
- Risk level classification for investments
- Template storage for recurring asset structures

## Development Guidance

**Internationalization:** The user stories are in Traditional Chinese, indicating the target market. Consider i18n support for UI text.

**Mobile-First:** User stories emphasize mobile optimization with bottom navigation, touch-friendly forms, and responsive charts.

**Offline Support:** Application should cache data locally and sync when network is restored.

**Security:** Implement proper authentication, data encryption, and avoid logging sensitive financial information.

**User Experience:** Focus on batch operations, quick input methods, and clear visual feedback for financial data.