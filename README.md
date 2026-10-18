# LIWI — One playground, many languages

LIWI is a mobile-first coding playground designed for learning and experimenting from a phone.

## Current starter features

- One editor with a language selector, examples, and a Run button
- Python in the browser via Pyodide, including pre-supplied input for `input()`
- JavaScript execution and TypeScript transpilation in the browser
- HTML and CSS preview in a sandboxed iframe
- JSON syntax validation
- Remote execution for C++, C, Java, C#, Go, Rust, PHP, Ruby, Bash, SQL, and Kotlin through the Piston API
- Output console, error display, and mobile-responsive layout

## Run it

Open `index.html` in a modern browser or enable GitHub Pages for this repository. The first Python run downloads the Python runtime. Remote languages need an internet connection and a reachable Piston service.

**Privacy note:** Python, JavaScript, TypeScript, HTML, CSS, and JSON are processed in the browser (external runtime libraries may be downloaded). The other language options send code and stdin to a remote execution service. Do not submit passwords, API keys, or private information.

## Roadmap

- Improve editor autocomplete and language-specific highlighting
- Add persistent projects and multiple files
- Add a clearer input workflow for interactive programs
- Add tests and status checks for supported language runners
- Evaluate a self-hosted runner for better reliability and privacy

## Hosting

The workflow in `.github/workflows/pages.yml` deploys the site to GitHub Pages after a push to `main`. In the repository settings, set **Pages → Build and deployment → Source** to **GitHub Actions** if it is not already selected.
