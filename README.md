# Creating hello-gh-pages project

1) on dev machine

create project folder and a "dist" folder in the project folder.
inside the dist folder, create an index.html.

in project folder init the project and install gh-pages
```
npm init -y
npm i gh-pages
```

edit package.json and add
"homepage": "https://magnusmossberg.github.io/hello-gh-pages",

and change the "test" script to

"deploy": "gh-pages -d dist"


2) on github

create the repo


3) on dev machine

in project folder 

create .gitignore and add node_modules

then run
```
git init
git add .
git commit -m "init"
git remote add origin git@github.com:magnusmossberg/hello-gh-pages.git
git push -u origin master
```

and run
```
npm run deploy
```

first time this will create a gh-pages branch on github containing the content of the dist folder

and it will be available at https://magnusmossberg.github.io/hello-gh-pages/

after that it will update the gh-pages branch on GitHub
