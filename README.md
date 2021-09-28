# k8s-application-observer

## Architecture

Each `Observer` can have any number of `Monitor`s associated with it.

Each `Monitor` is defined in relation to a data source. This can be things like Prometheus, New Relic, Datadog, etc. A Monitor defines a MELT (Metric/Event/Log/Transaction) data point, and (depending on data type) a threshold, filter, etc to watch.

Each `Monitor` is then associated with any number of `Action`s
