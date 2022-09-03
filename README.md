# github-actions-on-gitpod
Self-hosted Github Actions runner in Gitpod
### why would need Self-hosted Github Actions runner inside Gitpod?
There's big advantage on that. Since Gitpod workspaces is more powerful than hosted Github Actions runner this would be useful for faster build
### Steps
1. Fork and clone this repo (or download .gitpod.yml and .gitpod.Dockerfile to your project directory)
2. Edit init.sh and replace `https://github.com/MiracleCherryPie/github-actions-on-gitpod` with your Github repository URL
3. Go to https://gitpod.io/variables and click New variable. Name it `GH_ACTIONS_TOKEN` and paste your Github Actions self-hosted runner Token to Value column (you can find it at Repository Settings > Actions > Runners > Add new runner > Choose Linux as runner image)
4. Edit .gitpod.yml and change `https://raw.githubusercontent.com/MiracleCherryPie/github-actions-on-gitpod/main/init.sh` with `https://raw.githubusercontent.com/<username>/<repo name>/main/init.sh`
5. Push your changes to your fork or your project repository
6. In gitpod create new project with your fork or your project repository and create new workspace
7. Wait for moment until the task done