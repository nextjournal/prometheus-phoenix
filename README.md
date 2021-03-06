# Prometheus.io Phoenix Instrumenter
[![Hex.pm](https://img.shields.io/hexpm/v/prometheus_phoenix.svg?maxAge=2592000)](https://hex.pm/packages/prometheus_phoenix)
[![Hex.pm](https://img.shields.io/hexpm/dt/prometheus_phoenix.svg?maxAge=2592000)](https://hex.pm/packages/prometheus_phoenix)
[![Build Status](https://travis-ci.org/deadtrickster/prometheus-phoenix.svg?branch=master)](https://travis-ci.org/deadtrickster/prometheus-phoenix)
[![Documentation](https://img.shields.io/badge/documentation-on%20hexdocs-green.svg)](https://hexdocs.pm/prometheus_phoenix/)

Phoenix integeration for [Prometheus.ex](https://github.com/deadtrickster/prometheus.ex).

 - IRC: #elixir-lang on Freenode;
 - [Slack](https://elixir-slackin.herokuapp.com/): #prometheus channel - [Browser](https://elixir-lang.slack.com/messages/prometheus) or App(slack://elixir-lang.slack.com/messages/prometheus).

## Metrics

 - `phoenix_controller_call_duration_microseconds` - Whole controller pipeline execution time.

## Configuration

This integartion is configured via <InstrumenterName> `:prometheus` app env key. Please see `Prometheus.PhoenixInstrumenter` module documentation for more information.

## Integrations / Collectors / Instrumenters
 - [Ecto collector](https://github.com/deadtrickster/prometheus-ecto)
 - [Plugs Instrumenter/Exporter](https://github.com/deadtrickster/prometheus-plugs)
 - [Elli middleware](https://github.com/elli-lib/elli_prometheus)
 - [Fuse plugin](https://github.com/jlouis/fuse#fuse_stats_prometheus)
 - [Phoenix instrumenter](https://github.com/deadtrickster/prometheus-phoenix)
 - [Process Info Collector](https://github.com/deadtrickster/prometheus_process_collector.erl)
 - [RabbitMQ Exporter](https://github.com/deadtrickster/prometheus_rabbitmq_exporter)

## Installation

[Available in Hex](https://hex.pm/packages/prometheus_phoenix/), the package can be installed as:

  1. Add `prometheus_phoenix` to your list of dependencies in `mix.exs`:

    ```elixir
    def deps do
      [{:prometheus_phoenix, "~> 1.0.1"}]
    end
    ```

  2. Ensure `prometheus_phoenix` is started before your application:

    ```elixir
    def application do
      [applications: [:prometheus_phoenix]]
    end
    ```

