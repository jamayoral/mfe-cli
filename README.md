## Requirements

Requires Node JS version `14.17.0+`. Using `nvm`:

```sh
nvm install 14.17.0
nvm use 14.17.0
```

## Running the app locally

```
npm i
node index.js
```

## Adding a new MFE

To generate a new remote (MFE) run the following command:

```
node index.js
```

This will run a MFE CLI Generator (node app located in the `./index.js` directory) that will generate a new remote (MFE) based on a set of 3 questions. Under the hood this MFE CLI Generator clones a [template repository](https://github.com/jamayoral/mfe-template) and renames the content of certain files to match the prompts.

After generating a new remote (MFE), make sure to update the port numbers, as follows:

- `package.json` on `line 8`
- `webpack.dev.js` on `line 19`

> If MFE of type `Shell`, make sure you also update the `remotes` object in the `federation.config.json` file

## Add CLI to the system and running standalone

```
npm link
generate-mfe
```
