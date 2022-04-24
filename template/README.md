# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

**NOTE**

To use the Husky Git Hooks feature provided by this template you must manually run the following command within the project directory after the bootstrap completes.

```sh
npm run husky:install

# or

yarn husky:install
```

## Crestron CH5 Specific

`yarn build` will compile the code in src to the build directory.  
`yarn build:archive` will build a ch5z file from the most recently built build and output to the dist folder.

`yarn build:deploy:touchscreen` will deploy the ch5z from the dist folder to a touchscreen.  
`yarn build:onestep:touchscreen` will execute the build, archive and deploy steps in sequence.

`yarn build:deploy:web` will deploy the ch5z from the dist folder to a control system.  
`yarn build:onestep:web` will execute the build, archive and deploy steps in sequence.

To learn more about Crestron CH5, check out the [Crestron CH5 documentation](https://sdkcon78221.crestron.com/sdk/Crestron_HTML5UI/Content/Topics/Home.htm).

## What does this template provide?

-   [Crestron CH5 CrComLib](https://www.npmjs.com/package/@crestron/ch5-crcomlib)
-   [Crestron CH5 WebXPanel](https://www.npmjs.com/package/@crestron/ch5-webxpanel)
-   [Crestron CH5 CLI](https://www.npmjs.com/package/@crestron/ch5-utilities-cli)
-   [Crestron CH5 Helper](https://www.npmjs.com/package/@norgate-av/crestron-ch5-helper)
-   [Typescript](https://www.typescriptlang.org/)
-   [React Router](https://reactrouterdotcom.fly.dev/)
-   [Redux](https://redux.js.org/)
-   [React Redux](https://react-redux.js.org/)
-   [Redux Toolkit](https://redux-toolkit.js.org/)
-   [Styled Components](https://styled-components.com/)
-   [React Icons](https://react-icons.github.io/react-icons/)
-   [Rooks](https://react-hooks.org/)
-   [Eruda](https://eruda.liriliri.io/)
-   [Axios](https://axios-http.com/)
-   [ESLint](https://eslint.org/)
-   [Prettier](https://prettier.io/)
-   [Husky](https://typicode.github.io/husky/#/)
-   [Lint-Staged](https://github.com/okonet/lint-staged)
-   [Commitizen](https://commitizen-tools.github.io/commitizen/)
-   [commitlint](https://commitlint.js.org/#/)
-   [VSCode Workspace Config](https://code.visualstudio.com/docs/getstarted/settings#_workspace-settings)
-   [EditorConfig](https://editorconfig.org/)

## Project Setup

To upload to a Crestron touchscreen or control system, you must add the IP address or hostname to the project properties in `package.json`.

```json
{
    "crestron": {
        "project": {
            "touchscreen": {
                "url": "Enter IP/Hostname of Crestron Touchpanel here...",
                "type": "touchscreen"
            },
            "web": {
                "url": "Enter IP/Hostname of Crestron Processor here...",
                "type": "web",
                "config": {
                    "host": "localhost",
                    "ipId": "0x03",
                    "roomId": ""
                }
            }
        }
    }
}
```

## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `yarn test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `yarn eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

To learn Crestron CH5, check out the [Crestron CH5 documentation](https://sdkcon78221.crestron.com/sdk/Crestron_HTML5UI/Content/Topics/Home.htm).