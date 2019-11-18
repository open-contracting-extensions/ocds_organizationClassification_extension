# Organization classification

Adds an array of Classification objects to Organization.details in order to categorize organizations.

## Legal context

In the European Union, this extension's fields correspond to [eForms BT-10 (Activity Authority)](https://github.com/eForms/eForms). See [OCDS for the European Union](http://standard.open-contracting.org/profiles/eu/master/en/) for the correspondences to Tenders Electronic Daily (TED).

## Examples

```json
{
  "parties": [
    {
      "id": "1",
      "details": {
        "classifications": [
          {
            "scheme": "TED_CA_ACTIVITY",
            "name": "Social protection"
          }
        ]
      }
    }
  ]
}

```

## Issues

Report issues for this extension in the [ocds-extensions repository](https://github.com/open-contracting/ocds-extensions/issues), putting the extension's name in the issue's title.
