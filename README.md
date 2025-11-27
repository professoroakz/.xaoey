# .xaoey
all things xaoex + code

## Installation

### npm Install

```bash
npm install github:professoroakz/.xaoey
```

Or with a specific release tag:

```bash
npm install github:professoroakz/.xaoey#release-v1.3.3.7-xaoey-room-ins-enterprise
```

### Docker Install

Pull and run using Docker:

```bash
# Clone the repository
docker run -it --rm -v $(pwd):/app -w /app alpine/git clone https://github.com/professoroakz/.xaoey.git .xaoey

# Or download a specific release
docker run -it --rm -v $(pwd):/app -w /app alpine/git clone --branch release-v1.3.3.7-xaoey-room-ins-enterprise https://github.com/professoroakz/.xaoey.git .xaoey
```

Alternatively, to build a Docker image from this repository:

```dockerfile
# Dockerfile
FROM node:18-alpine
WORKDIR /app
RUN apk add --no-cache git
RUN git clone https://github.com/professoroakz/.xaoey.git .
```

Build and run:

```bash
docker build -t xaoey .
docker run -it xaoey
```
