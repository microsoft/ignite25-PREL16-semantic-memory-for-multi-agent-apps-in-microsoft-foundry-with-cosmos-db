# GitHub Workflows Configuration

This directory contains GitHub Actions workflows for automating repository management.

## add-to-project.yml

This workflow automatically adds new issues to the Ignite GitHub Project and applies appropriate labels based on issue content.

### Features

- **Automatic Project Addition**: New issues are automatically added to the configured GitHub Project
- **Smart Labeling**: Issues are automatically labeled based on their title and content using pattern matching
- **Ignite-Specific Labels**: Includes labels specific to the PREL16 session content (AI Foundry, semantic memory, multi-agent)

### Configuration Required

Before the workflow can run successfully, you need to configure:

#### 1. Repository Variables

In your repository settings (Settings > Security > Secrets and variables > Actions > Variables):

- **IGNITE_PROJECT_URL**: The full URL of your GitHub Project
  - Example: `https://github.com/orgs/microsoft/projects/123`
  - Format: `https://github.com/orgs/{org}/projects/{project_number}`

#### 2. Repository Secrets

In your repository settings (Settings > Security > Secrets and variables > Actions > Secrets):

- **ADD_TO_PROJECT_PAT**: Personal Access Token with the following scopes:
  - `repo` - Full control of private repositories
  - `project` - Read and write access to GitHub Projects
  
  To create a PAT:
  1. Go to GitHub Settings > Developer settings > Personal access tokens > Tokens (classic)
  2. Generate new token with the required scopes
  3. Add it as a repository secret

### Label Configuration

The workflow uses `.github/labeler.yml` to define automatic labeling rules. The current configuration includes:

- **General Labels**: bug, enhancement, documentation, question
- **Project-Specific Labels**: ai-foundry, semantic-memory, multi-agent, lab, ignite

You can customize the labeling rules by editing `.github/labeler.yml`. Each label section contains regular expressions that match against issue titles and content.

### Triggers

The workflow runs automatically when:
- New issues are opened

### Permissions

The workflow requires the following permissions:
- `issues: write` - To apply labels to issues
- `contents: read` - To read repository files
- `repository-projects: write` - To add issues to projects

## Troubleshooting

### Common Issues

1. **Project not found**: Verify the IGNITE_PROJECT_URL variable is set correctly
2. **Permission denied**: Ensure the ADD_TO_PROJECT_PAT has the correct scopes
3. **Labels not applied**: Check the labeler.yml configuration and issue content

### Testing

To test the workflow:
1. Create a test issue with keywords that match the labeling rules
2. Check that the issue is added to the project
3. Verify that appropriate labels are applied

### For More Information

- [GitHub Actions Documentation](https://docs.github.com/en/actions)
- [GitHub Projects Automation](https://docs.github.com/en/issues/planning-and-tracking-with-projects/automating-your-project)
- [Issue Labeler Action](https://github.com/github/issue-labeler)