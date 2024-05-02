# A Package for Registry Test

## Process

```bash
#!/bin/bash

npm config set registry=https://registry.npmjs.com/
npm login # User: rt-owner
npm publish
npm version minor
npm publish
npm unpublish
npm version major
npm publish
```

## Result

```bash
#!/bin/bash

npm view @registrytest/package --json
```
