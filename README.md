# PipeChecks

> **Real-Time AWS CodePipeline Status in GitHub**

[![GitHub](https://img.shields.io/badge/GitHub-Integration-blue?logo=github)](https://github.com/pipechecks-io)
[![AWS CodePipeline](https://img.shields.io/badge/AWS-CodePipeline-orange?logo=amazon-aws)](https://aws.amazon.com/codepipeline/)

---

## 🚀 What is PipeChecks?

**PipeChecks** is a SaaS platform that bridges the gap between AWS CodePipeline and GitHub, providing seamless, real-time visibility into your CI/CD pipeline status directly within your GitHub workflow. Never leave GitHub to check your pipeline status again!

### The Problem We Solve

Modern development teams use AWS CodePipeline for robust CI/CD orchestration, but checking pipeline status requires constant context-switching to the AWS Console. This disrupts developer flow and slows down feedback loops.

### Our Solution

PipeChecks automatically syncs your AWS CodePipeline execution status to GitHub Checks, giving your entire team instant visibility into build and deployment health—right where they're already working.

---

## ✨ Key Features

### 🔄 Real-Time Pipeline Monitoring
- Continuous monitoring of AWS CodePipeline executions
- Instant updates on pipeline stage progress, success, and failure events
- Complete execution history at your fingertips

### ✅ GitHub Checks Integration
- Pipeline statuses appear directly as GitHub Checks on commits and pull requests
- See code-to-deploy health from the GitHub UI
- Clear visual indicators for pipeline state: in progress, success, or failure

### 📊 Multi-Pipeline Support
- Track unlimited CodePipelines across multiple AWS accounts
- Stage-by-stage breakdowns for detailed insights
- View current and historical executions with logs for troubleshooting

### 🔔 Instant Alerts & Notifications
- Immediate feedback when pipelines fail, stall, or complete
- Reduce time-to-fix and maintain deployment velocity
- Stay informed without manual checking

### 🔒 Security & Privacy First
- Minimal-scope AWS permissions using IAM roles
- Never stores your code or sensitive artifacts
- Focuses solely on pipeline status and metadata
- SOC 2 compliant infrastructure

### 🎯 Zero Console Switching
- Access all pipeline information and history without opening AWS Console
- Developer-friendly interface integrated into your existing workflow
- Streamlined troubleshooting with embedded logs and failure reasons

---

## 🛠️ How It Works

### 1. **Connect Your Accounts**
Connect PipeChecks to your AWS account and GitHub repositories using secure OAuth and IAM roles. Setup takes just minutes with our guided onboarding.

### 2. **Configure Pipeline Monitoring**
Select which CodePipelines and branches to track. Customize notification rules for each environment—Development, Staging, and Production.

### 3. **Monitor & Ship with Confidence**
As your pipeline runs, GitHub Checks are automatically updated with real-time status. When issues arise, get instant notifications with detailed logs—all without leaving GitHub.

### Technical Architecture

```
GitHub Push → AWS CodePipeline Trigger → EventBridge/CloudWatch Events
                                               ↓
                                         PipeChecks Service
                                               ↓
                                    GitHub Checks API Update
                                               ↓
                                    Status Visible in GitHub UI
```

---

## 💡 Benefits

### For Developers
- **Faster Feedback Loops**: See pipeline results instantly on your PRs
- **Less Context Switching**: Stay in GitHub, your primary workspace
- **Quick Troubleshooting**: Access logs and error details directly in GitHub

### For Teams
- **Better Collaboration**: Everyone sees the same real-time pipeline status
- **Improved Visibility**: Track deployment progress across all environments
- **Accelerated Releases**: Catch and fix issues earlier in the development cycle

### For Organizations
- **Increased Velocity**: Ship features faster with streamlined CI/CD visibility
- **Higher Quality**: Surface broken builds, security issues, and failed deployments immediately
- **Reduced Costs**: Minimize time spent investigating pipeline issues

---

## 🚦 Getting Started

### Prerequisites
- AWS account with CodePipeline configured
- GitHub repository (public or private)
- Basic understanding of CI/CD workflows

### Quick Start

1. **Sign up** at [pipechecks.io](https://pipechecks.io)
2. **Connect your AWS account** using our secure IAM role
3. **Link your GitHub repositories** via OAuth
4. **Select pipelines to monitor** from your AWS account
5. **Configure notifications** for your team
6. **Start shipping** with real-time visibility!

### Installation Options

#### GitHub App (Recommended)
Install the PipeChecks GitHub App for the easiest setup with automatic webhook configuration.

#### Manual Integration
For advanced users who want more control, configure webhooks and API access manually using our detailed documentation.

---

## 🔗 Integrations

### Supported Platforms

- **AWS CodePipeline**: Full compatibility with multi-stage pipelines, custom actions, and event triggers
- **GitHub**: Works with GitHub.com and GitHub Enterprise
- **GitHub Checks API**: Native integration for status reporting
- **AWS EventBridge/CloudWatch Events**: Real-time pipeline event monitoring
- **AWS IAM**: Secure, scoped access to your CodePipeline data

### Notification Channels
- GitHub Checks and Status API
- Email notifications
- Slack integration
- Microsoft Teams webhooks
- Custom webhooks for advanced workflows

---

## 📖 Use Cases

### Pull Request Workflow
```
1. Developer opens PR with new feature
2. AWS CodePipeline triggers automatically
3. PipeChecks updates GitHub Check status in real-time
4. Team reviews code + sees pipeline status in one place
5. Merge with confidence when both code review and pipeline succeed
```

### Multi-Environment Deployments
Track deployments across Dev → Staging → Production with clear visibility into which version is deployed where, and the status of in-flight deployments.

### Team Dashboards
Aggregate view of all pipeline statuses across your organization, helping engineering managers and DevOps teams understand system health at a glance.

---

## ❓ Frequently Asked Questions

### Do you store my code or AWS credentials?
No. PipeChecks uses secure, minimal-scope IAM roles and GitHub OAuth tokens. We only access pipeline metadata and status information—never your source code or artifacts.

### Can I monitor multiple AWS accounts and GitHub organizations?
Yes! PipeChecks scales to handle large teams with multiple AWS accounts and GitHub organizations. Enterprise plans support unlimited accounts.

### What AWS permissions do you need?
PipeChecks requires read-only access to CodePipeline executions and stages. We provide a CloudFormation template that creates an IAM role with minimal required permissions.

### How do I troubleshoot failed pipelines?
Failed pipeline checks include links to detailed logs and error messages. You can also jump directly to the AWS Console view for that specific execution if needed.

### Is there a free trial?
Yes! We offer a 14-day free trial with full access to all features. No credit card required.

### What's your uptime SLA?
PipeChecks maintains 99.9% uptime SLA for all paid plans, with redundant infrastructure across multiple AWS regions.

---

## 🏢 Enterprise Features

- **SSO/SAML Integration**: Seamless authentication with your identity provider
- **Advanced Role-Based Access Control**: Granular permissions for teams and individuals
- **Audit Logs**: Complete visibility into who accessed what and when
- **Dedicated Support**: Priority support with dedicated Slack channel
- **Custom Integrations**: Work with our team to build custom workflows
- **On-Premise Deployment**: Available for highly regulated industries

---

## 🤝 Contributing

We welcome contributions! This repository contains:
- Community health files
- Issue and PR templates  
- GitHub Actions workflows
- Documentation

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines (coming soon).

---

## 📄 License

This repository contains organizational configuration files for the PipeChecks GitHub organization.

---

## 🔗 Links

- **Website**: [pipechecks.io](https://pipechecks.io)
- **Documentation**: [docs.pipechecks.io](https://docs.pipechecks.io)
- **Status Page**: [status.pipechecks.io](https://status.pipechecks.io)
- **Support**: [support@pipechecks.io](mailto:support@pipechecks.io)
- **Twitter**: [@pipechecks](https://twitter.com/pipechecks)

---

## 💬 Support

Need help? We're here for you!

- 📧 Email: [support@pipechecks.io](mailto:support@pipechecks.io)
- 💬 Community: [GitHub Discussions](https://github.com/orgs/pipechecks-io/discussions)
- 📚 Documentation: [docs.pipechecks.io](https://docs.pipechecks.io)
- 🐛 Report Issues: [GitHub Issues](https://github.com/pipechecks-io/.github/issues)

---

<div align="center">

**Made with ❤️ for developers who love GitHub and AWS**

**[Get Started Free](https://pipechecks.io)** • **[View Demo](https://pipechecks.io/demo)** • **[Read Docs](https://docs.pipechecks.io)**

</div>
