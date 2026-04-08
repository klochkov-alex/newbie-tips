# Tips for newbie in git

Config:
```bash
git config --global user.name 'name'
git config --global user.email 'email'
```

Hot to use git:
- `cd ~`
- `mkdir local-repo`
- `cd local-repo`
- `git init`
- `echo '# My first repo! <br> There is nothing interesting.' > README.md`
- `git status`
- `git add README.md`
- `git status`
- `git commit -m 'My first commit.'`

Local repo is done. Now push it to GitHub:
- `ssh-keygen -t ed25519 -C '<your github email here>' -f <path to your future key>`
- `ssh-add <path to your key>`
- `ssh -T git@github.com -i <path to your key>`
- `git remote add origin git@github.com:<acc name>/<repo name>.git`
- `git push -u origin main #-u stands for --set-upstream` 

Полезная информация:
1. HEAD — это ссылка на последний коммит;
2. Логи коммитов можно посмотреть через git log (--online);
3. Сообщения к комитам должны быть краткими, но информативными;
4. Подробнее о сообщениях к комитам можно почитать тут: https://www.conventionalcommits.org/ru/v1.0.0-beta.4/#спецификация
5.