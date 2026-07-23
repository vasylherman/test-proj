```powershell
irm https://claude.ai/install.ps1 | iex
[Environment]::SetEnvironmentVariable("Path", ([Environment]::GetEnvironmentVariable("Path","User") + ";C:\Users\air\.local\bin"), "User")

```

```prompt
install latest powershell git and gh cli on my system

Install Oh My Posh via winget and a Meslo Nerd Font. 
Create a PowerShell 7 profile that loads a custom Powerlevel10k-style Oh My Posh theme with a single-line prompt: 
left side shows user@host, path, and git status; right side shows a ✓/✗ exit-status segment and the time. 
Enable PSReadLine inline autosuggestions from history, and bind Up/Down arrows to prefix history search. 
Finally, set the PowerShell 7 profile in Windows Terminal to use the Meslo Nerd Font and the One Half Dark color scheme.
```

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