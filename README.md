"# GitHub" 


git checkout -b header
echo "<h1>Welcome to Website</h1>" > header.html
git add header.html
git commit -m "Added header"

git checkout main
git checkout -b footer
echo "<p>Copyright 2026</p>" > footer.html
git add footer.html
git commit -m "Added footer"

git checkout main
git merge header
git merge footer

git branch
git log --oneline --graph --all

git remote add origin <repository-url>
git push -u origin main
