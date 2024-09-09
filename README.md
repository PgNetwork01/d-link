# D-link

`d-link` is a Python library designed to extract data from a Python script and push it to a GitHub Pages repository. This allows you to dynamically update content on your GitHub Pages site based on values from your Python code.

## Features

- Extract constants and other data from Python scripts.
- Push extracted data to a GitHub Pages repository.
- Easy setup and configuration.

## Installation

You can install the `d-link` library using pip:

```bash
pip install d-link
```

## Usage

### 1. Configure the Repository

First, configure the GitHub repository URL and authentication token:

```python
from d-link import DataToGitHub

# Initialize DataToGitHub with the path to your Python script
data_to_github = DataToGitHub(script_path="path/to/your/script.py")

# Configure the repository (run this once)
data_to_github.configure_repository()

# Optionally, display current settings
data_to_github.display_settings()
```

### 2. Push Data to GitHub

Once configured, you can push data from your Python script to GitHub Pages:

```python
from d-link import DataToGitHub

# Initialize DataToGitHub with the path to your Python script
data_to_github = DataToGitHub(script_path="path/to/your/script.py")

# Push data from the Python script to GitHub Pages
data_to_github.push_data()
```

## Configuration

The `configure_repository` method prompts you to enter:

- **GitHub Repository URL**: The URL of the GitHub repository where you want to push data.
- **GitHub Personal Access Token**: Used for authentication with GitHub.

Ensure that the GitHub Pages site is set up to display or use the data in `data.json`.

## Troubleshooting

- **Library Not Found**: Ensure the library is installed with `pip install d-link`. Verify installation with `pip show d-link`.
- **Path Issues**: Confirm that the file paths in your script are correct and accessible.
- **Authentication Errors**: Verify your GitHub personal access token and repository URL are accurate and have the necessary permissions.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any questions or issues, please open an issue on the [GitHub repository](https://github.com/PgNetwork01/d-link) or contact [Web Wizard](mailto:wert.ed00@gmail.com).
```
