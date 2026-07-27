# ConvoControl Print Masters

Print-ready book files for **Lulu** print-on-demand fulfillment. Public so Lulu can download each file by URL when n8n places a print job. These are the authoritative source files pulled from the ConvoControl Lulu account.

## Structure

```
<book>/
  paperback/  interior.pdf  cover.pdf
  hardcover/  interior.pdf  cover.pdf
  workbook/   interior.pdf  cover.pdf
```

Books print at 5 x 8 in (Novella, Cream, Glossy). Workbooks print at 8.5 x 11 in (US Letter, White, Glossy). Covers are wraparound (front + spine + back).

## Books

| Book | Folder | Status |
|---|---|---|
| Questions Close Deals | `qcd/` | paperback, hardcover, workbook |

More titles added as their source files are collected.

## How it is used

The n8n workflow "Physical Book Purchase → Lulu Print Job" references these files by their raw URL, e.g.
`https://raw.githubusercontent.com/tara885/convocontrol-print-masters/main/qcd/paperback/interior.pdf`
