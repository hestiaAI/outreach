# outreach
Management of relations between Hestia(Labs) and/or the collectives and external stakeholders: partners, the general public, journalists, funders, researchers...


## Outreach Landing Page

The outreach landing page generated from this repository is at https://hestiaai.github.io/outreach/

To update it, follow these steps

1. (first time only) Install mkdocs:
```
pip install mkdocs
```
2. (first time only) Clone this repository:
```
git clone git@github.com:hestiaAI/outreach.git
```
3. Fetch the latest code:
```
git fetch
git pull
```
4. Make whatever edits you need to make in `docs/index.md`. It is markdown with some embedded HTML. Styles are in `css/extra.css`. Images are loaded from `docs/img` and referenced as `./img/xxx.jpg`. Do not edit anything in the `site` directory.
5. To test changes locally, run `mkdocs serve` and load `http://127.0.0.1:8000/outreach/` in your browser. As long as the script is still running, any changes saved to the source .md file will be updated automatically in the browser.
6. When you are happy with locally testing your changes, you must build the mkdocs output. This writes HTML and other files to the `site` directory ready for deployment:
`mkdocs build`
7. After a successful build, commit all changes to the `main` branch on git as normal:
```
git status
git add <files you have changed>
git commit -m "<message about what you have changed>"
git push
```
8. Now you must deploy the generated files in the `site` directory to the `gh-pages` in order for them to be published via Github Pages at https://hestiaai.github.io/outreach:
```
git subtree push --prefix site origin gh-pages
```
10. Wait anything from a few seconds to a few minutes for to Google to pick up the changes on the watched `gh-pages` branch update the website. Then you can visit https://hestiaai.github.io/outreach/ and you should see your changes. You may need to do a hard reload (Ctrl+F5 or Cmd+R).

If further details on mkdocs is needed, see https://www.mkdocs.org/

