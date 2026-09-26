# Eamerald Console

A modern web console for [Eamerald](https://github.com/threehook/eamerald)

[![codecov](https://codecov.io/gh/threehook/eamerald-console/branch/main/graph/badge.svg?token=V6F5G43JXU)](https://codecov.io/gh/threehook/eamerald-console)
[![Tests](https://github.com/threehook/eamerald-console/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/threehook/eamerald-console/actions/workflows/tests.yml)
[<img src="https://img.shields.io/badge/slack-@asertocommunity-yellow.svg?logo=slack">](https://www.aserto.com/slack)


## 📋 Prerequisites

- Node.js (LTS version recommended)

## 🛠️ Installation

1. Clone the repository:
```bash
git clone git@github.com:threehook/eamerald-console.git
cd eamerald-console
```

2. Install dependencies:
```bash
yarn install
```
## ENV

Check the .env` file
```sh
VITE_REACT_APP_DISCOVERY_SERVICE_URL #eamerald console service gateway address
```
## 🚀 Development

To start the development server:

```bash
yarn dev
```

The application will be available at `http://localhost:3000`

## 📦 Build

To create a production build:

```bash
yarn build
```

The build output will be in the `dist` directory.

## 🧪 Available Scripts

- `yarn dev` - Start development server
- `yarn build` - Create production build
- `yarn preview` - Preview production build
- `yarn lint` - Run ESLint
- `yarn check` - TypeScript type checking
- `yarn generate:rest` - Generate REST API types
- `yarn detect-unused-exports` - Detect unused exports

## 🧪 Testing

The project uses [Vitest](https://vitest.dev/) for testing and [MSW (Mock Service Worker)](https://mswjs.io/) for API mocking.

### Running Tests

```bash
# Run tests in watch mode
yarn test

# Run tests once
yarn test:ci

# Run tests with coverage
yarn test:coverage
```

### Test Structure

- Tests are located alongside components in `*.test.tsx` files
- API mocks are generated using Orval and located in `src/api/*.msw.ts`
- Test utilities and custom render functions are in `src/testing/`

**Component Tests**
  - Use `renderWithProviders` from `src/testing/render` for consistent test setup
  - Mock API calls using MSW handlers
  - Test both success and error scenarios

## 🛠️ Tech Stack

- **Framework**: React 19
- **Language**: TypeScript
- **Build Tool**: Vite
- **Styling**: Styled Components, Bootstrap
- **State Management**: React Query
- **Routing**: React Router
- **API Client**: Orval
- **Linting**: ESLint
- **Formatting**: Prettier

## 📚 Documentation
- [Eamerald](https://www.topaz.sh/docs/getting-started)
- [React Documentation](https://react.dev/)
- [TypeScript Documentation](https://www.typescriptlang.org/docs/)
- [Vite Documentation](https://vitejs.dev/guide/)
- [React Query Documentation](https://tanstack.com/query/latest)
- [Styled Components Documentation](https://styled-components.com/docs)

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the Apache License - see the [LICENSE](LICENSE) file for details.
