# CryptoDev Docker Environment

This repository provides a development container (`devcontainer`) designed specifically for cryptography-related work with Jupyter notebooks.

## Overview

The CryptoDev environment includes a pre-configured Docker setup that combines all the necessary tools and libraries for cryptographic research, algorithm implementation, and educational work.

## Features

- Jupyter Notebook/Lab environment
- Pre-installed cryptography libraries:
  - `cryptography`
  - `pycryptodome`
  - `pyOpenSSL`
  - `hashlib`
- Mathematical libraries:
  - `numpy`
  - `sympy`
  - `matplotlib`
- Development tools:
  - Git
  - Python 3
  - Common development utilities

## Usage

### With VS Code

1. Install the "Remote - Containers" extension in your code editor.
2. Clone this repository.
3. The `sample` folder provides a sample project using this image as a development container.
4. Open `sample` in your code editor.
5. When prompted, select "Reopen in Container."
6. Your code editor will initialize and start the container automatically.

### Manual Docker Usage

To build the image yourself:

1. Introduce required modifications to `Dockerfile`.
2. Build the image

```bash
docker build -t username/image_name .
```

3. Push the image to GitHub Container Registry (optional)

```bash
docker login ghcr.io
docker push ghcr.io/username/image_name
```

4. Update `sample/.devcontainer/devcontainer.json` to use your image.

## License

[GNU General Public License v3.0](LICENSE)

This license ensures that all modifications to the software remain open source, prohibiting the creation of closed-source derivatives.