Vendored from `samoshkin/tmux-plugin-sysstat` at commit
`29e150f403151f2341f3abcb2b2487a5f011dd23`.

Local changes:

- Fix the inverted `vmstat` availability check in `scripts/cpu_collect.sh`.
  Linux and FreeBSD now use the lightweight `vmstat` collector when it is
  installed and fall back to `top` only when it is unavailable.
