# JS Code Helper

A VS Code extension with snippets for the modern React/JavaScript stack — Redux Toolkit, TanStack Query, React Hook Form + Zod, Axios, and common hooks. Works in `.js`, `.jsx`, `.ts`, and `.tsx` files, with TypeScript-typed variants where it matters.

## Snippets

### State management

| Prefix | What it inserts | Required packages |
| --- | --- | --- |
| `rtkslice` | `createSlice` with reducers + exported actions | `@reduxjs/toolkit`, `react-redux` |
| `rtkthunk` | `createAsyncThunk` + slice with pending/fulfilled/rejected | `@reduxjs/toolkit`, `axios` |
| `rtkstore` | `configureStore` (TS variant exports typed hooks) | `@reduxjs/toolkit`, `react-redux` |
| `rtkstorepersist` | `configureStore` with `redux-persist` (JS only) | `@reduxjs/toolkit`, `redux-persist` |
| `rtkhooks` | `useSelector` + `useDispatch` usage (JS only) | `react-redux` |
| `zustand` | Minimal Zustand store | `zustand` |

### Data fetching

| Prefix | What it inserts | Required packages |
| --- | --- | --- |
| `rqquery` | `useQuery` hook with `axios` fetcher | `@tanstack/react-query`, `axios` |
| `rqmutation` | `useMutation` with cache invalidation | `@tanstack/react-query`, `axios` |
| `rqprovider` | `QueryClientProvider` setup (JS only) | `@tanstack/react-query` |
| `axioget` / `axiopost` | Axios GET / POST with async/await | `axios` |
| `axioinstance` | Axios instance with auth + error interceptors | `axios` |
| `usefetch` | `useEffect` fetch with `AbortController` cleanup (JS only) | `axios` |

### Forms

| Prefix | What it inserts | Required packages |
| --- | --- | --- |
| `rhfzod` | React Hook Form + Zod (TS variant uses `z.infer`) | `react-hook-form`, `@hookform/resolvers`, `zod` |
| `rfy` | Formik + Yup form (kept for legacy) | `formik`, `yup` |

### Components & hooks

| Prefix | What it inserts |
| --- | --- |
| `rfc` | Functional component (TS variant adds typed props) |
| `rhook` | Custom hook scaffold |
| `rerrorboundary` | Error boundary class component |
| `rrouter` | React Router v6 routes setup (JS only) |
| `usestate`, `useeffect`, `usereducer` | Inline hook snippets |
| `usedebounce` | `useDebounce` hook (TS variant is generic) |

## Installation

Install from the [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=AmitKRout.js-helper-code-extension-vs), or search for "JS Helper Code Snippets" inside VS Code's Extensions panel.

## Usage

Open any `.js`, `.jsx`, `.ts`, or `.tsx` file, type a prefix from the table above, and press <kbd>Tab</kbd>. Use <kbd>Tab</kbd> to jump between placeholders.

## Contributing

Issues and PRs are welcome at [github.com/amitkroutthedev/js-code-helper](https://github.com/amitkroutthedev/js-code-helper). To add a snippet, edit `snippets/snippets.code-snippets` (and the TS counterpart if it makes sense to type) and update the table above.

## License

MIT — see [LICENSE.md](./LICENSE.md).
