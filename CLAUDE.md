# Voice Helper Project Guidelines

## Commands
- Build: `npm start` - Runs the Electron application
- Package: `npm run package` - Packages the app for distribution
- Distribution: `npm run make` - Creates distributables
- Publish: `npm run publish` - Publishes the app
- Lint: `npm run lint` - Runs ESLint on TypeScript files

## Code Style
- **TypeScript**: Use strict typing with noImplicitAny
- **Formatting**: Follow ESLint rules (Standard + TypeScript ESLint)
- **Imports**: Sort imports and use explicit named imports
- **Naming**: Use camelCase for variables/functions, PascalCase for components/interfaces
- **Error Handling**: Use try/catch blocks with specific error types
- **Components**: Use functional components with hooks, avoid class components
- **Comments**: Document complex logic and public interfaces
- **React**: Use React.FC type for components, organize by feature

## Architecture
- Electron app with main process (main.ts) and React-based renderer (renderer.tsx)
- React components in separate files, organized by feature
- Use preload.ts for secure IPC between processes
- Follow Electron security best practices

This is a TypeScript-based Electron project with React UI and Vite for bundling.