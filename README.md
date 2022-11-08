This is a starter that builds an app/component as a component library deployable on _npm_ and as a widget creating 2 files deployable on a CDN.

# Scaffolding

- **widget-build** - contains the build of the widget version
- **widget-example** - contains the usage example of the built widget
- **dist** - contains the component lib build
- **src/index.ts** - is the entry point for the component lib and exports the React component
- **src/index.widget.tsx** - is the entry point for the widget that is built as a single js and css file

# Development

Install deps
```
npm install
```

Run Storybook
```
npm run dev
```
The main component can be developed using Storybook. Inside the story is rendered the component exported by the final component library.

Tailwind CSS is enable by default.

# Build

Build component library

```
npm run build
```
Build widget
```
npm run build:widget
```
Serve the widget
```
npm run serve:widget
```

As you can see the app/component can be built in two ways.

- The component library built with Rollup
- The widget files built with Parcel