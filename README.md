
1) on dev machine

create project folder and a "dist" folder inside that
create a index.html file in the "dist" folder

in project folder run
```
npm init -y
npm i gh-pages
```

create .gitignore
and add node_modules

edit package.json and add
"homepage": "https://magnusmossberg.github.io/hello-gh-pages",

and change "test" script to

"deploy": "gh-pages -d dist"


2) on github

create the repo


3) on dev machine

in project folder run
```
git init
git add .
git commit -m "init"
git remote add origin git@github.com:magnusmossberg/hello-gh-pages.git
git push -u origin master
```
