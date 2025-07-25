nothing fancy — just a clean, static repo with plugin manifests
using sha256 hashes to make sure nothing’s been tampered with.




## how it works

* `main.json` lists all available plugins by ID
* each plugin has its own folder with a `manifest.json`
* the manifest includes a URL to the plugin and its expected sha256 hash
* clients can read the manifest, verify the hash, and load the plugin in a sandbox

all manifests live in this repo — no redirects, no lookups.
no backend. just static JSON files and trust through verification.



## why this exists

we believe plugins should be open, but also safe.
by checking the hash before loading, you avoid surprises.
you can host the actual plugin wherever you want — just match the hash.



## license

MIT — free to use, modify, or fork
no guarantees, and no responsibility for what any plugin does.






made with care by dotpen labs
