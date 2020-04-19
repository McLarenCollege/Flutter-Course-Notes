**There are two ways to publish the react website.**

# 1. By pushing the build folder.

- in `package.json` file add 'homepage' property below 'version' property, and set it equal to 'https://yourUsername.github.io/react_web_repo'
```
homepage: "https://yourUsername.github.io/react_web_repo",
```
- Open project in webstorm and in terminal run `npm run build`. 
- This will create a build folder.
- Now open that build folder separately in `webstorm`
- Go to VCS and select `import into version control` -> `Share project on github`
- Add repository name and then it should push the code to Github
- Then go to your Github Repo, go to settings and scroll down to Github pages section.
- There under source select `master` branch.

After this step you should have a link which you can share.

Problem with this approach is after you do a build React deletes the old folder and creates new one so you will have to do these steps again everytime. And second time you can't use Share on Github option because a repo already exist. So you will have to add origin manually from VCS -> Git -> Remotes section.


# 2. By using `gh-pages` plugin

- Push the code to github repo, let's say repository is called 'react_web_repo'
- install [`gh-pages`](https://www.npmjs.com/package/gh-pages) plugin in your project

```npm i gh-pages --save'```

- in `package.json` file add 'homepage' property below 'version' property, and set it equal to 'https://yourUsername.github.io/react_web_repo'
```
homepage: "https://yourUsername.github.io/react_web_repo",
```
- now in the same file under 'scripts' where you can see `start` and `build commands add these `predeploy` and `deploy` commands

```
"eject": "react-scripts eject",
"predeploy": "npm run build",
"deploy": "gh-pages -d build"
```

so your package.json should look something like this:
```json
{
  "name": "movies_task",
  "version": "0.1.0",
  "private": true,
  "homepage": "https://mclarencollege.github.io/react_movies_website_task/", // added this
  "dependencies": {
    "@testing-library/jest-dom": "^4.2.4",
    "@testing-library/react": "^9.5.0",
    "@testing-library/user-event": "^7.2.1",
    "axios": "^0.19.2",
    "react": "^16.13.1",
    "react-dom": "^16.13.1",
    "react-router-dom": "^5.1.2",
    "react-scripts": "3.4.1"
  },
  "scripts": {
    "start": "react-scripts start",
    "build": "react-scripts build",
    "test": "react-scripts test",
    "eject": "react-scripts eject",
    "predeploy": "npm run build", // added this
    "deploy": "gh-pages -d build" // added this
  },
  "eslintConfig": {
    "extends": "react-app"
  },
  "browserslist": {
    "production": [
      ">0.2%",
      "not dead",
      "not op_mini all"
    ],
    "development": [
      "last 1 chrome version",
      "last 1 firefox version",
      "last 1 safari version"
    ]
  },
  "devDependencies": {
    "gh-pages": "^2.2.0"
  }
}
```

- After making these changes just run `npm run deploy` in terminal.
- then go to your Github Repo, go to settings and scroll down to Github pages section.
- There under source select `gh-pages` branch.

That's it! You should have a link now which you can showcase or submit.

