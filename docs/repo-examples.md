# 11. Repository Examples

Well-structured repositories help teams collaborate efficiently. The following examples show different ways to organize code and documentation while keeping usability in mind.

## Example: Documentation-First Layout

This repository uses a documentation-only approach. Everything resides in a `docs/` folder with a simple README to guide learners. The structure might look like this:

```text
my-course/
├── README.md
└── docs/
    ├── introduction.md
    ├── principles.md
    └── ...
```

A clear index in the main README ensures visitors can quickly find each lesson.

## Example: Code with Docs and Tests

When your project includes source code, group related files so developers know where to look:

```text
my-app/
├── README.md
├── src/
│   ├── index.js
│   └── components/
├── docs/
│   └── getting-started.md
└── tests/
    └── basic.test.js
```

- **`src/`** contains the implementation.
- **`docs/`** holds guides and API references.
- **`tests/`** includes unit or integration tests.

This layout keeps documentation close to the code while maintaining separation between functionality and learning material.

## Example: Design Assets Repository

Large projects sometimes dedicate a repository to design files:

```text
design-system/
├── README.md
├── components/
│   └── button.sketch
├── style-guide.md
└── prototypes/
    └── mobile-wireframe.fig
```

Storing design artifacts alongside usage guidelines helps developers implement components consistently.

## Tips for Repository UX

- Keep your README concise with links to deeper documentation.
- Use consistent naming for folders so newcomers understand the structure.
- Provide example code or templates to accelerate setup.
- Include contribution guidelines to explain how others can help.

Thoughtful organization reduces onboarding time and makes it easier for teams to maintain a project over its lifetime.
