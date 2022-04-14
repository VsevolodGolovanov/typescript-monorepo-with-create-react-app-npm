# Typescript monorepo (npm workspaces + typescript project references)

Demoes how CRA based package can depend on another local package, including another CRA based package.

## Bootstrap:

- `npm install`

## When developing

Run global type checking with:

- `npm run tsc-watch-references`

keep this running, since it is responsible for emitting package code.

Then start the development process for the project your are working on e.g.

- `npm run company-app-start`
- `npm run company-components-start`

See the top-level `package.json` for further examples.

## Troubleshooting

In case you would end up in a corrupted state please run:

- `npm run tsc-build-references`
