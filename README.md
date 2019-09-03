# Platform UI customisations

This repository presents examples of customisations that can be done to the [platform app UI](https://github.com/opentargets/platform-app)

## Customisation

To customise the platform app:

- Clone the [platform-app](https://github.com/opentargets/platform-app) repository.
- Create a directory somewhere outside the `platform-app` repository where the customisation files will be put.
- Add an environment variable called `$CUSTOMISATIONS_DIR` that points to the customisation directory created in the step above.
- Inside your customisation directory you can overwrite or add new files following the same directory structure as
  [`src/public`](https://github.com/opentargets/platform-app/tree/master/src/public).
- When developing new customisations, you can use the `yarn start:customise` script inside the `platform-app` repository to see your
  customisations reflected in the app while developing. When done developing customisations, run the `yarn reset` command.
- For production, you can produce a build containing the customisations by running the `yarn build:customise` script inside the `platform-app`
  repository. This will create a `build` directory containing static assets files (html, css, js) that you can deploy.

