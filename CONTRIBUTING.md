## Adding your changes

1. Clone this repo
2. Create a branch
3. Commit your proposed changes
4. Push the branch
5. Open a PR
6. Get a code review
7. Merge and enjoy!

## Developing

- `npm install -g powerbi-visuals-tools`
- Follow Steps on https://github.com/Microsoft/PowerBI-visuals/blob/master/tools/CertificateSetup.md to setup your PowerBI live visual
- `npm install`
- `npm run build-turf` to refresh the subset of turf.js used in the Mapbox Visual for Power BI from source
- Log into your PowerBI web UI and enable dev tools https://github.com/Microsoft/PowerBI-visuals/blob/master/tools/DebugVisualSetup.md
- `npm start`
- Add a custom visual using the PowerBI custom viz options, using a latitude and longitude variable.

### Developing under MacOS

Due to an open PowerBI [issue](https://github.com/Microsoft/PowerBI-visuals-tools/issues/157) the `npm start` might fail with `FSEvents.framework`.

To mitigate the issue for powerbi-visuals-tools version 1.10.0 may run
```
git apply VisualBuilder-1.10.0.patch
```

### Running the tests
Please consult the [README.md](test/README.md) in the `/test` folder for futher details.

### Building

`npm run package`
The packaged output `pbiviz` file will be in the `/dist` folder.  
