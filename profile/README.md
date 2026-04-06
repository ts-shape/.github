# tsshape

**TypeScript utilities for shaping types and data.**

---

## About

tsshape is a collection of focused TypeScript packages for transforming, validating, and composing types and data structures. Each package is small, dependency-light, and designed to work seamlessly in both Node.js and browser environments.

---

## Packages

| Package | Description | Version |
|---------|-------------|---------|
| [`@tsshape/core`](https://github.com/ts-shape/core) | Core type transformation primitives | ![npm](https://img.shields.io/npm/v/@tsshape/core) |
| [`@tsshape/schema`](https://github.com/ts-shape/schema) | Runtime schema definition and validation | ![npm](https://img.shields.io/npm/v/@tsshape/schema) |
| [`@tsshape/utils`](https://github.com/ts-shape/utils) | Type-safe utility helpers | ![npm](https://img.shields.io/npm/v/@tsshape/utils) |

---

## Quick Start

```sh
npm install @tsshape/core
```

```ts
import { shape } from '@tsshape/core'

const User = shape({
  id: 'number',
  name: 'string',
  email: 'string',
})

type User = typeof User.infer
// { id: number; name: string; email: string }
```

---

## Links

- [GitHub Repositories](https://github.com/orgs/ts-shape/repositories)
- [npm Organization](https://www.npmjs.com/org/tsshape)
