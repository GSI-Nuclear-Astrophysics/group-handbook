# 💻 Software Development Guidelines

To ensure our scientific code is maintainable and reproducible, all members follow these practices.

### 1. Development Workflow
*   **`main` branch:** Protected primary branch. It must always hold a working version. **No direct commits to main.**
*   **Feature Branches:** Use the pattern `devel-<initials>-<feature>` (e.g., `devel-df-schottky-fit`).
*   **Pull Requests (PR):** When a feature is tested, open a PR into `main`. At least one other group member should review the code for major projects.
*   **Legacy Branches:** For specific beamtimes, use `run-YYYY-MM` (e.g., `run-2025-05`).

### 2. Commit Messages
*   Use the **Conventional Commits** format: `type(scope): description`.
*   *Types:* `feat` (new feature), `fix` (bug fix), `docs` (documentation), `refactor` (code cleanup).
*   *Example:* `feat(analysis): add relativistic correction to mass fit`

### 3. Coding Style
*   **Python:** Follow [PEP 8](https://peps.python.org/pep-0008/). Use `black` or `flake8` for auto-formatting.
*   **C++:** Follow the [Google C++ Style Guide](https://google.github.io/styleguide/cppguide.html) or similar.
*   **Comments:** Write code that is "self-documenting," but use comments to explain the *physics* logic behind complex formulas.

### 4. Documentation
*   Every repository must have a `README.md` with:
    *   Installation instructions (dependencies).
    *   A minimal working example (MWE).
    *   Contact person for the code.

### 5. Security
*   **NEVER** commit GSI passwords, private SSH keys, or internal IP addresses to public repositories.
*   Use `.gitignore` to exclude large data files (`.root`, `.csv`, `.dat`).

### 6. Extra Resources
*   Find our **Git Introduction Slides** [here](./assets/slides/git-introduction.pdf).
*   Check the [Git Deep Dive](./docs/git-advanced.md) for handling merge conflicts.
