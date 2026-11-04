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
`brew install`. Installing over a running chumux quits it, and an upgrade may
do the same, so quit chumux first or open it again afterwards. tmux keeps every
session and process, and chumux reattaches when it starts.

`Casks/chumux.rb` and the release zips here are published by the chumux release
script; do not edit the cask by hand.
