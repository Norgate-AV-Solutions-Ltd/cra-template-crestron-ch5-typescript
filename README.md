# cra-template-crestron-ch5-typescript

This is an unofficial third party TypeScript template for [Create React App](https://github.com/facebook/create-react-app) and [Crestron CH5](https://www.npmjs.com/package/@crestron/ch5-crcomlib)

The template is setup to work with Crestron CH5 out of the box so you can get up and running quickly. It also provides packages for page routing, styling using [CSS-in-JS](https://en.wikipedia.org/wiki/CSS-in-JS) (you can still use regular CSS or SCSS 😄), a wide variety of icons, mobile browser console, linting and more... 🚀 🚀 🚀

To use this template, add `--template @norgate-av/crestron-ch5-typescript` when creating a new app.

For example:

```sh
npx create-react-app my-app --template @norgate-av/crestron-ch5-typescript

# or

yarn create react-app my-app --template @norgate-av/crestron-ch5-typescript
```

## What does this template provide?

-   Crestron CH5 CrComLib
-   Crestron CH5 WebXPanel
-   Crestron CH5 CLI
-   [Typescript](https://www.typescriptlang.org/)
-   [React Router](https://reactrouterdotcom.fly.dev/)
-   [Styled Components](https://styled-components.com/)
-   [React Icons](https://react-icons.github.io/react-icons/)
-   [Eruda](https://eruda.liriliri.io/)
-   [ESLint](https://eslint.org/)
-   [Prettier](https://prettier.io/)
-   [Husky](https://typicode.github.io/husky/#/)
-   [Lint-Staged](https://github.com/okonet/lint-staged)
-   [Commitizen](https://commitizen-tools.github.io/commitizen/)
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
				"type": "web"
			}
		}
	}
}
```

For more information, please refer to:

-   [Getting Started](https://create-react-app.dev/docs/getting-started) – How to create a new app.
-   [User Guide](https://create-react-app.dev) – How to develop apps bootstrapped with Create React App.
-   [Crestron CH5 Documentation](https://sdkcon78221.crestron.com/sdk/Crestron_HTML5UI/Content/Topics/Home.htm)