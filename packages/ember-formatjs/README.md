# ember-formatjs

Classic (ember-cli / broccoli) wiring for [`babel-plugin-ember-formatjs`](../babel-plugin-ember-formatjs), which combines the FormatJS authoring API with `ember-intl`.

```
ember install ember-intl ember-formatjs
```

That is the whole setup. This addon registers the two transforms with the classic build and does nothing else; all the transform logic lives in the plugin package, which comes along as a dependency.

**Embroider + Vite apps should not install this package.** Embroider v2 has no hook that lets an addon add a Babel plugin or a template transform to the host app, so there is nothing for this addon to do there. Install `babel-plugin-ember-formatjs` and wire it into `babel.config.mjs` instead; the [repository README](../../README.md) shows how.

See the [repository README](../../README.md) for usage, the extract and compile workflow, and options.
