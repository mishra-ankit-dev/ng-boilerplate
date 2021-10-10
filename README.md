<h1 align="center">RoboFi</h1>

<hr>

```
Types of pages

public: everybody can see them
private: only logged in users can see them
```

- General
  - home
  - not-found
- Auth
  - sign-in
  - sign-up
  - forgot-password
  - forgot-password-email-sent
  - password-reset
  - password-reset-succeeded
  - password-reset-failed
- Settings
  - account
  - appearance
  - billing
  - blocked-Users
  - notifications
  - security
  - security-log
- User
  - my-profile
  - overview
- Features
  - dashboard

## 🧱 Self-contained components

- footer
- header
- layout

```console
├───app
│   ├───@core
│   │   ├───directives
│   │   │   └───click-outside
│   │   ├───guards
│   │   ├───interceptors
│   │   ├───pipes
│   │   │   └───bytes
│   │   ├───services
│   │   │   ├───seo
│   │   │   └───theme
│   │   └───utils
│   ├───@shell
│   │   ├───ft
│   │   └───ui (layout components)
│   │       ├───footer
│   │       ├───header
│   │       ├───layout
│   │       └───not-found
│   ├───components (generic shared components)
│   └───pages
│       ├───auth
│       │   ├───pages
│       │   │   ├───forgot-password
│       │   │   ├───forgot-password-email-sent
│       │   │   ├───password-reset
│       │   │   ├───password-reset-failed
│       │   │   ├───password-reset-succeeded
│       │   │   ├───sign-in
│       │   │   └───sign-up
│       │   └───services
│       ├───dashboard
│       ├───home
│       ├───settings
│       │   └───pages
│       │       ├───account
│       │       ├───appearance
│       │       ├───billing
│       │       ├───blocked-users
│       │       ├───notifications
│       │       ├───security
│       │       └───security-log
│       └───user
│           └───pages
│               ├───my-profile
│               └───overview
├───assets
├───environments
└───theme
    ├───01-base
    ├───02-components
    └───03-utilities
```

## 🧙‍♂️ Commands

| Command       | Description                                                    | NPM                   | Yarn               | Background command                                          |
| ------------- | -------------------------------------------------------------- | --------------------- | ------------------ | ----------------------------------------------------------- |
| ng            | See available commands                                         | npm run ng            | yarn ng            | ng                                                          |
| start         | Run your app in development mode                               | npm start             | yarn start         | ng serve                                                    |
| build         | Build your app for production                                  | npm run build         | yarn build         | ng build                                                    |
| build:stats   | Build your app for production and generate a "stats.json" file | npm run build:stats   | yarn build:stats   | ng build --stats-json                                       |
| watch         | Run build when files change.                                   | npm run watch         | yarn watch         | ng build --watch --configuration development                |
| test:unit     | Run your unit tests                                            | npm run test          | yarn test          | ng test                                                     |
| test:e2e      | Run your e2e tests                                             | npm run e2e           | yarn e2e           | ng e2e                                                      |
| test:coverage | Run your unit tests & generates a coverage report              | npm run test:coverage | yarn test:coverage | ng test --coverage                                          |
| lint          | Use ESLint to lint your app                                    | npm run lint          | yarn lint          | ng lint                                                     |
| analyze       | Open webpack-bundle-analyzer                                   | npm run analyze       | yarn analyze       | webpack-bundle-analyzer dist/angular-boilerplate/stats.json |
