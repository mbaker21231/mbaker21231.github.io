WEBSITE UPDATE — Interactive Economics

What's new
- interactive-economics.html: new exercise landing page
- supply-demand.html: the original supply and demand exercise, preserved
- profit-maximization.html: new synchronized MC/AC/profit exercise
- docs/ counterparts: ready to publish on GitHub Pages
- _quarto.yml: tracks standalone HTML assets across future quarto render runs
- teaching.qmd and docs/teaching.html: updated teaching link description

HOW TO PUBLISH (using your existing cloned repo on your computer)
1. Open the terminal in your local repository. First run:
   git status
   git pull --ff-only origin main
   (If you have uncommitted changes, back them up or commit them before pulling.)
2. Extract this ZIP somewhere OUTSIDE your local repository. Copy its contents
   INTO your existing local repository folder, merging and replacing files.
   Do not replace the .git directory of your local clone.
3. If you have Quarto installed, run: quarto render
   Otherwise the included docs/ pages are ready to publish as supplied.
4. Check: git status ; git diff --stat
5. Commit and push:
   git add _quarto.yml teaching.qmd interactive-economics.html supply-demand.html profit-maximization.html docs/interactive-economics.html docs/supply-demand.html docs/profit-maximization.html docs/teaching.html WEBSITE_UPDATE_README.txt
   git commit -m "Add interactive economics lesson hub and profit maximization"
   git push origin main
6. Visit https://mbaker21231.github.io/interactive-economics.html

Note: Quarto may refresh additional rendered docs files; check git diff before
committing, especially if you run quarto render.
