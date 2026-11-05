TensegrityPoseCollector

A tiny prototype demonstrating a workflow: ingest paper URLs / pasted supplement text / uploaded ZIPs, simulate extraction of per-module pose time-series, normalize into a JSON schema, and attach provenance metadata.

This is a front-end-only proof-of-concept. Replace simulated extraction with real PDF/ZIP parsing and repository connectors when expanding.

Usage: open index.html in a browser, paste text or drop a ZIP, press "Extract".

Schema: output JSON has records with fields: id, module_id, times (array), poses (array of {qx,qy,qz,qw or euler}), source {type,origin,filename,extracted_at}.