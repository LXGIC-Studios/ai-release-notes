# ai-release-notes

[![npm version](https://img.shields.io/npm/v/ai-release-notes.svg)](https://www.npmjs.com/package/ai-release-notes)
[![npm downloads](https://img.shields.io/npm/dm/ai-release-notes.svg)](https://www.npmjs.com/package/ai-release-notes)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/lxgic-studios/ai-release-notes)](https://github.com/lxgic-studios/ai-release-notes/stargazers)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0+-blue)](https://www.typescriptlang.org/)



Turn your messy git log or changelog into release notes that people actually want to read.

## What it does

Point it at your repo and it'll read through your commits or CHANGELOG file, then spit out clean, grouped release notes. You can pick a tone too. Want it fun? Professional? Casual? Up to you.

## Install

```bash
npm install -g ai-release-notes
```

## Usage

```bash
# Generate from git history since a tag
npx ai-release-notes --from v1.0.0

# Make it fun
npx ai-release-notes --from v1.0.0 --tone fun

# Between two tags
npx ai-release-notes --from v1.0.0 --to v2.0.0

# From a changelog file
npx ai-release-notes --changelog CHANGELOG.md
```

## Setup

You'll need an OpenAI API key set as an environment variable:

```bash
export OPENAI_API_KEY=your-key-here
```

## Options

- `--from <tag>` - Starting git tag or commit
- `--to <tag>` - Ending tag (defaults to HEAD)
- `--tone <tone>` - How you want it to sound (fun, professional, casual)
- `--changelog <path>` - Point to a specific changelog file
- `--cwd <dir>` - Run from a different directory

## License

MIT
