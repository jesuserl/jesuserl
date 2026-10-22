name: Metrics
on:
  schedule:
    - cron: "0 0 * * *" # Se ejecuta todos los días a medianoche
  workflow_dispatch:
jobs:
  github-metrics:
    runs-on: ubuntu-latest
    steps:
      - uses: lowlighter/metrics@latest
        with:
          token: ${{ secrets.METRICS_TOKEN }}
          plugin_activity: yes
          plugin_community: yes
