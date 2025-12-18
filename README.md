# kubemind

## Installation

```sh
helm install kubemind oci://ghcr.io/mikolajsemeniuk/charts/kubemind \
  --version 0.1.0 \
  -n kubemind-system --create-namespace
```

## Installation Locally

```sh
helm install kubemind charts/kubemind -n kubemind-system --create-namespace
```

## Context

Chciałbym zrobić aplikację używając operatora Kubernetes która będzie się nazywała kubemind. Aplikacja ma przy użyciu operatora śledzić stan klastra ale też później może innych zasobów takich jak confluence, JIRA etc. Celem aplikacji jest hostowanie bazy wektorowej oraz modelu AI oraz jakiegoś daemon seta czy innego programu który monitoruje stan klastra i w razie jakiegoś outage, lub dokonania jakiejść zmiany ma posiadać wiedzę plemnienną i zamiast pytać się innych pracowników lub tracić wiedzę kiedy pracownicy odchodzą lub przy outagu ma ci powiedzieć gdzie najlepiej zacząć szukać infomacji albo gdzie najlepiej zacząć.

Na razie zrobiłem prosty operator z jednym komponentem oraz helmem do pobrania + obraz dockerowy hostowany na GH, chcę rozwijać to dalej.
