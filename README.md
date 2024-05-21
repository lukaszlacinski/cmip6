# CMIP6 Extension Specification

- **Title:** CMIP6
- **Identifier:** <https://cedadev.github.io/cmip6/v0.1.0/schema.json>
- **Field Name Prefix:** cmip6
- **Scope:** Item
- **Extension [Maturity Classification](https://github.com/radiantearth/stac-spec/tree/master/extensions/README.md#extension-maturity):** Proposal
- **Owner**: @nmassey001 @rhys.r.evans3

This document explains the CMIP6 Extension to the
[SpatioTemporal Asset Catalog](https://github.com/radiantearth/stac-spec) (STAC) specification.

This extension specifies a set of properties for the Coupled Model Intercomparison Project Phase 6 (CMIP6)
prefixed with `cmip6`.

- Examples:
  - [Item: CMIP6](examples/CMIP6.ScenarioMIP.UA.MCM-UA-1-0.ssp245.r1i1p1f2.Amon.psl.gn.v20190731.json)
- [JSON Schema](json-schema/schema.json)
- [Changelog](./CHANGELOG.md)

## Fields

The fields in the table below can be used in these parts of STAC documents:

- [ ] Catalogs
- [ ] Collections
- [x] Item Properties (incl. Summaries in Collections)
- [ ] Assets (for both Collections and Items, incl. Item Asset Definitions in Collections)
- [ ] Links

| Field Name               | Type    | Description                                                                                                               |
|--------------------------|---------|---------------------------------------------------------------------------------------------------------------------------|
| cmip6:access             | array   | e.g. `["HTTPServer"]`                                                                                                     |
| cmip6:index_node         | string  | e.g. `null`                                                                                                               |
| cmip6:latest             | boolean | e.g. `true`                                                                                                               |
| cmip6:pid                | string  | e.g. `null`                                                                                                               |
| cmip6:replica            | boolean | e.g. `false`                                                                                                              |
| cmip6:retracted          | boolean | e.g. `false`                                                                                                              |
| cmip6:instance_id        | string  | e.g. `CMIP6.ScenarioMIP.UA.MCM-UA-1-0.ssp245.r1i1p1f2.Amon.psl.gn.v20190731`                                              |
| cmip6:citation_url       | string  | e.g. `http://cera-www.dkrz.de/WDCC/meta/CMIP6/CMIP6.ScenarioMIP.UA.MCM-UA-1-0.ssp245.r1i1p1f2.Amon.psl.gn.v20190731.json` |
| cmip6:variable_long_name | string  | e.g. `Sea Level Pressure`                                                                                                 |
| cmip6:variable_units     | string  | e.g. `Pa`                                                                                                                 |
| cmip6:cf_standard_name   | string  | e.g. `air_pressure_at_mean_sea_level`                                                                                     |
| cmip6:activity_id        | string  | e.g. `ScenarioMIP`                                                                                                        |
| cmip6:data_specs_version | string  | e.g. `01.00.28`                                                                                                           |
| cmip6:experiment_title   | string  | e.g. `update of RCP4.5 based on SSP2`                                                                                     |
| cmip6:frequency          | string  | e.g. `mon`                                                                                                                |
| cmip6:further_info_url   | string  | e.g. `https://furtherinfo.es-doc.org/CMIP6.UA.MCM-UA-1-0.ssp245.none.r1i1p1f2`                                            |
| cmip6:grid               | string  | e.g. `lat-lon`                                                                                                            |
| cmip6:grid_label         | string  | e.g. `gn`                                                                                                                 |
| cmip6:institution_id     | string  | e.g. `UA`                                                                                                                 |
| cmip6:mip_era            | string  | e.g. `CMIP6`                                                                                                              |
| cmip6:source_id          | string  | e.g. `MCM-UA-1-0`                                                                                                         |
| cmip6:source_type        | string  | e.g. `AOGCM`                                                                                                              |
| cmip6:experiment_id      | string  | e.g. `ssp245`                                                                                                             |
| cmip6:sub_experiment_id  | string  | e.g. `none`                                                                                                               |
| cmip6:nominal_resolution | string  | e.g. `250 km`                                                                                                             |
| cmip6:table_id           | string  | e.g. `Amon`                                                                                                               |
| cmip6:variable_id        | string  | e.g. `psl`                                                                                                                |
| cmip6:variant_label      | string  | e.g. `r1i1p1f2`                                                                                                           |
| cmip6:levels             | string  | e.g. `null`                                                                                                               |
| cmip6:updated            | string  | e.g. `2024-02-20T19:28:19.804842Z`                                                                                        |
| cmip6:created            | string  | e.g. `2024-02-20T19:28:19.804842Z`                                                                                        |

### Additional Field Information

#### cmip6:access
...

#### cmip6:index_node
...

#### cmip6:latest
...

#### cmip6:pid
...

#### cmip6:replica
...

#### cmip6:retracted
...

#### cmip6:instance_id
...

#### cmip6:citation_url
...

#### cmip6:variable_long_name
...

#### cmip6:variable_units
...

#### cmip6:cf_standard_name
...

#### cmip6:activity_id
...

#### cmip6:data_specs_version
...

#### cmip6:experiment_title
...

#### cmip6:frequency
...

#### cmip6:further_info_url
...

#### cmip6:grid
...

#### cmip6:grid_label
...

#### cmip6:institution_id
...

#### cmip6:mip_era
...

#### cmip6:source_id
...

#### cmip6:source_type
...

#### cmip6:experiment_id
...

#### cmip6:sub_experiment_id
...

#### cmip6:nominal_resolution
...

#### cmip6:table_id
...

#### cmip6:variable_id
...

#### cmip6:variant_label
...

#### cmip6:levels
...

#### cmip6:updated
...

#### cmip6:created
...

## Contributing
...

All contributions are subject to the
[STAC Specification Code of Conduct](https://github.com/radiantearth/stac-spec/blob/master/CODE_OF_CONDUCT.md).
For contributions, please follow the
[STAC specification contributing guide](https://github.com/radiantearth/stac-spec/blob/master/CONTRIBUTING.md) Instructions
for running tests are copied here for convenience.

### Running tests

The same checks that run as checks on PR's are part of the repository and can be run locally to verify that changes are valid. 
To run tests locally, you'll need `npm`, which is a standard part of any [node.js installation](https://nodejs.org/en/download/).

First you'll need to install everything with npm once. Just navigate to the root of this repository and on 
your command line run:
```bash
npm install
```

Then to check markdown formatting and test the examples against the JSON schema, you can run:
```bash
npm test
```

This will spit out the same texts that you see online, and you can then go and fix your markdown or examples.

If the tests reveal formatting problems with the examples, you can fix them with:
```bash
npm run format-examples
```
