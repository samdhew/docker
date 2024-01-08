# Dockerfile for Amazon Corretto 17 with Alpine

This Dockerfile sets up a lightweight containerized environment based on Amazon Corretto 17 and Alpine Linux. It installs specific versions of `curl` (8.3.0-r0) and `tzdata` (2023c-r0), sets the timezone to America/New_York, and displays the current date.

## Usage

### Build the Docker Image

```bash
docker build -t your-image-name .
```

### Run a Container

```bash
docker run -d your-image-name
```

## Dockerfile Details

### Amazon Corretto 17

The Dockerfile starts with the Amazon Corretto 17 Alpine image, providing a reliable Java runtime environment.

### Installing Dependencies

Specific versions of `curl` and `tzdata` are installed using the Alpine package manager (`apk`). You can alternatively choose to install the latest versions by uncommenting the corresponding line in the Dockerfile.

### Setting Timezone

The Dockerfile sets the timezone to America/New_York using the `ENV TZ` instruction.

### Displaying Current Date

The last command in the Dockerfile displays the current date using the `date` command.

### Customization

Feel free to modify this Dockerfile to suit your specific requirements. Adjust the timezone, include additional dependencies, or modify commands as needed.

### Build and Run

Build the Docker image and run a container to experience a minimal and functional Amazon Corretto 17 environment with Alpine Linux.

**Note:** Ensure you have Docker installed on your machine before building and running the container.

```bash
docker build -t your-image-name .
docker run -d your-image-name
```

Happy containerizing!
