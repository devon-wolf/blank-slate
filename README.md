# blank-slate

## general react setup process
- `npx create-react-app app-name --template typescript`
- `cd app-name`
- `npx eslint --init` - follow prompts
- `npm i --save-dev --save-exact prettier`
- add `.prettierrc.json` to project root with options
- add `.prettierignore`, copy `.gitignore` contents over
- run `npm run start`
    - see there are issues with eslint dependencies, follow steps provided by error to fix
    - the issue here is generally that eslint shouldn't be listed in the `package.json` because it's already a dependency within `create-react-app`
- add extra typings to boilerplate files to make eslint happy
- run prettier: `npx prettier --write .`
