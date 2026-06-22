# Invoice Exchange Rate Reference Data

Practical examples for teams that need a reference exchange rate for invoice dates, old receipts, ecommerce orders, reimbursements, or month-end reports.

This repository points to FXpeek resources for historical exchange-rate lookup, CSV export, and lightweight API workflows. It is for reporting and spreadsheet reference data only. It is not a broker quote, payment quote, trading signal, tax advice, or accounting advice.

## Useful FXpeek Entry Points

- Invoice and report date lookup: https://fxpeek.com/en/answers/exchange-rate-by-date?utm_source=github&utm_medium=repo&utm_campaign=fxpeek_invoice_exchange_rate&utm_content=exchange_rate_by_date
- Currency converter by date: https://fxpeek.com/en/answers/currency-converter-by-date?utm_source=github&utm_medium=repo&utm_campaign=fxpeek_invoice_exchange_rate&utm_content=currency_converter_by_date
- Historical exchange-rate API and CSV docs: https://fxpeek.com/en/api?utm_source=github&utm_medium=repo&utm_campaign=fxpeek_invoice_exchange_rate&utm_content=api_csv
- Excel and Google Sheets historical-rate workflow: https://fxpeek.com/en/answers/excel-spreadsheet-historical-rates?utm_source=github&utm_medium=repo&utm_campaign=fxpeek_invoice_exchange_rate&utm_content=spreadsheet_answer_hub
- Full historical FX reference report: https://fxpeek.com/en/reports/2026-historical-fx-reference?utm_source=github&utm_medium=repo&utm_campaign=fxpeek_invoice_exchange_rate&utm_content=reference_report

## When This Is Useful

- Matching an invoice date to a reference FX rate
- Rebuilding old travel or reimbursement records
- Preparing spreadsheet rows for monthly reporting
- Reconciling ecommerce orders across currencies
- Creating repeatable API or CSV pulls for supported currency pairs

## Example Spreadsheet Columns

```csv
invoice_id,invoice_date,from_currency,to_currency,amount,reference_rate,converted_amount,source
INV-1001,2026-06-15,USD,IDR,125.00,17809.00,2226125.00,FXpeek reference
```

## Example API Workflow

```bash
curl "https://fxpeek.com/api/rates?from=USD&to=IDR"
```

Use the FXpeek API docs for supported endpoints, CSV workflows, and current production behavior:

https://fxpeek.com/en/api?utm_source=github&utm_medium=repo&utm_campaign=fxpeek_invoice_exchange_rate&utm_content=api_docs

## Localized Starting Points

- Chinese API and CSV docs: https://fxpeek.com/zh/api?utm_source=github&utm_medium=repo&utm_campaign=fxpeek_invoice_exchange_rate&utm_content=zh_api
- Indonesian API and CSV docs: https://fxpeek.com/id/api?utm_source=github&utm_medium=repo&utm_campaign=fxpeek_invoice_exchange_rate&utm_content=id_api
- Vietnamese API and CSV docs: https://fxpeek.com/vi/api?utm_source=github&utm_medium=repo&utm_campaign=fxpeek_invoice_exchange_rate&utm_content=vi_api
- Thai API and CSV docs: https://fxpeek.com/th/api?utm_source=github&utm_medium=repo&utm_campaign=fxpeek_invoice_exchange_rate&utm_content=th_api
- Tagalog API and CSV docs: https://fxpeek.com/tl/api?utm_source=github&utm_medium=repo&utm_campaign=fxpeek_invoice_exchange_rate&utm_content=tl_api

## Disclaimer

FXpeek provides reference data for reports, spreadsheets, and research workflows. Always verify accounting, tax, and payment requirements with your own finance process and official sources.
