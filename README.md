# GBUAcademy

<!-- After connecting to Netlify, replace YOUR_BADGE_ID and YOUR_SITE_NAME with the values from your site's Settings → General → Status badge -->
[![Netlify Status](https://api.netlify.com/api/v1/badges/YOUR_BADGE_ID/deploy-status)](https://app.netlify.com/sites/YOUR_SITE_NAME/deploys)

GBUAcademy is an online learning platform providing high-quality educational resources and courses.

## 🚀 Live Site

The site is deployed on Netlify. Every push to `main` triggers an automatic production deployment, and every pull request generates a **Deploy Preview** so changes can be reviewed before merging.

## 📋 Table of Contents

- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Deployment](#deployment)
- [Netlify Deploy Previews](#netlify-deploy-previews)
- [Contributing](#contributing)

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or higher recommended)
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)

### Installation

```bash
# Clone the repository
git clone https://github.com/jeremyagnz/GBUAcademy.git

# Navigate into the project
cd GBUAcademy

# Install dependencies
npm install
```

### Running Locally

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## Project Structure

```
GBUAcademy/
├── public/          # Static assets
├── src/             # Source code
│   ├── components/  # Reusable UI components
│   ├── pages/       # Page components / routes
│   └── styles/      # Global styles
├── netlify.toml     # Netlify configuration
└── README.md        # Project documentation
```

## Deployment

This project is continuously deployed on **Netlify**.

| Branch / Event | Environment | URL |
|---|---|---|
| `main` | Production | `https://YOUR_SITE_NAME.netlify.app` *(replace after Netlify setup)* |
| Pull Request | Deploy Preview | Auto-generated unique URL |
| Feature Branch | Branch Deploy | `https://BRANCH--YOUR_SITE_NAME.netlify.app` *(replace after Netlify setup)* |

### How it works

1. Push a commit or open a pull request on GitHub.
2. Netlify detects the change and starts a build automatically.
3. For **pull requests**, a unique **Deploy Preview** URL is posted as a comment so reviewers can inspect the changes live before merging.
4. Once the PR is merged into `main`, the production site is updated automatically.

## Netlify Deploy Previews

Deploy Previews allow every pull request to have its own isolated preview environment. This means:

- **No manual staging deploys** — every PR gets a live URL automatically.
- **Safe testing** — changes are visible in a real environment without affecting production.
- **Team collaboration** — stakeholders can review changes via the preview URL before code is merged.

The preview URL follows this pattern:
```
https://deploy-preview-<PR_NUMBER>--<YOUR_SITE_NAME>.netlify.app
```
> Replace `<YOUR_SITE_NAME>` with the actual site name from **Netlify → Site settings → General → Site name**.

Netlify Bot will post the preview link directly in the pull request conversation.

Configuration for deploy previews is defined in [`netlify.toml`](./netlify.toml).

## Contributing

1. Fork the repository.
2. Create a feature branch: `git checkout -b feat/my-feature`.
3. Commit your changes: `git commit -m "feat: add my feature"`.
4. Push the branch: `git push origin feat/my-feature`.
5. Open a Pull Request — a Deploy Preview will be created automatically.

## License

This project is licensed under the [MIT License](LICENSE).
