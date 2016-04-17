> The npm module of Catalog can be integrated into your React application, so you can develop your components directly in your styleguide.

## Installation

```
npm install catalog --save
```

```hint
Please make sure that you're using npm `>= 2.14.12` (npm 3 is recommended). Older versions have a bug which prevents the catalog module from being installed properly. To upgrade, use `npm install npm@2 -g` (omit the `@2` if you want to upgrade to npm 3).
```

## Usage

### Standalone

```code|lang-jsx
import {render} from 'catalog';
import Intro from './docs/Intro';
import ButtonDocs from './docs/Buttons';
import GridDocs from './docs/Grids';

render({
  title: 'My Styleguide',
  basePath: '/catalog',
  pages: [
    {
      path: '/',
      title: 'Introduction',
      component: Intro
    },
    {
      title: 'Components',
      pages: [
        {path: 'buttons', title: 'Buttons', component: ButtonDocs},
        {path: 'grid', title: 'Grid', component: GridDocs}
      ]
    }
  ]
}, document.getElementById('app'));
```

### With React Router

Instead of directly rendering, Catalog can provide its routes to mix them with your existing ones.

```code|lang-jsx
import {configureRoutes} from 'catalog';
import Intro from './docs/Intro';
import ButtonDocs from './docs/Buttons';
import GridDocs from './docs/Grids';

const catalogRoutes = configureRoutes({
  title: 'My Styleguide',
  basePath: '/catalog',
  pages: [
    {
      path: '/',
      title: 'Introduction',
      component: Intro
    }
    {
      title: 'Components',
      pages: [
        {path: 'buttons', title: 'Buttons', component: ButtonDocs},
        {path: 'grid', title: 'Grid', component: GridDocs}
      ]
    }
  ]
});

const routes = [
  catalogRoutes,
  // other routes ...
];


ReactDOM.render(<Router routes={routes} />, document.getElementById('app'));
```

## Writing Documentation

Instead of using Markdown files, you can use Catalog's components directly. This allows you to write your documentation in a relatively concise way while maintaining maximal flexibility.

If you provide these components to the configuration (see above), they will display nicely as individual pages.

```code|lang-jsx
import React from 'react';
import {Page, ReactSpecimen} from 'catalog';
import Button from 'components/Button/Button';

export default () => (
  <Page>
    <h2>My Buttons</h2>

    <p>Are so nice</p>

    <ul>
      <li>Yes</li>
      <li>or no?</li>
    </ul>

    <hr />

    <ReactSpecimen span={3}>
      <Button primary>Foo</Button>
    </ReactSpecimen>

    <ReactSpecimen span={3}>
      <Button disabled>Foo</Button>
    </ReactSpecimen>

    <ReactSpecimen span={3}>
      <Button disabled primary>Foo</Button>
    </ReactSpecimen>
  </Page>
);
```
