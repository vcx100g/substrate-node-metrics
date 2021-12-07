# Node metrics report 

`https://docs.substrate.io/tutorials/v3/node-metrics/`

start substrate node
```shell
# clear the dev database
./target/release/node-template purge-chain --dev -y
# start the template node  in dev & tmp mode to experiment
# optionally add the `--prometheus-port <PORT>`
# or `--prometheus-external` flags
./target/release/node-template --dev
```

## prometheus
download prometheus
`https://prometheus.io/download/`

start prometheus with prometheus.yml
```shell
$ ./prometheus --config.file ../prometheus.yml
```

## grafana

download grafana
`https://grafana.com/grafana/download`

start grafana
```shell
$ ./bin/grafana-server
```

set datasource in grafana to prometheus

load dashboard json file and done
`create > import`