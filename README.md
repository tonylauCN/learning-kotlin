


## learning-kotlin

```
hugo new site learning-kotlin
cd learning-kotlin

git init 

git submodule add https://github.com/alex-shpak/hugo-book themes/book

cp -R themes/book/exampleSite/content .
hugo server --minify --theme book

git remote add origin https://github.com/tonylauCN/learning-kotlin.git
git push -u origin master

echo "public" >> .gitignore
git checkout --orphan gh-pages
git reset --hard
git commit --allow-empty -m "Initializing gh-pages branch"
git push origin gh-pages
git checkout master

git pull origin master
git branch --set-upstream-to=origin/master master


```
