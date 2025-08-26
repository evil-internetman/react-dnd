# Publishing @evil-internetmann/react-dnd Packages

## Overview

This repository contains the forked react-dnd packages published under the @evil-internetmann scope on npm.

## Published Packages

The following packages have been successfully published to npm:

### Core Packages
- `@evil-internetmann/invariant` (v4.0.2)
- `@evil-internetmann/shallowequal` (v4.0.2)
- `@evil-internetmann/asap` (v5.0.2)
- `@evil-internetmann/dnd-core` (v16.0.1)
- `@evil-internetmann/react-dnd` (v16.1.1)

### Backend Packages
- `@evil-internetmann/react-dnd-html5-backend` (v16.0.1)
- `@evil-internetmann/react-dnd-test-backend` (v16.0.1)
- `@evil-internetmann/react-dnd-touch-backend` (v16.0.1)

### Utility Packages
- `@evil-internetmann/test-utils` (v16.0.1)

## Publishing Process

1. **Update Package Names**: All packages were renamed with the `@evil-internetmann` scope
2. **Update Dependencies**: Internal dependencies were updated to use the new scoped names
3. **Fix Repository URLs**: All repository URLs were updated to point to `evil-internetman/react-dnd`
4. **Build Packages**: Run `yarn build` to build all packages
5. **Publish**: Each package was published using `npm publish --access public`

## Installation

To use these packages in your project:

```bash
npm install @evil-internetmann/react-dnd @evil-internetmann/react-dnd-html5-backend
```

## Usage

```javascript
import { DndProvider } from '@evil-internetmann/react-dnd';
import { HTML5Backend } from '@evil-internetmann/react-dnd-html5-backend';

// Use as normal
<DndProvider backend={HTML5Backend}>
  <App />
</DndProvider>
```