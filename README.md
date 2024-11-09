
# 🌐 Test Websites with Docker Compose

![Docker](https://img.shields.io/badge/Docker-%230db7ed.svg?&style=flat&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-%23009639.svg?&style=flat&logo=nginx&logoColor=white)

This repository provides a simple setup for running two Nginx-based web servers, each serving distinct HTML files with unique background colors and the Saudi Arabia flag. Perfect for testing load balancing setups and service differentiation.

## 📑 Table of Contents
- [🌐 Test Websites with Docker Compose](#-test-websites-with-docker-compose)
  - [📑 Table of Contents](#-table-of-contents)
  - [🚀 Getting Started](#-getting-started)
    - [🔧 Prerequisites](#-prerequisites)
    - [⚙️ Installation](#️-installation)
  - [▶️ Usage](#️-usage)
    - [Starting the Containers](#starting-the-containers)
    - [Stopping and Removing Containers](#stopping-and-removing-containers)
  - [📁 File Structure](#-file-structure)
  - [🤝 Contributing](#-contributing)
  - [📜 License](#-license)

## 🚀 Getting Started

These instructions will help you set up and run the web servers locally.

### 🔧 Prerequisites

Ensure you have:
- Docker
- Docker Compose

### ⚙️ Installation

1. **Clone** this repository to your local machine:
   ```bash
   git clone https://github.com/amrmarey/test-websites.git
   ```
2. Navigate into the project directory:
   ```bash
   cd test-websites
   ```

## ▶️ Usage

### Starting the Containers

To build and start the Nginx services, run:

```bash
docker-compose up -d
```

- **Server 1** will be available at [http://localhost:8081](http://localhost:8081)
- **Server 2** will be available at [http://localhost:8082](http://localhost:8082)

### Stopping and Removing Containers

To stop and remove the containers:

```bash
docker-compose down
```

## 📁 File Structure

```
test-websites/
├── docker-compose.yml      # Docker Compose file to set up services
├── server01/
│   ├── index.html        # HTML file for Server 1
│   └── flag.jpg            # Saudi Arabia flag image for Server 1
└── server02/
    ├── index.html        # HTML file for Server 2
    └── flag.jpg            # Saudi Arabia flag image for Server 2
```

## 🤝 Contributing

We welcome contributions! Please fork this repository, make your changes, and submit a pull request.

For any questions, contact the maintainer: [amr.marey@msn.com](mailto:amr.marey@msn.com).

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
