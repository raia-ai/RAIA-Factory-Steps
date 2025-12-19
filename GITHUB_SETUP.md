# GitHub Setup Guide for RAIA Factory GitBook

## Quick Setup Instructions

### Option 1: Upload to Existing GitHub Repository

1. **Extract the zip file** to your local machine
2. **Navigate to the directory**:
   ```bash
   cd raia-factory-gitbook
   ```
3. **Add your GitHub remote**:
   ```bash
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
   ```
4. **Push to GitHub**:
   ```bash
   git branch -M main
   git push -u origin main
   ```

### Option 2: Create New GitHub Repository

1. **Go to GitHub** and create a new repository (e.g., `raia-factory-docs`)
2. **Extract the zip file** to your local machine
3. **Navigate to the directory**:
   ```bash
   cd raia-factory-gitbook
   ```
4. **Add your GitHub remote**:
   ```bash
   git remote add origin https://github.com/YOUR_USERNAME/raia-factory-docs.git
   ```
5. **Push to GitHub**:
   ```bash
   git branch -M main
   git push -u origin main
   ```

## Connect to GitBook

### Step 1: Link GitHub Repository to GitBook

1. Go to [GitBook.com](https://www.gitbook.com) and sign in
2. Create a new space or select an existing one
3. Go to **Integrations** → **GitHub**
4. Click **Configure** and select your repository
5. Choose the branch (usually `main`)
6. Click **Import**

### Step 2: Configure GitBook Sync

GitBook will automatically detect:
- `README.md` as your introduction page
- `SUMMARY.md` for navigation structure
- `.gitbook.yaml` for configuration

### Step 3: Enable Two-Way Sync (Optional)

1. In GitBook settings, enable **GitHub Sync**
2. Choose sync direction:
   - **GitBook → GitHub**: Changes in GitBook push to GitHub
   - **GitHub → GitBook**: Changes in GitHub pull to GitBook
   - **Bidirectional**: Both directions (recommended)

## Directory Structure

```
raia-factory-gitbook/
├── README.md                    # Introduction page
├── SUMMARY.md                   # Navigation structure
├── .gitbook.yaml               # GitBook configuration
├── setup/                      # Phase 1: Setup
│   ├── Onboarding&OrgSetup.md
│   └── Access&Credentials.md
├── auth-data/                  # Phase 2: Auth & Data
│   ├── Auth&APIVerification.md
│   └── DocumentCollection&Conversion.md
├── development/                # Phase 3: Development
│   ├── ETLSetupTemplateWorkflow.md
│   ├── InternalAIAuditOfTraining.md
│   ├── CustomWorkflowDesign.md
│   └── AIAgentBuild.md
├── quality-assurance/          # Phase 4: QA
│   ├── InternalQA.md
│   ├── ClientAgentTesting.md
│   └── FullEndtoEndTesting.md
├── live-operations/            # Phase 5: Live Operations
│   ├── Launch&Handoff.md
│   ├── Monitoring.md
│   ├── LongTermHold.md
│   └── ProjectComplete.md
└── reference/                  # Reference Materials
    └── Overview.md
```

## Making Updates

### Update Content in GitHub

1. Edit files in your local repository or directly on GitHub
2. Commit and push changes:
   ```bash
   git add .
   git commit -m "Update documentation"
   git push
   ```
3. GitBook will automatically sync the changes

### Update Content in GitBook

1. Edit pages directly in GitBook's editor
2. Changes will automatically sync to GitHub (if bidirectional sync is enabled)

## Tips

- **Use descriptive commit messages** to track changes
- **Create branches** for major updates before merging to main
- **Enable branch protection** on main branch for production docs
- **Add collaborators** in GitHub to allow team editing
- **Use GitBook's version control** to track documentation versions

## Troubleshooting

### GitBook Not Syncing

1. Check GitHub integration is active in GitBook settings
2. Verify repository permissions (GitBook needs read/write access)
3. Check `.gitbook.yaml` is properly formatted

### Navigation Not Showing

1. Verify `SUMMARY.md` structure is correct
2. Check file paths match exactly (case-sensitive)
3. Ensure all referenced files exist

### Files Not Displaying

1. Check file encoding is UTF-8
2. Verify Markdown syntax is valid
3. Ensure file extensions are `.md`

## Support

For GitBook-specific issues, visit [GitBook Documentation](https://docs.gitbook.com)

For GitHub-specific issues, visit [GitHub Docs](https://docs.github.com)
