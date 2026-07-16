```shell
gh repo create vasylherman/test-proj --public
gh repo clone vasylherman/test-proj
cd test-proj
open readme.md
touch README.md
open README.md
git add README.md
git commit -m "fix: JIRA-123 init readme"
git push origin main
git checkout -b JIRA-123-add-docs
echo test >> README.md
git add .
git commit -m "fix: JIRA-123 add test in readme"
gh pr create --base main --body "" --title "fix: JIRA-123 add test in readme"
gh pr merge --merge
git checkout main && git pull origin main
```