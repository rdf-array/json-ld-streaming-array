# json-ld-streaming-array: the JSON-LD streaming test suite for rdf-array

This fork of [w3c/json-ld-streaming](https://github.com/w3c/json-ld-streaming) carries the streaming
toRdf suite with its expectations rewritten for [rdf-array](https://github.com/rdf-array/rdf-array): a
JSON-LD `@list` is one sequence term and there are no `rdf:first`/`rdf:rest` ladders. Each expected
N-Quads file with a ladder was folded into sequences and had to agree with what
jsonld-streaming-parser-array reads from the input, in its streaming profile; all 23 do except `#tdi03`,
whose disagreement is the parser's handling of `@direction` in a list, not the list itself. Each
changed entry carries an `"rdfArrayNote"`. Branch `rdf-sequences`; tests at
<https://rdf-array.github.io/json-ld-streaming-array/tests/>. The method is that of
[json-ld-api-array](https://github.com/rdf-array/json-ld-api-array/blob/rdf-sequences/doc/rdf-array.md).

| Manifest | Test | File | Change |
|---|---|---|---|
| stream-toRdf-manifest.jsonld | `#t0013` | [0013-out.nq](../tests/stream-toRdf/0013-out.nq) | `@list` → sequence in the expected N-Quads |
| stream-toRdf-manifest.jsonld | `#t0014` | [0014-out.nq](../tests/stream-toRdf/0014-out.nq) | `@list` → sequence in the expected N-Quads |
| stream-toRdf-manifest.jsonld | `#t0015` | [0015-out.nq](../tests/stream-toRdf/0015-out.nq) | `@list` → sequence in the expected N-Quads |
| stream-toRdf-manifest.jsonld | `#t0025` | [0025-out.nq](../tests/stream-toRdf/0025-out.nq) | `@list` → sequence in the expected N-Quads |
| stream-toRdf-manifest.jsonld | `#t0036` | [0036-out.nq](../tests/stream-toRdf/0036-out.nq) | `@list` → sequence in the expected N-Quads |
| stream-toRdf-manifest.jsonld | `#tdi03` | [di03-out.nq](../tests/stream-toRdf/di03-out.nq) | `@list` → sequence in the expected N-Quads |
| stream-toRdf-manifest.jsonld | `#te004` | [e004-out.nq](../tests/stream-toRdf/e004-out.nq) | `@list` → sequence in the expected N-Quads |
| stream-toRdf-manifest.jsonld | `#te015` | [e015-out.nq](../tests/stream-toRdf/e015-out.nq) | `@list` → sequence in the expected N-Quads |
| stream-toRdf-manifest.jsonld | `#te016` | [e016-out.nq](../tests/stream-toRdf/e016-out.nq) | `@list` → sequence in the expected N-Quads |
| stream-toRdf-manifest.jsonld | `#te023` | [e023-out.nq](../tests/stream-toRdf/e023-out.nq) | `@list` → sequence in the expected N-Quads |
| stream-toRdf-manifest.jsonld | `#te027` | [e027-out.nq](../tests/stream-toRdf/e027-out.nq) | `@list` → sequence in the expected N-Quads |
| stream-toRdf-manifest.jsonld | `#te029` | [e029-out.nq](../tests/stream-toRdf/e029-out.nq) | `@list` → sequence in the expected N-Quads |
| stream-toRdf-manifest.jsonld | `#te062` | [e062-out.nq](../tests/stream-toRdf/e062-out.nq) | `@list` → sequence in the expected N-Quads |
| stream-toRdf-manifest.jsonld | `#tli01` | [li01-out.nq](../tests/stream-toRdf/li01-out.nq) | `@list` → sequence in the expected N-Quads |
| stream-toRdf-manifest.jsonld | `#tli02` | [li02-out.nq](../tests/stream-toRdf/li02-out.nq) | `@list` → sequence in the expected N-Quads |
| stream-toRdf-manifest.jsonld | `#tli03` | [li03-out.nq](../tests/stream-toRdf/li03-out.nq) | `@list` → sequence in the expected N-Quads |
| stream-toRdf-manifest.jsonld | `#tli04` | [li04-out.nq](../tests/stream-toRdf/li04-out.nq) | `@list` → sequence in the expected N-Quads |
| stream-toRdf-manifest.jsonld | `#tli05` | [li05-out.nq](../tests/stream-toRdf/li05-out.nq) | `@list` → sequence in the expected N-Quads |
| stream-toRdf-manifest.jsonld | `#tli06` | [li06-out.nq](../tests/stream-toRdf/li06-out.nq) | `@list` → sequence in the expected N-Quads |
| stream-toRdf-manifest.jsonld | `#tli07` | [li07-out.nq](../tests/stream-toRdf/li07-out.nq) | `@list` → sequence in the expected N-Quads |
| stream-toRdf-manifest.jsonld | `#tli08` | [li08-out.nq](../tests/stream-toRdf/li08-out.nq) | `@list` → sequence in the expected N-Quads |
| stream-toRdf-manifest.jsonld | `#tli09` | [li09-out.nq](../tests/stream-toRdf/li09-out.nq) | `@list` → sequence in the expected N-Quads |
| stream-toRdf-manifest.jsonld | `#tli10` | [li10-out.nq](../tests/stream-toRdf/li10-out.nq) | `@list` → sequence in the expected N-Quads |
