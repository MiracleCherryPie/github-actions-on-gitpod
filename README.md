# github-actions-on-gitpod
Self-hosted Github Actions runner in Gitpod (on ephemeral environment)
### why would need Self-hosted Github Actions runner inside Gitpod?
There's big advantage on that. Since Gitpod workspaces is more powerful than hosted Github Actions runner this would be useful for faster build
### Steps
1. Fork and clone this repo locally (or inside Gitpod)
2. Edit .gitpod.yml and replace `<Github Repository here>` with your Github repository URL
3. Go to https://gitpod.io/variables and click New variable. Name it `GH_ACTIONS_TOKEN` and paste your Github Actions self-hosted runner Token to Value column (you can find it at Repository Settings > Actions > Runners > Add new runner > Choose Linux as runner image)
4. Push your changes to your fork
5. In gitpod create new project with your fork and create new workspace
6. Wait for moment until the task done
