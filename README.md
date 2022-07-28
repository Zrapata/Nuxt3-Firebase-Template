# Nuxt 3 Minimal Starter with Firebase support

Look at the [nuxt 3 documentation](https://v3.nuxtjs.org) to learn more.

## Setup

### Firebase

You can learn more in the [nitro firebase documentation](https://nitro.unjs.io/deploy/providers/firebase.html) and configure more for your needs.

Make sure to replace `""` with `"FIREBASE_PROJECT_ID"` in the following places

```json
firebase.json

{
	"hosting": {
		"site": ""
	}
}
```

```json
.firebaserc

{
  "projects": {
    "default": ""
  }
}
```

### Node
The default node version is `nodejs16` in case that your firebase project is using another node version, you have to change it in the following file

``` json
firebase.json

{
	"functions": {
		"runtime": "nodejs16"
	}
}
```

### Packages

Make sure to install the dependencies:

```bash
# yarn
yarn install

# npm
npm install

# pnpm
pnpm install --shamefully-hoist
```

## Development Server

Includes the firebase emulators, you can learn more at the [documentation](https://firebase.google.com/docs/emulator-suite)

Start the development server on http://localhost:3000

```bash
npm run dev
```

## Production

Build the application for production:

```bash
npm run build
```

Locally preview production build:

```bash
npm run preview
```

Checkout the [deployment documentation](https://v3.nuxtjs.org/guide/deploy/presets) for more information.

### Deploy

Deploy for firebase

``` bash
npm run deploy
```