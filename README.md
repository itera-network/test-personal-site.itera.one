# test-personal-site.itera.one

## Initialize

Following those steps to create your own sites:

- Create your own repository
  - The name should same as domain name, otherwise you have to manually set the `name` of itera-network/actions-coudflare-dns@master in `./github/workflows/main.yml`
- Add some static files for your website to `dist/`
- Go to fleek website, to get the necessary infos
  - team id: ![team-id](./doc/team-id.png)
  - api key: goto fleek.co panel to generate your api key
- Initial once to get the config (`.fleek.json`) file

    ```bash
    npm install -g @fleekhq/fleek-cli

    # to generate .fleek.json
    FLEEK_API_KEY=xxx fleek site:init
    ```

- Add secrets for your github repository
  - FLEEK_API_KEY
  - CF_API_TOKEN
  - CF_ZONE_ID
- Add `.github/workflows/main.yml` into your repo
- Push code base to github
- Wait for the action done
- Check your website
