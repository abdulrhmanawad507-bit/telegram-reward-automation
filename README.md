name: Reward Check Test

'on':
  schedule:
    - cron: "0 * * * *"
  workflow_dispatch:

jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - name: Test cloud operation
        run: |
          echo "Cloud workflow is running"
          date -u
