# Upgrade guide

1. Refer to the [changelog](https://github.com/overleaf/toolkit/blob/master/CHANGELOG.md) for any important changes.
   Also note the ShareLaTeX version being used in the latest Overleaf toolkit version.

2. Sync this fork.

3. Merge the `main` into the `selfhosted` branch (ideally in an IDE).

4. Push to the origin.

5. On the server, pull from the origin.

6. Update the version noted in step 1. in [config/version](config/version) and the corresponding (based on the release
   date) image version in the [Docker compose file](docker-compose.yaml).

7. Run
    ```
    ./bin/start
    ```
