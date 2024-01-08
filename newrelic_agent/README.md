# Dockerfile for Amazon Corretto 17 with Alpine

This Dockerfile sets up a lightweight containerized environment based on Amazon Corretto 17 and Alpine Linux. It installs `curl` to facilitate downloading external resources and then downloads the NewRelic APM (Application Performance Monitoring) agent for Java.

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

It installs `curl` using the Alpine package manager (`apk`), which is needed for downloading external resources.

### NewRelic APM for Java

The Dockerfile then uses `curl` to download the NewRelic APM agent for Java from the official source and extracts it.

### Customization

Feel free to modify this Dockerfile to suit your specific requirements. You may want to customize the NewRelic APM version or include additional configurations based on your application's needs.

### Build and Run

Build the Docker image and run a container to use Amazon Corretto 17 with Alpine Linux and the NewRelic APM agent for Java.

**Note:** Ensure you have Docker installed on your machine before building and running the container.

```bash
docker build -t your-image-name .
docker run -d your-image-name
```

Happy containerizing!
