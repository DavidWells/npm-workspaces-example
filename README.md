# NPM workspaces example

Must have `npm` version 7.

## Install

```bash
npm install
```

## Running scripts

Running a script named "dev" in all workspaces located under apps/backend:

```bash
npm run dev -w apps/backend
```

Running a script named "dev" in all workspaces:

```
npm run dev --ws
```

Running a script named "dev" in a package named `package-a`

```
npm run dev -w package-a
```

## Observations

`npm run build --ws` doesn't build packages in the correct order... For example `app` with dep `package-a` will build before `package-a`

## Alt approaches

- [pnpm-workspaces-example](https://github.com/DavidWells/pnpm-workspaces-example)
- [lerna-example](https://github.com/DavidWells/lerna-example)
