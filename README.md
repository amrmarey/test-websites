
# Test Websites with Docker Compose

This repository provides a simple setup for running two Nginx-based web servers, each serving distinct HTML files with unique background colors and the Saudi Arabia flag. This configuration is designed for testing load balancing and service differentiation.

## Table of Contents
- [Test Websites with Docker Compose](#test-websites-with-docker-compose)
  - [Table of Contents](#table-of-contents)
  - [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)
  - [Usage](#usage)
    - [Starting the Containers](#starting-the-containers)
    - [Stopping and Removing Containers](#stopping-and-removing-containers)
  - [File Structure](#file-structure)
  - [Contributing](#contributing)
  - [License](#license)

## Getting Started

Follow these instructions to set up and run the web servers locally.

### Prerequisites

- Docker
- Docker Compose

### Installation

1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/amrmarey/test-websites.git
   ```
2. Navigate into the project directory:
   ```bash
   cd test-websites
   ```

## Usage

### Starting the Containers

To build and run the two Nginx services, execute:

```bash
docker-compose up -d
```

- Server 1 will be available at [http://localhost:8081](http://localhost:8081)
- Server 2 will be available at [http://localhost:8082](http://localhost:8082)

### Stopping and Removing Containers

To stop and remove the running containers, execute:

```bash
docker-compose down -v
```

## File Structure

The repository is organized as follows:

```
test-websites/
├── docker-compose.yml      # Docker Compose file to set up two services
├── server1/
│   ├── server1.html        # HTML file for Server 1
│   └── flag.jpg            # Saudi Arabia flag image for Server 1
└── server2/
    ├── server2.html        # HTML file for Server 2
    └── flag.jpg            # Saudi Arabia flag image for Server 2
```

## Contributing

Contributions are welcome! To contribute, please fork the repository, make your changes, and submit a pull request.

For any questions, feel free to contact the maintainer: [amr.marey@msn.com](mailto:amr.marey@msn.com).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
