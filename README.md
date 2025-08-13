# Public Containers 🐳

A curated collection of public Docker containers and container-related resources for various development and deployment scenarios.

## 📋 Overview

This repository serves as a centralized location for publicly available Docker containers, configurations, and related documentation. Whether you're looking for development environments, deployment templates, or specialized container setups, you'll find organized and well-documented solutions here.

## 🚀 Quick Start

### Prerequisites

- [Docker](https://docs.docker.com/get-docker/) installed on your system
- [Docker Compose](https://docs.docker.com/compose/install/) (optional, for multi-container setups)

### Basic Usage

```bash
# Clone the repository
git clone https://github.com/marcionicolau/public-containers.git
cd public-containers

# Navigate to a specific container directory
cd containers/<category>/<container-name>

# Build and run the container
docker build -t <container-name> .
docker run -d --name <container-name> <container-name>
```

## 📁 Repository Structure

```
public-containers/
├── README.md                    # This file
├── containers/                  # Container categories
│   ├── development/            # Development environment containers
│   ├── databases/              # Database containers (PostgreSQL, MySQL, etc.)
│   ├── web-servers/            # Web server containers (Nginx, Apache, etc.)
│   ├── tools/                  # Utility and tool containers
│   └── examples/               # Example and tutorial containers
├── docs/                       # Additional documentation
└── memory-bank/                # Project documentation and context
```

## 🏗️ Container Categories

### Development Environments
- **Purpose**: Ready-to-use development environments for various programming languages and frameworks
- **Examples**: Node.js, Python, Go, Java development containers

### Databases
- **Purpose**: Pre-configured database containers with optimized settings
- **Examples**: PostgreSQL, MySQL, MongoDB, Redis containers

### Web Servers
- **Purpose**: Production-ready web server configurations
- **Examples**: Nginx, Apache HTTP Server, Caddy containers

### Tools & Utilities
- **Purpose**: Containerized tools for development and operations
- **Examples**: CI/CD tools, monitoring solutions, backup utilities

### Examples & Tutorials
- **Purpose**: Educational containers demonstrating best practices
- **Examples**: Docker patterns, multi-stage builds, security examples

## 📖 Documentation Standards

Each container directory includes:

- **`README.md`** - Container-specific documentation with:
  - Purpose and use cases
  - Build and run instructions
  - Configuration options
  - Environment variables
  - Volume mappings
  - Network requirements
- **`Dockerfile`** - Container build instructions
- **`docker-compose.yml`** - Multi-service setups (when applicable)
- **`.env.example`** - Environment variable templates

## 🔧 Usage Examples

### Running a Development Container

```bash
# Navigate to a development container
cd containers/development/nodejs

# Build the container
docker build -t nodejs-dev .

# Run with volume mounting for live development
docker run -it --rm \
  -v $(pwd)/app:/workspace \
  -p 3000:3000 \
  nodejs-dev
```

### Using Docker Compose

```bash
# For multi-service setups
cd containers/examples/web-app-stack

# Start all services
docker-compose up -d

# View logs
docker-compose logs -f

# Stop services
docker-compose down
```

## 🛡️ Security Best Practices

All containers in this repository follow security best practices:

- ✅ No hardcoded secrets or credentials
- ✅ Minimal base images to reduce attack surface
- ✅ Non-root user execution where possible
- ✅ Regular security updates
- ✅ Clear documentation of security considerations

## 🤝 Contributing

We welcome contributions! Please follow these guidelines:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-container`)
3. **Follow** our documentation standards
4. **Test** your container thoroughly
5. **Commit** your changes (`git commit -m 'Add amazing container'`)
6. **Push** to the branch (`git push origin feature/amazing-container`)
7. **Open** a Pull Request

### Container Contribution Guidelines

- Follow the established directory structure
- Include comprehensive documentation
- Use official, minimal base images when possible
- Ensure cross-platform compatibility
- Add appropriate labels and metadata
- Test on multiple environments

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙋‍♂️ Support

- **Issues**: [GitHub Issues](https://github.com/marcionicolau/public-containers/issues)
- **Discussions**: [GitHub Discussions](https://github.com/marcionicolau/public-containers/discussions)
- **Documentation**: Check individual container README files

## 🌟 Acknowledgments

- Docker community for excellent documentation and best practices
- Contributors who help maintain and improve these containers
- Open source projects that inspire these configurations

---

**Happy Containerizing!** 🚀

*Last updated: August 2025*
