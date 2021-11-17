# blank-slate

## general react setup process
This is the process used to set up this template; if you are using the template, you can probably just `npm i` and go on with your day.

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

## pruning out create-react-app

- clear out `App` of everything but a wrapper div, update test to check for basic rendering
- clear out unused styling in `App.css`
- update `index.css` to reflect basic sensible defaults
- remove `reportWebVitals` from `index` and `src`
- remove logos and references to logos
