# Homebrew tap for chumux

chumux is a project sidebar and agent dashboard for tmux sessions: tmux keeps
owning every shell, editor and agent, and chumux is the window over them.

```sh
brew install --cask chucheloff/chumux/chumux
brew update && brew upgrade --cask chumux
```

The cask installs `chumux.app` for macOS on Apple Silicon (macOS 12 or later).
Releases are built and signed ad hoc on a Mac, not notarized; the cask clears
the quarantine flag after installing so Gatekeeper opens the app.

To replace a `chumux.app` that was installed by other means, add `--force` to
`brew install`. Upgrading replaces only the app bundle. A running chumux keeps
running until it is restarted, and the tmux sessions keep running too.

`Casks/chumux.rb` and the release zips here are published by the chumux release
script; do not edit the cask by hand.
