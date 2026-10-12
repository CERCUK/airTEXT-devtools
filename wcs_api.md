# WCS API definition

**Base URL:** `https://api.airtext.info`  

---

### ![GET](https://img.shields.io/badge/GET-2ea44f?style=flat-square) /geoserver/london/wcs

Downloads raw airTEXT pollution data for analysis.
The pollutant values are µg/m³ for individual pollutants, or DAQI index for the total coverage.

#### Parameters

| Name | Required | Description |
|------|----------|-------------|
| service  <br /> `string`  | &#10003; | Must be **WCS** |
| version  <br /> `string` | &#10003; | WCS version <br /> `Default: 2.0.0` |
| request  <br /> `string` | &#10003; | Must be **GetCoverage** |
| coverageId  <br /> `string` | &#10003; | Pollutant layer shown <br /> `Available values: NO2, O3, PM10, PM25, Total` |
| format  <br /> `string` | &#10003; | Output format <br /> `Available values: image/tiff, image/png` |
| subset  <br /> `string` | &#10003; | Date and time filter <br /> `Example: time("2026-12-25T00:00:00.000Z")` |
| subset  <br /> `string` | &#10003; | Output geographical area (longitude)  <br /> `Example: Long(-0.12,-0.11)` |
| subset  <br /> `string` | &#10003; | Output geographical area (latitude)  <br /> `Example: Lat(51.51,51.52)` |

#### Example cURL Command

```bash
curl -G 'https://api.airtext.info/geoserver/london/wcs' \
    --data-urlencode 'service=WCS' \
    --data-urlencode 'version=2.0.0' \
    --data-urlencode 'request=GetCoverage' \
    --data-urlencode 'coverageId=NO2' \
    --data-urlencode 'format=image/tiff' \
    --data-urlencode 'subset=Long(-0.12,-0.11)' \
    --data-urlencode 'subset=Lat(51.51,51.52)' \
    --data-urlencode 'subset=time("2026-10-09T00:00:00.000Z")' \
    -o no2.tiff
```

#### Responses

| Status | Description |
|--------|-------------|
| `200` | Payload returned successfully |
| `400` | Bad Request |

---


