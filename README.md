coursera-lab

A working archive of guided projects and capstones completed through Coursera. 
Each subdirectory is a self-contained project with its own context, code, and notes.

Structure

```
coursera-lab/
├── guided/
│   └── <project-slug>/
│       ├── README.md      # what it teaches, what I built
│       ├── src/           # code as submitted or refined
│       └── notes.md       # takeaways, gotchas, what I'd do differently
├── capstones/
│   └── <project-slug>/
│       ├── README.md
│       ├── src/
│       └── notes.md
└── certificates/
    ├── README.md          # index of credentials with dates and links
    └── <slug>.pdf         # one file per completed course or specialization
```

Conventions

- **Project slug**: lowercase, hyphenated, descriptive (e.g. `pandas-data-cleaning`, 
  not `course-1-week-3`)
- **Per-project README** answers three questions:
  1. What was the prompt?
  2. What did I build?
  3. What did I learn that I'll actually use?
- **notes.md** is for the honest version: where the guided path felt limiting, 
  what I extended on my own, what broke.
- **Starter code attribution**: Guided projects often provide a scaffold to build 
  on. Where that applies, the project README includes the line *"Starter scaffold 
  provided by Coursera; modifications and extensions are mine."* Projects built 
  entirely from scratch omit the line.
- **Certificates**: Stored as PDFs in `/certificates/`, named with the same slug 
  as the project they correspond to. Each project README links to its certificate 
  when one exists.

```
Index

| Project | Type | Stack | Status |
|---------|------|-------|--------|
| _populated as projects land_ | | | |
```

Licensing

Code in this repository is released under the [Apache License 2.0](LICENSE). 
Course-provided starter code, datasets, and assignment prompts remain the 
property of Coursera and the originating institutions; nothing proprietary 
is reproduced here.

Why this repo exists

Guided projects are short and easy to lose track of. Capstones deserve more 
visibility than a buried certificate page. This is the durable record.
