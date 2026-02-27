# Copy Engineer

A web-based tool that helps copywriters and marketers identify the desires, pain points, and obstacles of their Ideal Customer Profile (ICP) using the OpenAI GPT-4 API.

## Overview

Copy Engineer guides you through a three-step, AI-powered research process to build a rich picture of your target audience:

1. **Desires** — Discover the 20 top outcomes your audience wants to achieve.
2. **Pain Points** — Uncover the 20 biggest frustrations standing in their way.
3. **Obstacles / Objections** — Surface the 20 actions your audience most wants to avoid.

At each step you select the three items most relevant to your offer, and the tool carries those selections into the next prompt automatically.

## Features

- Guided multi-step prompt flow powered by GPT-4
- Clean, readable output formatted with numbered lists
- API key stored securely in `sessionStorage` for the duration of your browser session
- **Start Again** button to reset the entire session and begin a new research run
- Fully client-side — no backend or database required
- Responsive UI built with Tailwind CSS and Font Awesome icons

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Markup | HTML5 |
| Styling | [Tailwind CSS 2.2](https://tailwindcss.com/) |
| Icons | [Font Awesome 5](https://fontawesome.com/) |
| Font | [Ubuntu](https://fonts.google.com/specimen/Ubuntu) (Google Fonts) |
| AI | [OpenAI Chat Completions API](https://platform.openai.com/docs/api-reference/chat) (GPT-4) |

## Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Edge, Safari)
- An [OpenAI API key](https://platform.openai.com/account/api-keys) with access to the `gpt-4` model

### Running Locally

Clone the repository and open `index.html` directly in your browser — no build step or server required.

```bash
git clone https://github.com/buzz39/copy-engineer.git
cd copy-engineer
open index.html        # macOS
# or
start index.html       # Windows
# or
xdg-open index.html    # Linux
```

You can also serve it with any static file server, for example:

```bash
npx serve .
```

## Usage

1. Open `index.html` in your browser.
2. Enter your **OpenAI API Key** (stored only in `sessionStorage` — never sent anywhere except OpenAI).
3. Fill in the seven fields that describe your offer:
   | Field | Description |
   |-------|-------------|
   | **Niche** | The market or industry you are targeting |
   | **Target Audience** | Who your ideal customer is |
   | **Promised Result** | The outcome your product/service delivers |
   | **Timeframe for Result** | How quickly the result is achieved |
   | **Unique Method** | What makes your approach different |
   | **Proof** | Evidence that your method works (testimonials, data, etc.) |
   | **Story** | A short narrative that connects your audience to the result |
4. Click **Start Process**. GPT-4 will generate 20 desires relevant to your audience.
5. Enter three comma-separated numbers (e.g. `1,3,7`) to select the most relevant desires, then click **Continue**.
6. Repeat the selection step for pain points and obstacles/objections.
7. Use **Start Again** in the navigation bar to reset and run a new session.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## Author

Built by [@hi_gaganthakur](https://www.twitter.com/hi_gaganthakur).

## License

This project is open source. See the repository for details.
