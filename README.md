#How to deploy React App

1.npm install gh-pages --save-dev
2.Open package.json. At the top add a “homepage” property.
    "homepage": "http://{github-username}.github.io/{repo-name}",

3.In package.json, in “scripts” property, add a “predeploy” property and “deploy” property as shown below.
    "predeploy": "npm run build",
    "deploy": "gh-pages -d build"

4.Create a git repository in the app’s folder.
    git init

5.Add the GitHub repository as a “remote” in your local git repository.
     git remote add origin https://github.com/{username}/{repo-name}.git

6.Generate a production build of your app, and deploy it to GitHub Pages.
    npm run deploy

7.Commit your source code to the “master” branch and push it to use it later.

    a. git add .
    b. git commit -m "deployed"
    c. git push origin master


