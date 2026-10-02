# Portfolio maintenance changes

This repository remains based on the original academic project. The following maintenance was performed before publication rather than redesigning the solution.

## Security / privacy

- Removed the MongoDB Atlas Data API key that was stored in the original BaseX files.
- Moved the API key and Data API endpoint to environment variables.
- Removed group-member identifying information and the original group report from the public version.
- Replaced partner identification in public samples with generic demonstration values.

## Data and repository size

- Removed full generated exports such as `Vendas.json` (~616 MB) and `Devolucoes.json` (~153 MB).
- Replaced large generated JSON/XML outputs with small representative `*.sample.*` files.
- Added `.gitignore` and `.gitattributes`.

## Functional corrections retained from portfolio review

- Corrected customer-status boundaries: `<1 year = novo`, `1–5 years = regular`, `>5 years = premium`.
- Corrected the three-year customer statistics aggregation.
- Corrected invalid XML element naming (`5g` -> `is_5g`).
- Aligned XSD cardinalities/structures with the reports produced by the project.
- Corrected early-return classification to `<= 3 days`.
- Corrected distinct-product counting in monthly sales statistics.
- Updated BaseX resources to transform MongoDB responses into the project's XML vocabulary instead of returning generic JSON-to-XML output.
- Added `year`/`month` filtering to the monthly sales and return resources.

These changes are documented so the portfolio version is not presented as an exact byte-for-byte copy of the original submission.

## Final portfolio audit

- Removed the remaining full generated exports from the distributable repository, keeping only representative `.sample.*` files.
- Reduced customer, product and customer-statistics samples to a small set of representative records.
- Removed a duplicated MongoDB Data API URL validation branch in the BaseX resources.
- Revalidated the public sample XML documents against their XSD schemas.
- Rechecked the public tree for the original student identifiers and hard-coded MongoDB credentials.

