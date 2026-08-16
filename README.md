# JSONline

A lightweight, zero-dependency static web utility to flatten multiline text into single-line JSON strings and expand escaped payload strings back into human-readable text.

---

## Features

* **Multiline $\to$ Single Line**
* Escape newlines to literal `\n` sequences (ideal for raw JSON values and API testing).
* Optional space separation or complete newline removal.
* Optional quote escaping (`"` $\to$ `\"`).


* **Single Line $\to$ Multiline**
* Parse literal `\n` and `\r` into real line breaks.
* Auto-unescape quotes (`\"` $\to$ `"`).
* Auto-strip enclosing wrapping quotes (e.g. `"..."`).


* **Fast Workflow**
* One-click swap to easily invert transformations.
* Instant copy-to-clipboard functionality.
* Runs entirely client-side with zero telemetry or network calls.



---

## Getting Started

Because **JSONline** is a single static HTML file:

1. Clone or download `index.html`.
2. Double-click to open it in any modern browser.

No build tools, package managers, or server runtimes required.

---

## Use Cases

| Problem | Transformation | Output Target |
| --- | --- | --- |
| Injecting prompt templates, logs, or private keys into JSON payloads | Multiline $\to$ Single Line (with `\n`) | cURL, Postman, CI/CD env vars |
| Reading raw escaped strings from API error responses or logs | Single Line $\to$ Multiline | Text editor, Markdown preview |
| Formatting multiline SQL or GraphQL queries for inline JSON fields | Multiline $\to$ Single Line (with `\"`) | API test suites |

---

## License

MIT