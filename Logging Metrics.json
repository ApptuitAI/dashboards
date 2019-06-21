{
  "__inputs": [
    {
      "name": "DS_APPTUIT-PROMQL",
      "label": "Apptuit-PromQL",
      "description": "",
      "type": "datasource",
      "pluginId": "prometheus",
      "pluginName": "Prometheus"
    },
    {
      "name": "VAR_GTS",
      "type": "constant",
      "label": "Global Tagset",
      "value": "$jinsight",
      "description": ""
    },
    {
      "name": "VAR_SCRAPE_INTERVAL",
      "type": "constant",
      "label": "scrape_interval",
      "value": "15s",
      "description": ""
    }
  ],
  "__requires": [
    {
      "type": "grafana",
      "id": "grafana",
      "name": "Grafana",
      "version": "5.4.3"
    },
    {
      "type": "panel",
      "id": "graph",
      "name": "Graph",
      "version": "5.0.0"
    },
    {
      "type": "datasource",
      "id": "prometheus",
      "name": "Prometheus",
      "version": "5.0.0"
    }
  ],
  "annotations": {
    "list": []
  },
  "editable": true,
  "gnetId": null,
  "graphTooltip": 0,
  "id": null,
  "iteration": 1560936890739,
  "links": [],
  "panels": [
    {
      "aliasColors": {},
      "bars": false,
      "dashLength": 10,
      "dashes": false,
      "datasource": "${DS_APPTUIT-PROMQL}",
      "fill": 1,
      "gridPos": {
        "h": 7,
        "w": 24,
        "x": 0,
        "y": 0
      },
      "id": 1,
      "interval": "$scrape_interval",
      "legend": {
        "alignAsTable": true,
        "avg": false,
        "current": true,
        "max": true,
        "min": true,
        "rightSide": true,
        "show": true,
        "sort": "max",
        "sortDesc": true,
        "total": false,
        "values": true
      },
      "lines": true,
      "linewidth": 1,
      "links": [],
      "nullPointMode": "null",
      "percentage": false,
      "pointradius": 5,
      "points": false,
      "renderer": "flot",
      "seriesOverrides": [],
      "spaceLength": 10,
      "stack": false,
      "steppedLine": false,
      "targets": [
        {
          "expr": "sum by (level) (delta(logger_appends_total{$global_tag_filter}[$__interval]))",
          "format": "time_series",
          "intervalFactor": 1,
          "legendFormat": "{{level}}",
          "metrics": [],
          "refId": "A",
          "ts": {
            "alias": "A:$t(cloud_service) : $t(level)",
            "errors": [],
            "id": "A",
            "output": true,
            "query": "logger_appends"
          },
          "type": "Query"
        }
      ],
      "thresholds": [],
      "timeFrom": null,
      "timeRegions": [],
      "timeShift": null,
      "title": "Logging Rate",
      "tooltip": {
        "shared": true,
        "sort": 0,
        "value_type": "individual"
      },
      "type": "graph",
      "xaxis": {
        "buckets": null,
        "mode": "time",
        "name": null,
        "show": true,
        "values": []
      },
      "yaxes": [
        {
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": "0",
          "show": true
        },
        {
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        }
      ],
      "yaxis": {
        "align": false,
        "alignLevel": null
      }
    },
    {
      "aliasColors": {},
      "bars": false,
      "dashLength": 10,
      "dashes": false,
      "datasource": "${DS_APPTUIT-PROMQL}",
      "fill": 1,
      "gridPos": {
        "h": 7,
        "w": 24,
        "x": 0,
        "y": 7
      },
      "id": 2,
      "interval": "$scrape_interval",
      "legend": {
        "alignAsTable": true,
        "avg": false,
        "current": true,
        "max": true,
        "min": true,
        "rightSide": true,
        "show": true,
        "sort": "max",
        "sortDesc": true,
        "total": false,
        "values": true
      },
      "lines": true,
      "linewidth": 1,
      "links": [],
      "nullPointMode": "null",
      "percentage": false,
      "pointradius": 5,
      "points": false,
      "renderer": "flot",
      "seriesOverrides": [],
      "spaceLength": 10,
      "stack": false,
      "steppedLine": false,
      "targets": [
        {
          "expr": "sum by(instance) (delta(logger_throwables_total{$global_tag_filter}[$__interval]))",
          "format": "time_series",
          "intervalFactor": 1,
          "legendFormat": "$global_legend",
          "metrics": [],
          "refId": "A",
          "ts": {
            "alias": "A: $t(cloud_service)",
            "errors": [],
            "id": "A",
            "output": true,
            "query": ""
          },
          "type": "Query"
        }
      ],
      "thresholds": [],
      "timeFrom": null,
      "timeRegions": [],
      "timeShift": null,
      "title": "Throwables logged",
      "tooltip": {
        "shared": true,
        "sort": 0,
        "value_type": "individual"
      },
      "type": "graph",
      "xaxis": {
        "buckets": null,
        "mode": "time",
        "name": null,
        "show": true,
        "values": []
      },
      "yaxes": [
        {
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        },
        {
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        }
      ],
      "yaxis": {
        "align": false,
        "alignLevel": null
      }
    },
    {
      "aliasColors": {},
      "bars": false,
      "dashLength": 10,
      "dashes": false,
      "datasource": "${DS_APPTUIT-PROMQL}",
      "fill": 1,
      "gridPos": {
        "h": 7,
        "w": 24,
        "x": 0,
        "y": 14
      },
      "id": 3,
      "legend": {
        "alignAsTable": true,
        "avg": false,
        "current": true,
        "hideEmpty": true,
        "hideZero": true,
        "max": true,
        "min": true,
        "rightSide": true,
        "show": true,
        "sort": "max",
        "sortDesc": true,
        "total": false,
        "values": true
      },
      "lines": true,
      "linewidth": 1,
      "links": [],
      "nullPointMode": "null",
      "percentage": false,
      "pointradius": 5,
      "points": false,
      "renderer": "flot",
      "seriesOverrides": [],
      "spaceLength": 10,
      "stack": false,
      "steppedLine": false,
      "targets": [
        {
          "expr": "sum by(class) (delta(logger_throwables_total{$global_tag_filter}[$__interval]))",
          "format": "time_series",
          "interval": "",
          "intervalFactor": 1,
          "legendFormat": "{{class}}",
          "metrics": [],
          "refId": "A",
          "ts": {
            "alias": "e:$t(cloud_service)-$t(class)",
            "errors": [],
            "id": "A",
            "output": true,
            "query": "logger_throwabl.count"
          },
          "type": "Query"
        }
      ],
      "thresholds": [],
      "timeFrom": null,
      "timeRegions": [],
      "timeShift": null,
      "title": "Exception Class Metrics",
      "tooltip": {
        "shared": true,
        "sort": 0,
        "value_type": "individual"
      },
      "type": "graph",
      "xaxis": {
        "buckets": null,
        "mode": "time",
        "name": null,
        "show": true,
        "values": []
      },
      "yaxes": [
        {
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        },
        {
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        }
      ],
      "yaxis": {
        "align": false,
        "alignLevel": null
      }
    }
  ],
  "refresh": false,
  "schemaVersion": 16,
  "style": "dark",
  "tags": [
    "jinsight"
  ],
  "templating": {
    "list": [
      {
        "current": {
          "value": "${VAR_GTS}",
          "text": "${VAR_GTS}"
        },
        "hide": 2,
        "isGlobal": false,
        "label": "Global Tagset",
        "name": "gts",
        "options": [
          {
            "value": "${VAR_GTS}",
            "text": "${VAR_GTS}"
          }
        ],
        "query": "${VAR_GTS}",
        "refresh": 0,
        "skipUrlSync": true,
        "type": "constant"
      },
      {
        "current": {
          "value": "${VAR_SCRAPE_INTERVAL}",
          "text": "${VAR_SCRAPE_INTERVAL}"
        },
        "hide": 0,
        "isGlobal": false,
        "label": null,
        "name": "scrape_interval",
        "options": [
          {
            "value": "${VAR_SCRAPE_INTERVAL}",
            "text": "${VAR_SCRAPE_INTERVAL}"
          }
        ],
        "query": "${VAR_SCRAPE_INTERVAL}",
        "refresh": 0,
        "skipUrlSync": false,
        "type": "constant"
      }
    ]
  },
  "time": {
    "from": "now-3h",
    "to": "now"
  },
  "timepicker": {
    "refresh_intervals": [
      "5s",
      "10s",
      "30s",
      "1m",
      "5m",
      "15m",
      "30m",
      "1h",
      "2h",
      "1d"
    ],
    "time_options": [
      "5m",
      "15m",
      "1h",
      "6h",
      "12h",
      "24h",
      "2d",
      "7d",
      "30d"
    ]
  },
  "timezone": "",
  "title": "Prometheus Logging Metrics",
  "uid": "TMMnLoqmk",
  "version": 1
}