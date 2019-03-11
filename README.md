# Interactive Tax Resources for Youth through LRNG & EAC

A pair of tools built by Columbia students (maintained by @mikewesthad) to get youth understand tax forms for employment. These were produced for [LRNG](https://www.lrng.org/)'s online learning playlists and the [Economic Awareness Council](https://www.econcouncil.org/). The two tools are in `sites/` and are almost exact copies:

`tax-forms` - Chicago-specific, summer employment resource
`tax-forms-year-round` - National, year-round resource

## Technical

The tools are simple HTML sites. Each folder is self-contained and can be hosted as is.

Hint: you can view the differences between `tax-forms` and `tax-forms-year-round` via:

```
git diff --no-index ./tax-forms ./tax-forms-year-round
```

### Running

```
npm install
npm run dev
```

### Deploying

You can copy the folders within `sites/` to a server for deploying, just make sure you are _not_ copy the whole repository folder (which includes .git and the readme).

Deploying to GitHub for testing:

```
npm run deploy:gh-pages
```

### Changelog

03/11/2019:

- Updated version of both games that separates out the flow for contractors and hourly employees, @mikewesthad

01/18/2019:

- Restructure so that each game is modular and does NOT depend on a `../globals` folder, @mikewesthad
- Remove unused clipboard dependency, @mikewesthad
