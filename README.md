# Published artifacts

Machine-written. `blocklist.json`, `backend.json`, `threadsmod-update.json`
and `blocklist/v3/manifest.json` are signed; clients verify them against a key
compiled into them, so this mirror cannot change what anybody blocks or
installs. Everything under `blocklist/v3/objects/` is named by the SHA-256 of
its bytes and is bound to the signed root, so it cannot be substituted either.
Do not edit by hand -- the signature would stop verifying and clients would
ignore the file.
