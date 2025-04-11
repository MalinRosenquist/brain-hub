# Copy and upload a repository

## Copy a repository

- Copy the HTTPS link
- In VS Code, type >git clone and insert adress
- Remove the remote in terminal

## Remove remote

```bash
git remote remove origin
```

- Make sure remote has been removed

```bash
git remote -v
```

## Add new repository and upload

- Create repository on Github
- Add new remote to the new repositry in terminal

```bash
git remote add origin https://repolink.git
```

- Verify new remote in termminal

```bash
git remote -v
```

- Push changes to new repository

```bash
git push -u origin main
```

## Update and live

Make sure to install dependencies and change directory of project in config-file

Vite: vite.config.ts:

```javascript
export default defineConfig({
  base: "/new-subdirectory/",
});
```

Install the right dependencies according to README-instructions. Usually one of the following package manager:

- npm install (package-lock.json)
- pnpm install (pnmp-lock.yml)
- yarn install (yarn.lock)
