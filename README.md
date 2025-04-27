#### Yarn

| Yarn node-modules -home  | `yarn config set nodeLinker node-modules --home` |
| ------------------------ | ------------------------------------------------ |
| Yarn pnp --home          | `yarn config set nodeLinker pnp --home`          |
| Check yarn change or not | `yarn config get nodeLinker`                     |
| Yarn update              | `yarn set version stable`                        |

#### TypeScript File alias

| Install a Package          | `yarn add vite-tsconfig-paths -D`                                       |
| -------------------------- | ----------------------------------------------------------------------- |
| import into vite.config.ts | `import tsConfigPaths from "vite-tsconfig-paths"`                       |
| import into vite.config.ts | `import path from "path"`                                               |
| use into the the plugins:  | ` plugins: [tsConfigPaths()]`                                           |
| In tsconfig.json files     | `  "compilerOptions": {"baseUrl": ".","paths": { "@/*": ["./src/*"] }}` |
| In tsconfig.app.json files | `"baseUrl": ".","paths": { "@/*": ["./src/*"] }}`                       |
| use vite.config.ts         | `resolve: { alias: {"@": path.resolve(__dirname, "./src"),},}`          |
