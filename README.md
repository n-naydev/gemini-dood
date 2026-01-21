# Gemini Image

A Docker-based environment for running the Gemini CLI securely.

## Overview

This project provides a Dockerized setup for the Gemini CLI, ensuring a consistent environment and safe execution by mounting local directories and managing permissions.

## Prerequisites

- Docker
- Gemini API Key

## Usage

1. Build the image:
   ```bash
   docker build -t gemini-image .
   ```

2. Run the image using the provided helper script or directly via Docker:
   ```bash
   ./gemini.sh
   ```

## Files

- `Dockerfile`: Defines the Node.js environment with Docker CLI and Gemini CLI.
- `entrypoint.sh`: Handles user/group mapping and Docker socket permissions within the container.
- `gemini.sh`: A helper script to launch the Gemini CLI container.
