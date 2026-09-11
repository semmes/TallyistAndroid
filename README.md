# Tallyist for Android — public documents

This repository is the public home of the two documents the Android app must
publish at a stable address: its **privacy policy** and its **support page**.
They are served as a site at **<https://semmes.github.io/TallyistAndroid/>**,
and those URLs are the ones registered in Google Play Console and linked from
inside the app.

It exists as a separate repository so that these documents stay publicly
readable, with their full revision history, independently of the app's source
repository, which is private. The privacy policy claims that every change to it
is visible in a public history; keeping that claim true is this repository's
only job.

| Document | Source file | Published at |
| --- | --- | --- |
| Privacy Policy | `privacy-policy.md` | `/TallyistAndroid/privacy/` |
| Support | `support.md` | `/TallyistAndroid/support/` |

The iPhone app is a separate app with its own documents at
<https://semmes.github.io/Tallyist/>, published from
<https://github.com/semmes/Tallyist>. The two policies differ because the two
apps store and move data differently. Neither is a copy of the other.

## Editing

**`privacy-policy.md` and `support.md` in this repository are copies. Do not
edit them here.**

The Android app's source repository holds the canonical versions at
`docs/privacy-policy-android.md` and `docs/support-android.md`, because the
policy's claims are written to be checkable against the app's merged manifest
and its dependency graph, and the support page's answers describe shipping
behaviour. Edits are made there and copied here unchanged, front matter
included.

## Questions

Questions about the Android app, or about these documents, belong in
[Issues](https://github.com/semmes/TallyistAndroid/issues).
