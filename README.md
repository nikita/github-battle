# github-battle

### Battle between two GitHub users to see who is king

# Installing

1. Clone and install dependecies

```
git clone https://github.com/nikita/github-battle.git
cd github-battle
yarn
```

2. Setup GitHub client id and secret by going to https://github.com/settings/applications/new

- you can set `Application name` to anything you want
- `Homepage URL` can be either
  - https://github.com/nikita/github-battle
  - https://localhost:8080
- `Authorization callback URL`
  - http://localhost:8080/oauth (the url does not matter as we are not using the callback)

3. Rename `.env.example` to `.env` and fill in your client id and secret

```
CLIENT_ID=<YOUR_CLIENT_ID_HERE>
CLIENT_SECRET=<YOUR_CLIENT_SECRET_HERE>
NODE_ENV=production
```

4. You can start the website with

```
yarn start
```

The website should be available at http://localhost:8080 now, it hot reloads whenever you make changes.

5. You can build the website for development or production by specifying NODE_ENV in our .env file and running

```
yarn build
```

The build should now be in ./dist