# Organization classification

Adds an array of classification objects to an organization's details, in order to categorize it.

## Legal context

In the European Union, this extension's fields correspond to [eForms BT-10 (Activity Authority). BT-610 (Activity Entity), and BT-740 (Buyer Contracting Entity)](https://docs.ted.europa.eu/eforms/latest/reference/business-terms/). For correspondences to eForms fields, see [OCDS for eForms](https://standard.open-contracting.org/profiles/eforms/).

## Examples

```json
{
  "parties": [
    {
      "id": "1",
      "details": {
        "classifications": [
          {
            "id": "10",
            "scheme": "TED_CA_ACTIVITY",
            "description": "Social protection"
          }
        ]
      }
    }
  ]
}
```

## Versions

Use the following extension URL for different versions of OCDS:

* 1.2: https://raw.githubusercontent.com/open-contracting-extensions/ocds_organizationClassification_extension/1.2/extension.json
* 1.1: https://raw.githubusercontent.com/open-contracting-extensions/ocds_organizationClassification_extension/1.1/extension.json

## Issues

Report issues for this extension in the [ocds-extensions repository](https://github.com/open-contracting/ocds-extensions/issues), putting the extension's name in the issue's title.

## Changelog

### 2023-04-05

* Add 'buyer-contracting-type' and 'Directive 2014/25/EU' to the `+itemClassificationScheme.csv` codelist.

### 2021-02-15

* [#1157](https://github.com/open-contracting/standard/issues/1157) Move the COFOG code from the `+itemClassificationScheme.csv` codelist to the standard.

### 2020-04-24

* Add `minProperties`, `minItems` and/or `minLength` properties.

This extension was originally discussed as part of the [OCDS for EU profile](https://github.com/open-contracting-extensions/european-union/issues), in [pull requests](https://github.com/open-contracting-extensions/ocds_organizationClassification_extension/pulls?q=is%3Apr+is%3Aclosed) and in <https://github.com/open-contracting/standard/issues/711>.
