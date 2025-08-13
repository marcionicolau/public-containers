# Technical Context: Public Containers Repository

## Technologies Used
- **Version Control**: Git with GitHub hosting
- **Containerization**: Docker and Docker Compose
- **Documentation**: Markdown format
- **Repository Structure**: File-based organization

## Development Setup
- **Local Environment**: Linux-based development
- **Repository Location**: `/home/marcio/codes/personal/public-containers`
- **Remote Origin**: `https://github.com/marcionicolau/public-containers.git`
- **Branch**: `main` (currently no commits)

## Technical Constraints
- **Public Repository**: All content must be suitable for public access
- **Docker Compatibility**: Containers must work with standard Docker installations
- **Cross-Platform**: Containers should work on Linux, macOS, and Windows
- **Documentation Standards**: All documentation in Markdown format

## Dependencies
### Required
- Docker Engine
- Git

### Optional
- Docker Compose (for multi-container setups)
- Docker Desktop (for GUI management)

## Tool Usage Patterns
- **Container Building**: Standard `docker build` commands
- **Container Running**: `docker run` with appropriate flags
- **Multi-Service**: Docker Compose for complex setups
- **Documentation**: Markdown with code blocks for examples

## Development Workflow
1. Create container directory structure
2. Write Dockerfile with best practices
3. Create comprehensive documentation
4. Test container functionality
5. Commit and push to repository

## Quality Standards
- **Security**: No hardcoded secrets or credentials
- **Performance**: Optimized image sizes
- **Maintainability**: Clear, commented Dockerfiles
- **Documentation**: Complete usage instructions
