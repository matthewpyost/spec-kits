# Spec Kits Repository

This repository contains specification kits (spec-kits) for various projects within our organization. Each spec-kit provides structured specifications, requirements, and checklists to guide project development and ensure consistency across initiatives.

## Purpose

The Spec Kits Repository serves as:

- A centralized location for project specifications
- A standardized framework for defining project requirements
- A shared constitution that ensures consistency across all spec-kits
- A collaborative platform for teams to develop and refine specifications

## Repository Structure

```
spec-kits/
├── .specify/
│   └── memory/
│       └── constitution.md    # Shared constitution inherited by all spec-kits
├── specs/
│   └── [project-name]/       # Individual spec-kit directories
│       ├── README.md
│       ├── spec.md
│       └── checklists/
└── README.md                  # This file
```

> **Note:** Files and directories not listed above are part of the spec-kit utility infrastructure and should never be changed unless they are being updated by the repository owners.

## Contributing

We welcome contributions from all team members! There are two main ways to contribute depending on your role:

### For All Users: Creating a New Spec-Kit

To create a new specification kit for your project:

1. **Use the `/speckit.specify` command** as described in the [spec-kit repository documentation](https://github.com/github/spec-kit?tab=readme-ov-file#3-create-the-spec)

2. **Follow the standard structure** by ensuring your spec-kit includes:

   - `README.md` - Overview and introduction
   - `spec.md` - Detailed specifications
   - `checklists/` - Directory containing requirement checklists

3. **Inherit from the constitution** - Your spec-kit will automatically inherit guidelines from our shared constitution

4. **Submit a Pull Request** (see workflow below)

### For Engineering Leadership: Managing the Constitution

The constitution defines the shared principles and standards that all spec-kits inherit.

**To update the constitution:**

1. Navigate to `.specify/memory/constitution.md`

2. Make your proposed changes to the constitution document

3. Submit a Pull Request with a clear explanation of:

   - What changes you're making
   - Why these changes are necessary
   - How they will affect existing spec-kits

4. The changes will be reviewed by repository maintainers

### For Repository Owners: Updating Spec-Kit Infrastructure

The spec-kit utility infrastructure (scripts, templates, and configuration files) should be kept in sync with the official [spec-kit repository](https://github.com/github/spec-kit).

**To update the infrastructure:**

1. Switch to the **Update Spec-Kit Infrastructure** custom agent in GitHub Copilot Chat

2. Ask the agent: _"Update the spec-kit infrastructure to the latest version"_

3. The agent will:

   - Fetch the latest release from the official spec-kit repository
   - Download and extract the appropriate template
   - Update files in `.specify/scripts/`, `.specify/templates/`, and `.github/`
   - Add version headers to all updated files

4. Review the changes and commit them with a descriptive message

5. Submit a Pull Request for review

> **Important**: The `.specify/` directory contains utility infrastructure and should only be updated using this automated process, never manually.

## Pull Request Workflow

For any contribution (new spec-kit or constitution update):

1. **Create a new branch** for your changes

   ```bash
   git checkout -b feature/your-spec-kit-name
   # or
   git checkout -b update/constitution-description
   ```

2. **Make your changes** following the guidelines above

3. **Commit your changes** with clear, descriptive messages

   ```bash
   git add .
   git commit -m "Add spec-kit for [project-name]"
   # or
   git commit -m "Update constitution: [brief description]"
   ```

4. **Push to the repository**

   ```bash
   git push origin feature/your-spec-kit-name
   ```

5. **Create a Pull Request** through GitHub

   - Provide a clear title and description
   - Reference any related issues or discussions
   - Request review from repository maintainers

6. **Address review feedback** if any changes are requested

7. **Await approval and merge** from authorized reviewers

## Getting Help

- Review existing spec-kits in the `specs/` directory for examples
- Consult the [spec-kit documentation](https://github.com/github/spec-kit) for detailed guidance
- Reach out to the engineering leadership team with questions about the constitution
- Open an issue in this repository for general questions or suggestions

## Best Practices

- **Be specific**: Clearly define requirements and acceptance criteria
- **Stay consistent**: Follow the established structure and inherit from the constitution
- **Collaborate**: Engage with stakeholders and team members during spec development
- **Iterate**: Specifications can evolve; update them as projects progress
- **Document thoroughly**: Future teams will rely on your specifications

## Using Published Spec-Kits

Once spec-kits are published in this repository, they become discoverable and can be installed into target projects through the **Platform Engineering MCP Server**.

### Getting Started with the MCP Server

To access published spec-kits, you need to connect to the Platform Engineering MCP server. Follow the detailed instructions at:

**[Platform Engineering MCP Server Setup Guide](https://github.com/wegmans/platform-engineering-dashboard?tab=readme-ov-file#mcp-server)**

### Discovering Spec-Kits

Once connected to the MCP server, you can interact with available spec-kits through your AI agent:

**Option 1: List All Available Spec-Kits**

- Ask your AI agent: _"List all available spec-kits published by Wegmans"_
- This will show you all published spec-kits in the repository

**Option 2: Find a Specific Spec-Kit**

- Ask your AI agent: _"Find a Wegmans spec-kit for [specific purpose]"_
- For example: _"Find a Wegmans spec-kit for web application projects"_
- The agent will help you locate spec-kits that match your needs

### Installing Spec-Kits

After discovering a spec-kit that fits your project requirements, simply ask your AI agent to use the chosen spec-kit. The AI agent will:

1. Install the spec-kit to your target project
2. Provide further instructions on how to use the spec-kit effectively

For example: _"Use the [spec-kit-name] spec-kit for my project"_

## Contact

For questions or support, please contact the repository maintainers or open an issue.
