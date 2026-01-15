---
description: Update spec-kit toolkit to the latest version from GitHub
agent: update-speckit-toolkit
tools: ["fetch", "githubRepo", "file_management", "terminal"]
---

# Update Spec-Kit Toolkit

This prompt will use the specialized "Update Spec-Kit Toolkit" agent to download and install the latest spec-kit toolkit from the official GitHub repository.

The agent will:

1. Fetch the latest release from https://github.com/github/spec-kit/releases
2. Download the `spec-kit-template-claude-ps-{version}.zip` asset
3. Extract and copy toolkit files to the correct locations
4. Add version headers to all updated files
5. Clean up temporary files and provide a summary

Please proceed with updating the spec-kit toolkit to the latest available version.
