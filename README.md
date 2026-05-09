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
| `SyntaxError: Cannot use import statement outside a module` | [nodejs-errors.dev/SyntaxError-Cannot-use-import-statement/](https://nodejs-errors.dev/SyntaxError-Cannot-use-import-statement/) |

### File System & I/O

| Error | Page |
|---|---|
| `ENOENT: no such file or directory` | [nodejs-errors.dev/ENOENT/](https://nodejs-errors.dev/ENOENT/) |
| `EMFILE: too many open files` | [nodejs-errors.dev/EMFILE/](https://nodejs-errors.dev/EMFILE/) |
| `Error: write EPIPE` | [nodejs-errors.dev/EPIPE/](https://nodejs-errors.dev/EPIPE/) |

### Network

| Error | Page |
|---|---|
| `EADDRINUSE: address already in use` | [nodejs-errors.dev/EADDRINUSE/](https://nodejs-errors.dev/EADDRINUSE/) |
| `Error: read ECONNRESET` | [nodejs-errors.dev/ECONNRESET/](https://nodejs-errors.dev/ECONNRESET/) |
| `Error: connect ECONNREFUSED` | [nodejs-errors.dev/ECONNREFUSED/](https://nodejs-errors.dev/ECONNREFUSED/) |
| `Error: connect ETIMEDOUT` | [nodejs-errors.dev/ETIMEDOUT/](https://nodejs-errors.dev/ETIMEDOUT/) |
| `Error: getaddrinfo ENOTFOUND` | [nodejs-errors.dev/ENOTFOUND/](https://nodejs-errors.dev/ENOTFOUND/) |

### Runtime

| Error | Page |
|---|---|
| `TypeError: Cannot read properties of undefined` | [nodejs-errors.dev/TypeError-Cannot-read-properties-of-undefined/](https://nodejs-errors.dev/TypeError-Cannot-read-properties-of-undefined/) |
| `ReferenceError: document is not defined` | [nodejs-errors.dev/ReferenceError-document-is-not-defined/](https://nodejs-errors.dev/ReferenceError-document-is-not-defined/) |
| `TypeError [ERR_INVALID_ARG_TYPE]` | [nodejs-errors.dev/ERR_INVALID_ARG_TYPE/](https://nodejs-errors.dev/ERR_INVALID_ARG_TYPE/) |
| `UnhandledPromiseRejection` | [nodejs-errors.dev/UnhandledPromiseRejection/](https://nodejs-errors.dev/UnhandledPromiseRejection/) |
| `FATAL ERROR: JavaScript heap out of memory` | [nodejs-errors.dev/JavaScript-heap-out-of-memory/](https://nodejs-errors.dev/JavaScript-heap-out-of-memory/) |

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
├── index.html                                              # Homepage — lists all error pages
├── sitemap.xml
├── robots.txt
├── llms.txt                                               # AI crawler manifest
├── MODULE_NOT_FOUND/
│   └── index.html
├── ERR_PACKAGE_PATH_NOT_EXPORTED/
│   └── index.html
├── ERR_REQUIRE_ESM/
│   └── index.html
├── SyntaxError-Cannot-use-import-statement/
│   └── index.html
├── ENOENT/
│   └── index.html
├── EMFILE/
│   └── index.html
├── EPIPE/
│   └── index.html
├── EADDRINUSE/
│   └── index.html
├── ECONNRESET/
│   └── index.html
├── ECONNREFUSED/
│   └── index.html
├── ETIMEDOUT/
│   └── index.html
├── ENOTFOUND/
│   └── index.html
├── TypeError-Cannot-read-properties-of-undefined/
│   └── index.html
├── ReferenceError-document-is-not-defined/
│   └── index.html
├── ERR_INVALID_ARG_TYPE/
│   └── index.html
├── UnhandledPromiseRejection/
│   └── index.html
└── JavaScript-heap-out-of-memory/
    └── index.html
```
