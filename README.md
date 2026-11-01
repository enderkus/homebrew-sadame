# Homebrew tap for sadame

[Sadame](https://github.com/enderkus/sadame) describes the desired state of
Linux machines in plain Ruby, shows every change as a diff before it
happens, and applies it over SSH from a single binary.

```sh
brew install enderkus/sadame/sadame
```

or, to tap first:

```sh
brew tap enderkus/sadame
brew install sadame
```

The formula installs the release binary for your system, macOS (Apple
silicon, Intel) or Linux (x86_64, ARM64), after Homebrew checks it against
the SHA-256 checksum in the formula.

Documentation: <https://enderkus.github.io/sadame/>

## Updating the formula

`Formula/sadame.rb` is written for each release in the main repository by
`rake "packaging[VERSION]"`, from the release's `SHA256SUMS`, as
`homebrew/sadame.rb`. Copy that file here; do not edit it by hand.
