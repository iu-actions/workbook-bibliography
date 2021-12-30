# workbook-bibliography

[![GitHub issues](https://img.shields.io/github/issues/iu-actions/workbook-bibliography)](https://github.com/iu-actions/workbook-bibliography/issues)

This action generates the bibliography for an IU workbook.

## Found a bug? 💁‍♀️

Thanks for letting us know! Please [file an issue](../../issues/new?assignees=&labels=&template=bug_report.md&title=) and we should reply shortly.

## Configuration

This action requires the presence of inputs, which are listed below.

### Inputs
- `bibliography`: Path to the `bibliography.md`. (**required**)

*Note*: The following files must be present at the specified location and contain the appropriate variables.

- `format_doc`: Path to the Microsoft Word template of the bibliography. (**required**) → [Learn more](https://pandoc.org/MANUAL.html#option--reference-doc)

## Example

Below you will find an example of how you can use this action.

```yaml
uses: iu-actions/workbook-bibliography@v1
with:
  # content details
  bibliography: exam/bibliography.md
          
  # configuration details
  format_doc: .workbook/bibliography/format.docx
```
