# Backend Application Documentation

This document provides an overview of the backend application for the Azure Search OpenAI Demo.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The backend application is responsible for handling API requests, processing data, and interacting with Azure Search and OpenAI services. It is built using Python and Flask.

## Installation

To install the backend application, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/your-repo/azure-search-openai-demo.git
    ```
2. Navigate to the backend directory:
    ```bash
    cd azure-search-openai-demo/app/backend
    ```
3. Create a virtual environment:
    ```bash
    python -m venv venv
    ```
4. Activate the virtual environment:
    - On Windows:
        ```bash
        venv\Scripts\activate
        ```
    - On macOS/Linux:
        ```bash
        source venv/bin/activate
        ```
5. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Configuration

Before running the application, you need to configure the following environment variables:

- `AZURE_SEARCH_API_KEY`: Your Azure Search API key.
- `OPENAI_API_KEY`: Your OpenAI API key.
- `AZURE_SEARCH_SERVICE_NAME`: Your Azure Search service name.
- `AZURE_SEARCH_INDEX_NAME`: Your Azure Search index name.

You can set these variables in a `.env` file in the `app/backend` directory.

## Usage

To start the backend application, run the following command:

```bash
flask run
```

The application will be available at `http://localhost:5000`.

## API Endpoints

The backend application provides the following API endpoints:

- `GET /search`: Search the Azure Search index.
- `POST /query`: Query the OpenAI service.

## Contributing

We welcome contributions to the backend application. To contribute, follow these steps:

1. Fork the repository.
2. Create a new branch:
    ```bash
    git checkout -b feature-branch
    ```
3. Make your changes and commit them:
    ```bash
    git commit -m "Description of changes"
    ```
4. Push to the branch:
    ```bash
    git push origin feature-branch
    ```
5. Create a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.