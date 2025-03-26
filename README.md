# 2nd brain  obsidian template

This structure has been useful for me -and may be useful for you too.

Types of notes:
- contact
- meeting
- idea
- link
- project overview

## usage

Prerequisites: 

- git
- an installation of cruft `pip install cruft`
- an installation of pixi https://pixi.sh/latest/#installation `curl -fsSL https://pixi.sh/install.sh | bash`
- text editor of choice such as vscode
- obsidian


```bash
curl -fsSL https://pixi.sh/install.sh | bash
git clone https://github.com/geoHeil/second-brain-obsidian-template.git
cd second-brain-obsidian-template
pixi run tpl-init-cruft

# alternatively:
pip install cruft
cruft create https://github.com/geoHeil/second-brain-obsidian-template.git

cd <<your project name>>
git init
git add .
git commit -m "initial commit"
```

Then open the folder as a vault in obsidian.
