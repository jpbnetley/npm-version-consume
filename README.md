# npm version consume
> consume package published on github

## Pre-requisites
setup a personal access token and save it to your home dir, as explained here: https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-npm-registry#authenticating-with-a-personal-access-token

## Order of events
> The expected behaviour
The [package's](https://github.com/jpbnetley/npm-version-release) pre-release version is installed and utilised in the dev branch.  
As this project prepares for a release, the [package's](https://github.com/jpbnetley/npm-version-release) production release should be done first.  
Once the release has been completed, this project's production release can commence.

The production build will install the latest production version of the [package](https://github.com/jpbnetley/npm-version-release).
Once the build completes, a pull request is made to merge the changes down to dev (the updated dependencies that now utilizes the production version)

### Ref
This project consumes the package: https://github.com/jpbnetley/npm-version-release
