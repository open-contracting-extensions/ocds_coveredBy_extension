# Covered By

This extension adds a field to indicate the treaties that the contracting process is covered by.

A treaty, like the Agreement on Government Procurement (GPA), can require a member to indicate that a contracting process is covered by it. The `tender.coveredBy` field should be used to meet such requirements.

To disclose the laws or regulations that govern the contracting process and that grant legal authority to the procuring entity, use the [legalBasis extension](https://github.com/open-contracting-extensions/ocds_legalBasis_extension) instead.

## Legal context

The [Revised Agreement on Government Procurement](https://www.wto.org/english/docs_e/legal_e/rev-gpr-94_01_e.htm) (GPA) includes: "each notice of intended procurement shall include … l. an indication that the procurement is covered by this Agreement."

The European Union is a [party](https://www.wto.org/english/tratop_e/gproc_e/memobs_e.htm) to the GPA, and as such its [Directive 2014/24/EU](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=uriserv:OJ.L_.2014.094.01.0065.01.ENG) (Public contracts — setting out clear ground rules) includes: "Part C: Information to be included in contract notices … 29. Indication whether the contract is covered by the GPA."

## Example

The `tender.coveredBy` field is an array of strings, whose values are selected from the `coveredBy.csv` open codelist.

```json
{
  "tender": {
    "coveredBy": [
      "GPA"
    ]
  }
}
```

## Issues

Report issues for this extension in the [ocds-extensions repository](https://github.com/open-contracting/ocds-extensions/issues), putting the extension's name in the issue's title.

## Changelog

### 2020-04-24

* Add `minProperties`, `minItems` and/or `minLength` properties.
