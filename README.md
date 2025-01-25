# Instagram Auto-Follow Bot

A Python script using the Instagrapi library to automatically follow users from a target account's followers list.

## Features

- Automated Instagram login with session management
- Two-factor authentication support
- Random delays between actions to avoid rate limiting
- Configurable daily follow limits
- Proxy support (optional)
- Detailed logging and follow session summaries

## Prerequisites

- Python 3.9+
- Required packages:
  - instagrapi
  - Pillow
  - python-dotenv

## Installation

1. Clone this repository
2. Install the required packages: pip install instagrapi Pillow python-dotenv


## Configuration

1. Create a `.env` file in the project root with the following variables:

- INSTAGRAM_USERNAME=your_username
- INSTAGRAM_PASSWORD=your_password
- TARGET_INSTAGRAM_USERNAME=target_account

2. (Optional) To use a proxy, uncomment and configure the proxy settings in the script.

## Usage

1. Run the Jupyter notebook `auto_follow.ipynb`
2. Enter your 2FA code when prompted
3. The script will:
   - Log in to your Instagram account
   - Fetch followers from the target account
   - Follow random users with delays between actions
   - Display a summary of the follow session

## Safety Features

- Random delays between actions (2-10 seconds)
- Session management to avoid frequent logins
- Error handling and logging
- Configurable daily follow limits to avoid Instagram restrictions

## Disclaimer

This tool is for educational purposes only. Using automated scripts with Instagram may violate their terms of service. Use at your own risk.

## License

[MIT License](LICENSE)
