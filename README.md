# Nexora Documentation

Official multilingual documentation for Nexora, built with [Mintlify](https://www.mintlify.com/).

## Local preview

Requires Node.js 20.17 or newer and the Mintlify CLI.

```bash
npm install
npm run dev
```

The preview opens at `http://localhost:3000`.

## Quality checks

```bash
npm run validate
npm run check:links
npm run check:a11y
```

## Publishing

Connect this repository and the `main` branch in the Mintlify dashboard. After the Mintlify GitHub App is installed for `lipedevv/nexora-docs`, every push to `main` triggers a production deployment.

The site uses one `docs.json`, one navigation tree, and localized content for 26 languages. Mintlify's native selector supports 23 of them. Thai, Slovak, and Lithuanian remain available as global navigation links because Mintlify does not currently list their language codes as supported selector values.

## License

Nexora may be used for commercial and personal projects. Resale and redistribution are prohibited. The authoritative terms are in each localized `commercial-license.md` page.
