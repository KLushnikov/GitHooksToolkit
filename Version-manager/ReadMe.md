# Automated Version Increment Script

A Git-integrated tool to automatically increment version numbers in .NET projects and solutions. It:
- Scans staged files for changes in project directories
- Increments `VersionPrefix` in `.csproj` files (patch version)
- Updates `SolutionVersion` in `Solution.props` if any projects were modified
- Skips manual version overrides in the same commit
- Handles projects with spaces in filenames