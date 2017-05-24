# Get Docker Compose

Why is Docker Compose not packaged for Linux? Why do we always have to Google the installation two-liner? This is easier to remember:

    docker run --rm japsu/get-docker-compose > /usr/local/bin/docker-compose
    chmod +x /usr/local/bin/docker-compose

The `japsu/get-docker-compose` container, when run, will output the full Docker Compose binary on stdout.

For version information, see `Dockerfile`. Only Linux on AMD64 supported as Docker Compose is bundled in Docker for Mac & Windows. If you're interested in maintaining this for ARM, please fork.
