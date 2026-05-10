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
| `ERR_UNSUPPORTED_DIR_IMPORT` | [nodejs-errors.dev/ERR_UNSUPPORTED_DIR_IMPORT/](https://nodejs-errors.dev/ERR_UNSUPPORTED_DIR_IMPORT/) |
| `ERR_DLOPEN_FAILED` (native addon ABI mismatch) | [nodejs-errors.dev/ERR_DLOPEN_FAILED/](https://nodejs-errors.dev/ERR_DLOPEN_FAILED/) |

### File System & I/O

| Error | Page |
|---|---|
| `ENOENT: no such file or directory` | [nodejs-errors.dev/ENOENT/](https://nodejs-errors.dev/ENOENT/) |
| `EMFILE: too many open files` | [nodejs-errors.dev/EMFILE/](https://nodejs-errors.dev/EMFILE/) |
| `Error: write EPIPE` | [nodejs-errors.dev/EPIPE/](https://nodejs-errors.dev/EPIPE/) |
| `EACCES: permission denied` | [nodejs-errors.dev/EACCES/](https://nodejs-errors.dev/EACCES/) |
| `EPERM: operation not permitted` | [nodejs-errors.dev/EPERM/](https://nodejs-errors.dev/EPERM/) |
| `ENOSPC: no space left on device` / `System limit for number of file watchers reached` | [nodejs-errors.dev/ENOSPC/](https://nodejs-errors.dev/ENOSPC/) |

### Network

| Error | Page |
|---|---|
| `EADDRINUSE: address already in use` | [nodejs-errors.dev/EADDRINUSE/](https://nodejs-errors.dev/EADDRINUSE/) |
| `Error: read ECONNRESET` | [nodejs-errors.dev/ECONNRESET/](https://nodejs-errors.dev/ECONNRESET/) |
| `Error: connect ECONNREFUSED` | [nodejs-errors.dev/ECONNREFUSED/](https://nodejs-errors.dev/ECONNREFUSED/) |
| `Error: connect ETIMEDOUT` | [nodejs-errors.dev/ETIMEDOUT/](https://nodejs-errors.dev/ETIMEDOUT/) |
| `Error: getaddrinfo ENOTFOUND` | [nodejs-errors.dev/ENOTFOUND/](https://nodejs-errors.dev/ENOTFOUND/) |
| `Error [ERR_HTTP_HEADERS_SENT]: Cannot set headers after they are sent to the client` | [nodejs-errors.dev/ERR_HTTP_HEADERS_SENT/](https://nodejs-errors.dev/ERR_HTTP_HEADERS_SENT/) |

### Streams

| Error | Page |
|---|---|
| `Error [ERR_STREAM_WRITE_AFTER_END]: write after end` | [nodejs-errors.dev/ERR_STREAM_WRITE_AFTER_END/](https://nodejs-errors.dev/ERR_STREAM_WRITE_AFTER_END/) |
| `Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close` | [nodejs-errors.dev/ERR_STREAM_PREMATURE_CLOSE/](https://nodejs-errors.dev/ERR_STREAM_PREMATURE_CLOSE/) |

### Runtime

| Error | Page |
|---|---|
| `TypeError: Cannot read properties of undefined` | [nodejs-errors.dev/TypeError-Cannot-read-properties-of-undefined/](https://nodejs-errors.dev/TypeError-Cannot-read-properties-of-undefined/) |
| `TypeError: Cannot set properties of undefined` | [nodejs-errors.dev/TypeError-Cannot-set-properties-of-undefined/](https://nodejs-errors.dev/TypeError-Cannot-set-properties-of-undefined/) |
| `ReferenceError: document is not defined` | [nodejs-errors.dev/ReferenceError-document-is-not-defined/](https://nodejs-errors.dev/ReferenceError-document-is-not-defined/) |
| `TypeError [ERR_INVALID_ARG_TYPE]` | [nodejs-errors.dev/ERR_INVALID_ARG_TYPE/](https://nodejs-errors.dev/ERR_INVALID_ARG_TYPE/) |
| `UnhandledPromiseRejection` | [nodejs-errors.dev/UnhandledPromiseRejection/](https://nodejs-errors.dev/UnhandledPromiseRejection/) |
| `RangeError: Maximum call stack size exceeded` | [nodejs-errors.dev/RangeError-Maximum-call-stack-size-exceeded/](https://nodejs-errors.dev/RangeError-Maximum-call-stack-size-exceeded/) |
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
├── JavaScript-heap-out-of-memory/
│   └── index.html
├── ERR_HTTP_HEADERS_SENT/
│   └── index.html
├── EACCES/
│   └── index.html
├── EPERM/
│   └── index.html
├── ENOSPC/
│   └── index.html
├── ERR_UNSUPPORTED_DIR_IMPORT/
│   └── index.html
├── ERR_DLOPEN_FAILED/
│   └── index.html
├── ERR_STREAM_WRITE_AFTER_END/
│   └── index.html
├── ERR_STREAM_PREMATURE_CLOSE/
│   └── index.html
├── RangeError-Maximum-call-stack-size-exceeded/
│   └── index.html
└── TypeError-Cannot-set-properties-of-undefined/
    └── index.html
```
