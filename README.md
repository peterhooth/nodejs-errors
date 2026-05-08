# nodejs-errors.dev

**[nodejs-errors.dev](https://nodejs-errors.dev/)** — authoritative reference for Node.js error messages.

Each page covers the exact error message, root cause, step-by-step fixes, and copy-pasteable code examples.

---

## Error pages

### Module Resolution

| Error | Page |
|---|---|
| `Error: Cannot find module` | [nodejs-errors.dev/MODULE_NOT_FOUND/](https://nodejs-errors.dev/MODULE_NOT_FOUND/) |
| `ERR_PACKAGE_PATH_NOT_EXPORTED` | [nodejs-errors.dev/ERR_PACKAGE_PATH_NOT_EXPORTED/](https://nodejs-errors.dev/ERR_PACKAGE_PATH_NOT_EXPORTED/) |
| `ERR_REQUIRE_ESM` | [nodejs-errors.dev/ERR_REQUIRE_ESM/](https://nodejs-errors.dev/ERR_REQUIRE_ESM/) |

### File System

| Error | Page |
|---|---|
| `ENOENT: no such file or directory` | [nodejs-errors.dev/ENOENT/](https://nodejs-errors.dev/ENOENT/) |

### Network

| Error | Page |
|---|---|
| `EADDRINUSE: address already in use` | [nodejs-errors.dev/EADDRINUSE/](https://nodejs-errors.dev/EADDRINUSE/) |

### Runtime

| Error | Page |
|---|---|
| `TypeError: Cannot read properties of undefined` | [nodejs-errors.dev/TypeError-Cannot-read-properties-of-undefined/](https://nodejs-errors.dev/TypeError-Cannot-read-properties-of-undefined/) |

---

## Contributing

To add a new error page:

1. Create a new folder named after the error code, e.g. `ENOENT/`
2. Add an `index.html` inside it — use an existing page as a template
3. Add a card to the right category section in `index.html` (root)
4. Add a `<url>` entry to `sitemap.xml`
5. Add a line to `llms.txt`
6. Add a row to the table in `README.md`
7. Open a pull request

---

## Structure

```
nodejs-errors.dev/
├── index.html                                          # Homepage — lists all error pages
├── sitemap.xml
├── robots.txt
├── llms.txt                                            # AI crawler manifest
├── MODULE_NOT_FOUND/
│   └── index.html
├── ERR_PACKAGE_PATH_NOT_EXPORTED/
│   └── index.html
├── ERR_REQUIRE_ESM/
│   └── index.html
├── ENOENT/
│   └── index.html
├── EADDRINUSE/
│   └── index.html
└── TypeError-Cannot-read-properties-of-undefined/
    └── index.html
```
