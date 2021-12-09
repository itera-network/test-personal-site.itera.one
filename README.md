# test-personal-site.itera.one

- Create repository
  - The name should same as domain name
- Build the static website to `dist/`
- Go to fleek website, to get the necessary infos
  - team id: ![team-id](./doc/team-id.png)
  - api key
- Initial once to get the config (`.fleek.json`) file

    ```bash
    npm install -g @fleekhq/fleek-cli

    # to generate .fleek.json
    FLEEK_API_KEY=xxx fleek site:init
    ```

- Add `.github/workflows/main.yml` into the repo
- Edit code base
- Push code base to github
- Check the action
- Check the website
