# importmap-store

**importmap-store** is a free and open-source tool to manage import maps dynamically in your JavaScript projects.

---

## Import Map

```json
{
  "imports": {
    "react": "https://cdn.jsdelivr.net/npm/react@19.2.4/umd/react.development.js",
    "react-dom": "https://cdn.jsdelivr.net/npm/react-dom@19.2.4/umd/react-dom.development.js",
    "classnames": "https://cdn.jsdelivr.net/npm/classnames@2.3.2/index.js",
    "@reduxjs/toolkit": "https://cdn.jsdelivr.net/npm/@reduxjs/toolkit@1.9.5/dist/redux-toolkit.umd.min.js",
    "react-router-dom": "https://cdn.jsdelivr.net/npm/react-router-dom@6.17.0/umd/react-router-dom.development.js",
    "framer-motion": "https://cdn.jsdelivr.net/npm/framer-motion@10.12.5/dist/framer-motion.js"
    // ...other packages. see store/all.json
  }
}
```

## Usage

```js
import { loadImportMaps } from "https://cdn.jsdelivr.net/npm/@jdx-plugins/importmap-loader@0.1.0/dist/loader.js";

(async () => {
  const maps = await loadImportMaps({
    maps: ['https://impm.opendnf.cloud/store/all.json'],
    version: '1'
  });

  console.log(maps.imports);
})();
```

## License
MIT License

## Author

2026 (C) OpenDN Foundation
