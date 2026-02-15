# Linux Assistants

Agent skills for Linux distribution assistance. Each skill helps an AI assist with a specific distro: package management, system diagnosis, scripting, and troubleshooting.

## Available skills

- **CachyOS** — Arch-based; pacman, CachyOS repos and kernels (BORE/EEVDF/BMQ), systemd, performance tuning. See [cachyos-linux-assistant/SKILL.md](cachyos-linux-assistant/SKILL.md).

## How multiple skills are added

Each distro is one skill. Add a **directory per distro** (name must match the `name` in SKILL.md frontmatter) with a `SKILL.md` inside. Skills can live at repo root or under a folder like `skills/`; the CLI discovers any directory that contains a valid SKILL.md.

```
cachyos-linux-assistant/
│   └── SKILL.md
fedora-assistant/
│   └── SKILL.md
```

CachyOS lives at `cachyos-linux-assistant/SKILL.md`. Add new distro skills as `<skill-name>/SKILL.md` (e.g. `fedora-assistant/SKILL.md`).

## More distros coming

Additional distro assistant skills (e.g. Fedora, Ubuntu, openSUSE, NixOS) are planned. Check back for updates or [contribute](#contributing) your own.

## Contributing

Contributions are welcome. You can:

- **Add a distro skill** — Create `<skill-name>/SKILL.md` (e.g. `fedora-assistant/SKILL.md`) following the structure of [cachyos-linux-assistant/SKILL.md](cachyos-linux-assistant/SKILL.md): when to use the skill, core principles, package management, scripts, and diagnosis/troubleshooting guidance.
- **Improve existing skills** — Open an issue or pull request to refine docs, add commands, or fix inaccuracies.

Include a clear frontmatter `name` and `description` in each SKILL.md so the skill is discoverable. When in doubt, open an issue to discuss before sending a large PR.

## License

See [LICENSE](LICENSE).
