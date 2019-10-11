This repository is for hosting `headless-gl` prebuilt binaries for Alpine Linux. This is useful if you are running builds that require `gl` in an Alpine Linux continuous integration environment. `gl` installs by either downloading prebuilt binaries or rebuilding using `node-gyp`. The exact command is `prebuild-install || node-gyp rebuild`. `prebuild-install` looks by default to the `https://github.com/stackgl/headless-gl/releases` page for the correct binaries, but non exist for Alpine Linux. I have created this repository to provide Alpine Linux prebuilt binaries for `gl` v4.4.0.

In order for `prebuild-install` to find the correct binary in this repository, you must add this line to your `.npmrc`

`gl_binary_host=https://github.com/jcallin/headless-gl-alpine-prebuilt/releases/download`

Read more about `prebuild-install`: https://www.npmjs.com/package/prebuild-install
Prebuilt binaries for OSX and Trusty Linux are available at the original `headless-gl` project page https://github.com/stackgl/headless-gl/releases
