# GitHub Actions Matrix Build Challenge

This repository demonstrates a GitHub Actions workflow with matrix builds and artifact management.

## Workflow Features

- **Matrix Strategy**: Builds across Node.js versions 14, 16, and 18
- **Parallel Execution**: All matrix jobs run in parallel
- **Artifact Upload**: Each job uploads unique artifacts with the prefix `build-9f3dd16-`
- **Step Identifier**: Contains the required `matrix-9f3dd16` step

## Contact

**Email**: your.email@example.com

## Artifacts

Each workflow run produces 3 artifacts:
- `build-9f3dd16-v14` - Build output for Node.js 14
- `build-9f3dd16-v16` - Build output for Node.js 16
- `build-9f3dd16-v18` - Build output for Node.js 18

Each artifact contains:
- `output.txt` - Build information and metadata
- `build-info.json` - Structured build information

## Running the Workflow

The workflow triggers on:
- Push to main/master branch
- Pull requests to main/master branch
- Manual workflow dispatch (Actions tab)
