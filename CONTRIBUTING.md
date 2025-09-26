# Contributing to GitNAP

Welcome to the GitNAP project! This guide will help you understand how to contribute to the White Out Survival NAP management system.

## 🎯 Project Goals

GitNAP aims to provide transparent, efficient governance tools for White Out Survival alliance councils through:
- Standardized NAP documentation
- Transparent weighted voting systems
- Multi-state collaboration
- Historical record keeping

## 👥 Who Can Contribute

### Council Members (R4/R5)
- Create and vote on rule proposals
- Report violations and suggest penalties
- Update alliance information and contact details
- Propose new voting initiatives

### Alliance Leaders
- Suggest rule clarifications
- Report issues with documentation
- Request translations for their language
- Provide feedback on voting processes

### Technical Contributors
- Improve voting system functionality
- Enhance documentation templates
- Add new state support features
- Fix bugs and security issues

## 📋 Contribution Types

### 1. Rule Documentation Updates
**What:** Changes to NAP rules, event protocols, or violation penalties
**Process:**
1. Create an issue using the [rule change template](/.github/ISSUE_TEMPLATE/rule-change.md)
2. Discuss with council members in the issue comments
3. Create a pull request with the proposed changes
4. Initiate a formal vote if required by NAP rules
5. Merge after vote approval

### 2. New State Onboarding
**What:** Adding a new state to the GitNAP system
**Process:**
1. Copy the [state template](/templates/state-template/) to `states/{your-state-number}/`
2. Customize configuration files for your state's NAP structure
3. Add council member registry with proper voting weights
4. Create initial rule documentation
5. Submit pull request for review

### 3. Voting System Improvements
**What:** Enhancements to the custom voting platform
**Process:**
1. Create an issue describing the improvement
2. Discuss technical approach with maintainers
3. Implement changes following coding standards
4. Test with sample votes
5. Submit pull request with documentation

### 4. Translation Contributions
**What:** Adding support for new languages
**Process:**
1. Create language directory (e.g., `fr/`, `de/`, `pt/`)
2. Translate core documentation files
3. Maintain parallel structure with English version
4. Submit pull request with translation status

## 🔄 Workflow Process

### Branch Strategy
```
main → Production-ready rules and code
develop → Integration branch for multiple changes
feature/state-{number}-{description} → State-specific updates
feature/voting-{enhancement} → Voting system improvements
translation/{language} → Language-specific updates
hotfix/{critical-issue} → Emergency fixes
```

### Pull Request Requirements
1. **Clear Description**: Explain what changes and why
2. **Testing**: Verify changes work as expected
3. **Documentation**: Update relevant docs if needed
4. **Review**: Get approval from appropriate council members
5. **Compliance**: Follow NAP voting requirements for rule changes

## 📏 Templates and Standards

### Issue Templates
- **Rule Change**: For proposing NAP rule modifications
- **Violation Report**: For reporting rule violations
- **New State**: For onboarding new states
- **Bug Report**: For technical issues
- **Feature Request**: For new functionality

### Documentation Standards
- Use clear, concise language
- Include examples where helpful
- Maintain consistent formatting
- Add appropriate headers and navigation
- Include last updated dates

### Code Standards
- Comment complex logic clearly
- Follow consistent naming conventions
- Include error handling
- Write tests for new functionality
- Document API changes

## 🔒 Security Guidelines

### Sensitive Information
- **Never commit**: Player passwords, personal information, or private Discord tokens
- **Use player IDs only**: No real names unless explicitly consented
- **Sanitize logs**: Remove sensitive data from debug output
- **Review permissions**: Ensure proper access controls

### Voting Security
- **Verify voters**: Confirm council membership before vote participation
- **Audit trails**: Maintain complete voting history
- **Session management**: Use secure, temporary authentication
- **Data integrity**: Hash vote data to prevent tampering

## 🎯 State-Specific Contributions

### Your State Directory Structure
```
states/{your-state}/
├── README.md              # State overview
├── config.json            # Configuration
├── council/
│   ├── members.json       # Council registry
│   └── voting-history.md  # Vote records
├── rules/
│   ├── BiA/index.md       # Brothers in Arms rules
│   ├── SvS/index.md       # State vs State rules
│   ├── Fortress/index.md  # Fortress protocols
│   └── Violations/index.md # Violation system
└── voting/
    ├── active/            # Current votes
    ├── completed/         # Archived votes
    └── templates/         # Vote templates
```

### Required Files for New States
1. **config.json**: NAP configuration and voting rules
2. **council/members.json**: R4/R5 registry with vote weights
3. **rules/{event}/index.md**: Event-specific rule documentation
4. **README.md**: State overview and quick navigation

## 🚑 Emergency Procedures

### Critical Rule Violations
1. **Immediate Response**: Create hotfix branch
2. **Document Incident**: Use violation report template
3. **Emergency Vote**: Use expedited 24-hour voting if needed
4. **Update Rules**: Implement penalty or rule clarification
5. **Notify Stakeholders**: Discord announcements and GitHub notifications

### System Issues
1. **Create Issue**: Use bug report template with priority label
2. **Hotfix Branch**: For critical functionality
3. **Emergency Contacts**: Ping repository maintainers
4. **Rollback Plan**: Revert to last stable version if needed

## 💬 Communication Channels

- **GitHub Issues**: For formal proposals and bug reports
- **GitHub Discussions**: For general questions and coordination
- **Discord**: For real-time coordination (link your server)
- **Pull Request Comments**: For code and documentation review

## ❓ Questions and Support

If you need help:
1. Check existing [documentation](/docs/)
2. Search [GitHub issues](https://github.com/HelloDevSero/GitNAP/issues)
3. Start a [discussion](https://github.com/HelloDevSero/GitNAP/discussions)
4. Contact your state's council representatives

Thank you for contributing to GitNAP and helping create transparent, effective NAP governance!