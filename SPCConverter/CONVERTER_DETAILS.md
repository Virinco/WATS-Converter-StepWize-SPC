# Technical Details: StepWize SPC

## Overview

Converts StepWize SaaS platform XSPC test result files to WATS UUT reports.

## File Format Assumptions and Requirements

- Input encoding: UTF-8
- XML format with `ConfigAndResultsDataFile/ConfigandResultsData/Config_and_Result_Data/Config_and_Data_Result` structure
- `dataType` values: `0` = Numeric, `1` = Action/PassFail, `2` = Generic Action step
- Date format: `yyyy-MM-ddTHH:mm:ss.fff`

## Converter Parameter Details

| Parameter | Default | Effect |
|-----------|---------|--------|
| `operator` | `oper` | Default operator name if not provided by the input file |
| `sequenceVersion` | `1.0.0` | Sequence version used for imported reports |
| `operationTypeCode` | `10` | Operation type code for imported reports |

## Change History

See [CHANGELOG.md](CHANGELOG.md) for version history.
