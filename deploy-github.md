1 - Create git repository
```
create-react-app . --use-npm
```

2 - Add a package.json
```
"homepage": "https://youtube-courses.github.io/notes",

on 


{
  "homepage": "https://youtube-courses.github.io/notes",
  "name": "notes",
  "version": "0.1.0",
  ...
 }
```

3 - Add a package.json

```
"predeploy" : "npm run build",
"deploy" : "gh-pages -d build",

on

"scripts": {
    "predeploy" : "npm run build",
    "deploy" : "gh-pages -d build",
    "start": "react-scripts start",
    "build": "react-scripts build",
    "test": "react-scripts test",
    "eject": "react-scripts eject"
  },
```

4- Install
```
npm i gh-pages --save-dev
```

5- Run deploy
```
npm run deploy 
```

6- .gitignore
```
// .build
```

7- Git
```
git add .
git commit -m "sc"
git push


