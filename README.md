# mobile_test

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

## Commit Convention and Versioning Increment

This project follows a strict commit convention that allows for the automatic increment of the project's version based on the types of changes made to the code. This convention ensures that version updates are handled correctly and consistently with each significant change.

### Commit Types

Commits should follow the conventions below to ensure the version increment script works correctly:

- **`breaking:`** (Breaking Change) - Changes that introduce backward-incompatible changes to the project.
- **`feat:`** (Feature) - Adding new features to the project.
- **`fix:`** (Bug Fix) - Fixing bugs in the project.
- **`chore:`** (Chore) - Miscellaneous tasks that do not alter the functionality (e.g., updating dependencies, improving tests, etc.).

### Versioning Increment

The version increment script relies on commit messages to determine the type of change made and automatically increments the version accordingly.

## Version Increment Rules

### 1. Major Version (`breaking:`)

- If a commit contains the keyword `breaking:`, the **major** version is incremented.
- Both the **minor** and **patch** versions are reset to `0`.
- **Example:**  
  If the current version is `1.2.3`, after a `breaking:` change, the new version will be `2.0.0`.
- The changelog will also include a **Major Changes** section that lists any breaking changes under this increment.

### 2. Minor Version (`feat:`)

- If a commit contains the keyword `feat:`, the **minor** version is incremented.
- The **patch** version is reset to `0`.
- **Example:**  
  If the current version is `1.2.3`, after a `feat:` change, the new version will be `1.3.0`.

### 3. Patch Version

#### Bug Fixes (`fix:`)

- If a commit contains the keyword `fix:`, the **patch** version is incremented.
- **Example:**  
  If the current version is `1.2.3`, after a `fix:` change, the new version will be `1.2.4`.

#### Chores (`chore:`)

- If a commit contains the keyword `chore:`, the **patch** version is incremented.
- **Example:**  
  If the current version is `1.2.3`, after a `chore:` change, the new version will be `1.2.4`.

#### Refactors (`refactor:`)

- If a commit contains the keyword `refactor:`, the **patch** version is incremented.
- **Example:**  
  If the current version is `1.2.3`, after a `refactor:` change, the new version will be `1.2.4`.

#### Style Changes (`style:`)

- If a commit contains the keyword `style:`, the **patch** version is incremented.
- **Example:**  
  If the current version is `1.2.3`, after a `style:` change, the new version will be `1.2.4`.

### Example Commits

Here are some example commit messages that follow the convention:

- **Breaking change**:

  ```bash
  breaking: update API to support new data format
  ```

- **Adding a new feature**:

  ```bash
  feat: add file upload feature
  ```

- **Fixing a bug**:

  ```bash
  fix: resolve issue with file upload
  ```

- **Chore task (e.g., dependency update)**:
  ```bash
  chore: update dependencies
  ```

