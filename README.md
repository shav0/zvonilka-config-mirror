# zvonilka-config-mirror

Public mirror of Zvonilka's signed transport config, published automatically
by `tools/admin-cli publish-config` (in the main
[zvonilka](https://github.com/shav0/zvonilka) repo) whenever the server list
changes.

`transport-config.json` in this repo is a `{payload, signature}` envelope
signed with the family admin's Ed25519 key. Clients verify that signature
themselves before trusting anything here — this repo (like the R2 mirror) is
just a fallback delivery path for when the primary relay isn't reachable, not
a trust boundary.
