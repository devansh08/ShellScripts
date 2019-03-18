# ShellScripts
My BASH scripts
---
# aes
## Automated Environment Setup
Setup your development enviroment i.e. start all editors/tools, run scripts in background etc. automatically.

Configuration via ```.aes.json``` file.

Sample configuration:
```
{
	"components": [
		{
			"editor": "code",
			"path": "/home/devansh/Projects/Proj1/"
		},
		{
			"editor": "subl",
			"path": "/home/devansh/Projects/Proj2/",
			"files": ["main.py", "temp.c"]
		}
	],
	"scripts": [
		{
			"path": "/home/devansh/Projects/Proj1/",
			"command": "urxvt -e npm start"
		},
		{
			"path": "/home/devansh/Projects/Proj2/",
			"command": "urxvt -e python3 server.py"
		}
	]
}
```
