# Organization classification

Adds an array of classification objects to an organization's details, in order to categorize it.

## Legal context

In the European Union, this extension's fields correspond to [eForms BT-10 (Activity Authority)](https://docs.ted.europa.eu/eforms/latest/reference/business-terms/). For correspondences to eForms fields, see [OCDS for eForms](https://standard.open-contracting.org/profiles/eforms/latest/en/). For correspondences to Tenders Electronic Daily (TED), see [OCDS for the European Union](https://standard.open-contracting.org/profiles/eu/latest/en/).

## Examples

An organization categorized as a Social protection business.

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

An Organization classified as a women-owned small business by the Small Business Administration in the USA.

```json
{
  "parties": [
    {
      "id": "1",
      "details": {
        "classifications": [
          {
            "id": "WOSB",
            "scheme": "USA-SBA",
            "description": "Woman-Owned Small Business",
            "uri": "https://www.ecfr.gov/current/title-13/chapter-I/part-127/subpart-B"
          }
        ]
      }
    }
  ]
}
```

## Issues

Report issues for this extension in the [ocds-extensions repository](https://github.com/open-contracting/ocds-extensions/issues), putting the extension's name in the issue's title.

## Changelog

### 2023-08-01

* Add 'eu-main-activity' and 'eu-buyer-contracting-type' to `+itemClassificationScheme.csv`.

### 2020-04-24

* Add `minProperties`, `minItems` and/or `minLength` properties.

This extension was originally discussed as part of the [OCDS for EU profile](https://github.com/open-contracting-extensions/european-union/issues), in [pull requests](https://github.com/open-contracting-extensions/ocds_organizationClassification_extension/pulls?q=is%3Apr+is%3Aclosed) and in <https://github.com/open-contracting/standard/issues/711>.
