# wechatStep 🚶‍♂️✨

[中文说明 (Chinese README)](./README_CN.md)

## Project Introduction
wechatStep is a fun and automated tool powered by GitHub Actions for submitting WeChat steps daily. No local scripts or manual operation are required—just set it up and let the bot do the walking for you! 🏃‍♀️🤖

## How It Works
- ⏰ Uses GitHub Actions scheduled workflow (runs every day at 21:00 Beijing Time) to automatically submit steps to WeChat Sports.
- 🎲 Step count range is customizable and supports randomization for a more natural look.
- 🌐 Submits steps by calling a third-party API.

## Account & API Info
This project uses the public [Steps-API](https://github.com/ymyuuu/Steps-API) service. For account registration, API usage, and details, please refer to that project.

## Setup Instructions
1. 🍴 Fork this repository to your own GitHub account.
2. 🔐 Go to your repository's Settings > Secrets and variables > Actions, and configure the following:
   - Add to Secrets:
     - `STEP_ACCOUNTS`: Multiple accounts in the format `email1:password1;email2:password2` (use `:` to separate email and password, `;` to separate multiple accounts)
   - Add to Variables:
     - `API_URL`: The API endpoint for submitting steps (e.g., `https://steps.api.030101.xyz/api`)
     - `STEP_MIN`: Minimum daily steps (e.g., 8000)
     - `STEP_MAX`: Maximum daily steps (e.g., 12000)
3. 🚀 The workflow will run automatically every day. To trigger it manually, go to the Actions page, select the workflow, and click "Run workflow".

## Notes
- 📚 This project is for learning and communication purposes only. Do not use it for illegal activities.
- 🛡️ Keep your account information secure to avoid leaks.
- ⚠️ WeChat may restrict accounts for abnormal or frequent step submissions. Use responsibly and have fun!

## License
MIT 📝
