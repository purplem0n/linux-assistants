# Linux Assistants

Agent skills for Linux distribution assistance. Each skill helps an AI assist with a specific distro: package management, system diagnosis, scripting, and troubleshooting.

## Available skills

- **CachyOS** — Arch-based; pacman, CachyOS repos and kernels (BORE/EEVDF/BMQ), systemd, performance tuning. See [skills/cachyos/SKILL.md](skills/cachyos/SKILL.md).

## How multiple skills are added

Each distro is one skill. Add a **directory per distro** with a `SKILL.md` inside:

```
skills/
├── cachyos/
│   └── SKILL.md
├── fedora/
│   └── SKILL.md
└── ubuntu/
    └── SKILL.md
```

CachyOS lives at `skills/cachyos/SKILL.md`. Add new distro skills under `skills/<distro>/SKILL.md`.

## More distros coming

Additional distro assistant skills (e.g. Fedora, Ubuntu, openSUSE, NixOS) are planned. Check back for updates or [contribute](#contributing) your own.

## Contributing

Contributions are welcome. You can:

- **Add a distro skill** — Create `skills/<distro>/SKILL.md` (e.g. `skills/fedora/SKILL.md`) following the structure of [skills/cachyos/SKILL.md](skills/cachyos/SKILL.md): when to use the skill, core principles, package management, scripts, and diagnosis/troubleshooting guidance.
- **Improve existing skills** — Open an issue or pull request to refine docs, add commands, or fix inaccuracies.

Include a clear frontmatter `name` and `description` in each SKILL.md so the skill is discoverable. When in doubt, open an issue to discuss before sending a large PR.

## License

See [LICENSE](LICENSE).
