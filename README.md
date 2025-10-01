# Dataspace Connector

This repo is a copy of [IDS Testbed](https://github.com/International-Data-Spaces-Association/IDS-testbed) and extract connector only to make sure it's fully compatible with the original IDS Testbed.

## Setup
1. First please generate corresponding keys in the original IDS Testbed or an indenpendent CA server. You will need to put `connector.cert`, `connector.key`, `connector.p12` and `truststore.p12` under `certs` folder, replace the existed ones.
2. Update `.env` to set at least `DAPS_SERVER_HOST` to the corresponding server's public IP address. If you are setting up the full IDS Testbed you they should be the same value.
3. Run `docker compose up -d` to run the containers, now you can treat it as a normal connector.