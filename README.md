# cdxgen-action
action for cdxgen with upload to license server

```
on: [push]

jobs:
  cdxgen:
    runs-on: ubuntu-latest
    name: Generate license information and upload it
    steps:
      - name: Generate license information and upload it
        id: cdxgen
        uses: sorenmat/cdxgen-action@main
        with:
          server-url: 'http://localhost/api/v1/bom'
          fetch-licenses: true
          token: '1234'

```
