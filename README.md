<p align="center">
  <img src="./github-metrics.svg" alt="Metrics" width="80%" />
</p>

name: Most used (with details)
uses: lowlighter/metrics@latest
with:
  filename: metrics.plugin.languages.details.svg
  token: ${{ secrets.METRICS_TOKEN }}
  base: ""
  plugin_languages: yes
  plugin_languages_ignored: >-
    html, css, tex, less, dockerfile, makefile, qmake, lex, cmake, shell,
    gnuplot
  plugin_languages_details: bytes-size, percentage
  plugin_languages_limit: 4
