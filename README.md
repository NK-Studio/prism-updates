# prism-updates

The in-app update feed for [Prism](https://github.com/NK-Studio/prism), deployed by Vercel.

**Don't edit by hand.** The *Publish update* workflow in the Prism repository
(`.github/workflows/publish-update.yml`, via `cargo xtask update publish`) writes this
repository and force-pushes it as a single commit:

```text
stable/latest.json            the feed, signed (never cached)
stable/latest.json.minisig    its minisign signature
releases/<version>/           update packages for the newest three versions
```

See `docs/releasing.md` › In-app updates in the Prism repository.
