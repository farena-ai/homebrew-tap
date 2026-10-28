# farena-ai/homebrew-tap

Homebrew tap for [Sara](https://github.com/farena-ai/sara), a self-hosted AI companion and coding
partner. The cask installs the signed and notarized Mac app from Sara's GitHub Releases.

```sh
brew install --cask farena-ai/tap/sara
```

Update with `brew upgrade --cask sara` (the app also tells you when a new release is out). Remove
with `brew uninstall --cask sara`; `brew uninstall --zap --cask sara` also deletes her data
(memories, keys, chats), so make a backup first (`sara backup`).

`Casks/sara.rb` is made in Sara's repository (`packaging/homebrew/sara.rb`, filled by
`scripts/update-packaging.ts` from each release's `SHA256SUMS`) and copied here at each release.
Problems: https://github.com/farena-ai/sara/issues
