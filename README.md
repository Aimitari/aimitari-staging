# AImitari Website

This is the official website for AImitari, showcasing our innovative medical technology products including the A2FO Pump System, TeleCardia Cardiovascular Monitoring System, and FormeBuds Intelligent Earbuds.

## About AImitari

AImitari develops cutting-edge AI-powered medical devices and health technology solutions. Our products combine advanced artificial intelligence with medical expertise to improve patient care and outcomes.

## What technologies are used for this project?

This project is built with:

- **Vite** - A fast build tool that provides instant server start and lightning-fast hot module replacement during development
- **TypeScript** - Adds type safety to JavaScript, helping catch errors before runtime
- **React** - A JavaScript library for building the user interface with reusable components
- **shadcn-ui** - A collection of accessible, customizable UI components built on Radix UI
- **Tailwind CSS** - A utility-first CSS framework for rapidly styling the website with responsive design

## Understanding GitHub Pages

This website is hosted using GitHub Pages, a free static site hosting service provided by GitHub. Here's how it works:

- GitHub Pages serves static files (HTML, CSS, JavaScript, images) directly from your repository
- This project is configured to serve from the root of the `main` branch
- When you push changes to the `main` branch, GitHub Pages automatically updates the live website
- The `.nojekyll` file tells GitHub Pages not to process the site with Jekyll (GitHub's default static site generator)
- The `CNAME` file contains the custom domain configuration (if applicable)

## How to Work with This Website

### Prerequisites

Before you begin, make sure you have:
- **Node.js** (version 16 or higher) and **npm** installed - [Download here](https://nodejs.org/) or [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating)
- **Git** installed - [Download here](https://git-scm.com/downloads)
- A **GitHub account** with access to the repository

### Step 1: Clone the Repository

First, download the website code to your computer:

```sh
# Clone the repository
git clone https://github.com/Aimitari/aimitari-staging.git

# Navigate into the project folder
cd aimitari-staging
```

### Step 2: Install Dependencies

Install all the required packages:

```sh
npm install
```

This will download all the necessary libraries and tools needed to run the website.

### Step 3: Make Your Changes

Edit the website files using your preferred code editor (VS Code, Sublime Text, etc.). The main files you'll work with are:

- `src/` - Contains all the React components and page content
- `public/` - Contains static assets like images and PDFs
- `index.html` - The main HTML file

### Step 4: Test Locally

Before pushing changes, test the website on your computer:

```sh
npm run dev
```

This starts a local development server. Open your browser and go to `http://localhost:8080` to see your changes in real-time. Press `Ctrl+C` in the terminal to stop the server when done.

### Step 5: Build the Website

Once you're happy with your changes, build the production version:

```sh
npm run build
```

This creates optimized files in the `dist/` folder. Now copy these files to the root directory:

**On Windows:**
```sh
Copy-Item -Path dist\* -Destination . -Recurse -Force
```

**On Mac/Linux:**
```sh
cp -r dist/* .
```

### Step 6: Commit Your Changes

Save your changes to Git:

```sh
# Add all changed files
git add .

# Commit with a descriptive message
git commit -m "Describe what you changed"
```

### Step 7: Push to GitHub

Upload your changes to GitHub:

```sh
git push origin main
```

You may be prompted to authenticate with GitHub. Once pushed, GitHub Pages will automatically update the live website within a few minutes.

### Quick Reference Commands

```sh
# Pull latest changes from GitHub
git pull origin main

# Check what files have changed
git status

# View recent commits
git log --oneline -5

# Discard local changes (be careful!)
git reset --hard origin/main
```

## Alternative Editing Methods

**Edit directly in GitHub**

- Navigate to the desired file in the GitHub repository
- Click the "Edit" button (pencil icon) at the top right
- Make your changes and commit directly
- Note: You'll still need to build and deploy for changes to appear on the live site

**Use GitHub Codespaces**

- Navigate to the repository on GitHub
- Click the "Code" button (green button)
- Select the "Codespaces" tab
- Click "New codespace" to launch a cloud-based development environment
- Edit, build, and commit changes directly in your browser
