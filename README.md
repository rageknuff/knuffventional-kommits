# knuffventional kommits ✨

A commit message format that uses emojis for quick visual identification.  
> 🤷 *it's fun. - don't take it too seriously.*
## Format

```
emoji (scope) description
```

- `emoji` - one of the type emojis (see below)
- `(scope)` - optional context
- `description` - present tense, max 72 characters

## Commit Types

| Emoji | Type        | Description                         | Conventional Equivalent |
| ----- | ----------- | ----------------------------------- | ----------------------- |
| ✨     | feature     | new functionality / new UI          | `feat`                  |
| 🐛    | fix         | fix bugs, errors, issues            | `fix`                   |
| 🔨    | refactor    | code refactors                      | `refactor`              |
| 🧪    | test        | add / update tests                  | `test`                  |
| 📋    | docs        | documentation changes               | `docs`                  |
| 🏎️   | performance | performance improvement             | `perf`                  |
| 📦    | build       | dependencies, build, CI/CD          | `build`, `ops`          |
| 🧹    | chore       | maintenance, cleanup, misc. changes | `chore`, `style`        |

## Conventional to Emoji Mapping

- `feat` → ✨
- `fix` → 🐛  
- `refactor` → 🔨
- `test` → 🧪
- `docs` → 📋
- `perf` → 🏎️
- `build`, `ops` → 📦
- `chore`, `style` → 🧹

## Rules

- **One emoji per commit** - No combining types
- **Lowercase start** - Except proper nouns, brands, or technical terms (API, OAuth, Docker)
- **Present tense** - "add" not "added", "fix" not "fixed"  
- **72 character limit** - For clean display in `git log --oneline`
	- *if you need more, put it in the body, or split into smaller commits*
- **Optional scope** - Use `(scope)` for context: modules, components, files (e.g., `(auth)`, `(cart)`), etc.
	- *to mark a breaking change, append `!` after the closing parenthesis: `(scope)!`*
- **No empty descriptions** - Always provide meaningful description

## Examples

```
✨ add user authentication system
✨ (auth) add OAuth integration
🐛 fix login redirect loop
🐛 (ui) fix navigation menu overflow
🔨 simplify user service module
🔨 (utils) extract validation helpers
🧪 add unit tests for user service
📋 update API documentation
📋 (readme) add installation instructions
🧹 apply gofmt 
✨ improve mobile responsiveness
✨ (dashboard) redesign layout
🏎️ cache user info after login
📦 update dependencies
📦 (ci) add GitHub Actions workflow
🧹 add build artifacts to .gitignore
🔨 (cfg)! change default database port to 5433
```

## Git Log Example

```
886bb7c7 ✨ add user authentication system
9a4d2f1e 🐛 (ui) fix navigation menu overflow
1c7b5a3f 📋 update API documentation
7d8e9b0a 🔨 simplify user service module
2f5c6d4b 🧪 add unit tests for user service
d34db44f 🔨 (api)! remove `old_login` endpoint
9e3a7b5c ✨ redesign dashboard layout
6d8c3e9f 📦 update dependencies
137ee79a 🧹 add build artifacts to .gitignore
```

> *Like it? Make it yours! Use whatever emojis you prefer - embrace the silliness🕺*