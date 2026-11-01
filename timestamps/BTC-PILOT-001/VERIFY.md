# Verify the unchanged packet and timestamp

From the repository root:

```bash
(cd packets && sha256sum -c BTC-PILOT-001-2026-11-01.zip.sha256)
openssl ts -verify -data packets/BTC-PILOT-001-2026-11-01.zip -in timestamps/BTC-PILOT-001/batch.tsr -CAfile timestamps/BTC-PILOT-001/cacert.pem -untrusted timestamps/BTC-PILOT-001/tsa.crt
openssl ts -reply -in timestamps/BTC-PILOT-001/batch.tsr -text
```

Expected packet SHA-256:

`ca65ba4ec2f30f3305dec477f2c5f462cb775e6dd5d4c0ae8b41f5824fd17e9e`

Expected service-asserted time: 2026-11-01T12:24:34Z. The signature is from FreeTSA
and is verified against FreeTSA's own supplied trust anchor. Trust in the provider,
its key and clock remains a condition; universal or qualified legal trust is not
claimed. This proof establishes the hash/time binding, not accuracy, originality,
an earlier public seal or OSF registration. The original packet must remain available.

The JSON receipt retains original local custody paths. Those paths are descriptive;
the signed hash is independent of the file's later hosting location.
