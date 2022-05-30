# Getting Started with Create React App

Push to github pages with React

1. Create a new public repo

2. Create a React app
```
npx create-react-app {project-name}
```

2B. Enter the folder:
```
cd {project-name}
```

3. Install the gh-pages npm package
```
npm i gh-pages
```

4. Add a "homepage" property to the "package.json" file under version
```
"homepage":"https://{username}.github.io/{repo-name}"
```

5. Add deployment scripts to the "package.json" file
```
"predeploy": "npm run build"
```

```
"deploy": "gh-pages -d build"
```

6. Add a remote repo

```
git init
```

```
git add *
```

```
git commit -m "first commit"
```

```
git branch -M main
```

```
git remote add origin https://github.com/{github-name}/{repo-name}.git
```

```
git push -u origin main
```

7. Deploy React app to Github Pages

```
npm run deploy
```

8. Push to repo
```
git add *
```

```
git commit -m "{commit-message}"
```

```
git push origin {branch-name}
```
