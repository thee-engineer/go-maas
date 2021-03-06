# Golang MAAS API


[NASA](https://www.nasa.gov)'s Mars Atmospheric Aggregation System (MAAS) Golang API

[![Go Report Card](https://goreportcard.com/badge/github.com/thee-engineer/go-maas)](https://goreportcard.com/report/github.com/thee-engineer/go-maas)

- [Golang MAAS API](#golang-maas-api)
    - [CAB Disclaimer](#cab-disclaimer)
    - [API](#api)
    - [Dashboard](#dashboard)

## [CAB](http://www.cab.inta.es/en/inicio) Disclaimer

The information contained into this file is provided by Centro de Astrobiologia (CAB) and is intended for outreach purposes only. Any other use is discouraged. CAB will take no responsibility for any result or publication made base on the content of this file. To access REMS scientific data, visit [PDS](http://pds.nasa.gov). The environmental magnitudes given into this file are obtained from the values read by the Rover Environmental Monitoring Station (REMS) on board the Mars Science Laboratory (MSL) rover on Mars. This file provides the environmental magnitudes at REMS location, so MSL rover influences those magnitudes (rover position, rover temperature, rover orientation, rover shade, dust depositions on the rover, etc.) REMS does not take measurements continuously and it takes measurements at different times from one day to another. This fact has influence on the variation of the values given in this file from one day to another. For different reasons (instrument maintenance, instrument calibration, instrument degradation, etc.),  some or all of the magnitudes in this file may not be available.

## API

`GET /api/temp`

```json
[
    {
        "min": -50, "max": -20
    },
    {
        "min": -47, "max": -19
    },
    {
        "min": -51, "max": -26
    },
    ...
]
```

`GET /api/temp/max`
`GET /api/temp/min`

```json
[
    -10, -20, -15, -14, -25, ...
]
```

`GET /api/sol/{id}`

`GET /api/date?year={}&month={}&day={}`

## Dashboard
