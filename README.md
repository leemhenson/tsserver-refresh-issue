### tsserver refresh issue

1. `pnpm recursive install --link-workspace-packages`
2. `tsc --build ./tsconfig.json --verbose --watch`
3. Observe the two packages compile successfully.
4. Open `packages/consumer-package/src/index.ts` and `packages/shared-package/src/index.ts` in your editor.
5. Uncomment the `age` property in `packages/shared-package/src/index.ts` and observe no feedback in `packages/consumer-package/src/index.ts`.
6. Observe that the `tsc --build` output shows the error as expected.
