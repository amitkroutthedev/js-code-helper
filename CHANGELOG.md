# Changelog

## 1.0.0

### Added
- TypeScript and JSX/TSX language support — snippets now activate in `.js`, `.jsx`, `.ts`, and `.tsx` files.
- Separate TS-typed snippet file with `PayloadAction`, `z.infer`, typed `useQuery`/`useMutation`, and typed Axios calls.
- Redux Toolkit snippets: `rtkslice`, `rtkthunk`, `rtkstore`, `rtkstorepersist`, `rtkhooks`.
- TanStack Query snippets: `rqquery`, `rqmutation`, `rqprovider`.
- React Hook Form + Zod snippet: `rhfzod`.
- Modern Axios patterns: async/await `axioget`/`axiopost`, `axioinstance` with interceptors, `usefetch` with `AbortController`.
- Component & hook scaffolds: `rfc`, `rhook`, `rerrorboundary`, `rrouter`, `usestate`, `useeffect`, `usereducer`, `usedebounce`.
- Zustand store snippet.

### Changed
- Replaced legacy hand-written Redux action/reducer/store snippets (`actioncreate`, `reducercreate`, `storecreate`) with Redux Toolkit equivalents.
- Bumped minimum VS Code engine to `^1.85.0`.
- Repository field now points to the public GitHub URL.

### Kept
- Formik + Yup snippet (`rfy`) preserved for projects still on that stack.

## 0.1.0
- Updated Formik snippet.

## 0.0.1
- Initial release: snippets for Axios, Redux, Formik, and Yup.