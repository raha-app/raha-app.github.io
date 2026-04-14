# raha-app.github.io

Raha App information website built with Hugo and the Blowfish theme.

## Requirements

- Git
- Hugo Extended (minimum `0.141.0` to match Blowfish requirements)

Check your installed versions:

```bash
git --version
hugo version
```

## Clone the project (with submodules)

This project includes Blowfish as a Git submodule under `themes/blowfish`, so clone it recursively:

```bash
git clone --recurse-submodules https://github.com/<your-org-or-user>/raha-app.github.io.git
cd raha-app.github.io
```

If you already cloned without submodules, run:

```bash
git submodule update --init --recursive
```

## Run locally

Start the local dev server:

```bash
hugo server -D
```

Then open:

- http://localhost:1313/

## Build for production

Generate the static site into `public/`:

```bash
hugo --minify
```

## Update the Blowfish theme submodule

From the repository root:

```bash
git submodule update --remote --merge
git add themes/blowfish
git commit -m "chore: update blowfish submodule"
```

## Common setup flow for contributors

```bash
git clone --recurse-submodules https://github.com/<your-org-or-user>/raha-app.github.io.git
cd raha-app.github.io
hugo server -D
```

## Notes

- Main site config is under `config/_default/`.
