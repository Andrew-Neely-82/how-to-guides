# How to Host a React App on GitHub Pages

<br>

## 1. Modify package.json

Add the following line to the package.json file:

```json
"homepage": "https://<github-username>.github.io/<repo-name>"

// make sure theres no <> in the actual value
```

Your package.json should look something like this now:

```json
{
  "name": "portfolio",
  "version": "0.1.0",
  "homepage": "https://<github-username>.github.io/<repo-name>",
  "private": true,
  "dependencies": {
    "@testing-library/jest-dom": "^5.16.5",
    "@testing-library/react": "^13.4.0",
    "@testing-library/user-event": "^13.5.0",
    "react": "^18.2.0",
    "react-dom": "^18.2.0",
    "react-scripts": "5.0.1",
    "sass": "^1.61.0",
    "web-vitals": "^2.1.4"
  },
```

<br>

## 2. Install gh-pages

```bash
npm i gh-pages --save-dev
```

<br>

## 3. Add build and deploy to scripts in package.json

Add the following line to the scripts in package.json:

```json
  "scripts": {
    "predeploy": "npm run build",
    "deploy": "gh-pages -d build",
    "start": "react-scripts start",
    "build": "react-scripts build",
    "test": "react-scripts test",
    "eject": "react-scripts eject"
  },
```

<br>

## 4. Deploy the site by running npm run deploy

run the build command in your terminal

```bash
npm run build
```

next run deploy

```bash
npm run deploy
```

<br>

## 5. Add your gh-pages branch to GitHub

Go to your GitHub repo and click on the settings tab. Scroll down to the GitHub Pages section and select the gh-pages branch as your source.

```bash
git remote add origin https://<github-username>.github.io/<repo-name>.git
```

<br>

## 6. Push your changes to GitHub

```bash
git add .
git commit -m "deploying react app to gh-pages"
git push origin main
```

<br>

## 7. Setup your pages to use the gh-pages branch

Go to your GitHub repo and click on the settings tab. Scroll down to the GitHub Pages section and click Pages. Under Build and deployment, select the gh-pages branch as your source. The next option should be root. Click save and your site should be live at the url provided.

<br>

## 8. Your site should be live at the url provided

The page may take a few minutes to load. If it doesn't load, try refreshing the page.
