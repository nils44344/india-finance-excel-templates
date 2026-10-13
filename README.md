# India Finance Excel Templates

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23349745.svg)](https://doi.org/10.5281/zenodo.23349745)


Free Excel templates for common Indian personal-finance decisions. Every sheet uses live formulas: change the yellow cells and the green cells recalculate.

| Template | What it answers | Live version |
|---|---|---|
| [reduce-emi-or-tenure-calculator.xlsx](reduce-emi-or-tenure-calculator.xlsx) | After a home-loan part-prepayment: reduce EMI or reduce tenure, and the interest each saves. After a rate change: raise the EMI or extend the loan (RBI reset rules, RBI/2023-24/55). Includes a letter to your bank. | [Reduce EMI or Tenure calculator](https://paisatools.co.in/reduce-emi-or-tenure-calculator) |
| [1-lakh-savings-planner.xlsx](1-lakh-savings-planner.xlsx) | How many months to save ₹1 lakh on your salary and saving rate, with or without interest, plus a 36-month tracker. | [1 lakh kaise jama kare](https://paisatools.co.in/blog/1-lakh-kaise-jama-kare) |
| [epf-interest-calculator.xlsx](epf-interest-calculator.xlsx) | EPF interest for one financial year from your current balance and monthly EPF credit, month by month the way EPFO computes it (interest on the balance at the start of each month; credited once at year end). Shows why the credit looks smaller than the headline rate. | [PF interest calculator](https://paisatools.co.in/pf-interest-calculator) |

## How the numbers work
- Loans: standard reducing-balance amortisation at the annual rate ÷ 12, using Excel's `PMT` and `NPER`.
- "Reduce tenure" keeps the EMI and solves for the number of months; the last instalment is smaller, so a bank's schedule may differ by a few rupees and by the date it posts the prepayment.
- EPF: interest = balance at the start of each month × rate ÷ 12; a month's contribution earns from the next month; the year's interest is credited once at the end of March. Use the passbook EPF credit (employee + employer share), not the pension (EPS) part.
- Savings: months to goal with `NPER` on monthly deposits; the tracker compares planned and actual saving each month.

Worked check (in the template defaults): ₹30 lakh, 240 EMIs left, rate 8.25% → 8.50%. Keeping the EMI at ₹25,562 stretches the loan to 253 EMIs; raising it to ₹26,035 keeps the end date and costs about ₹1.97 lakh less interest.

## Licence
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Use, share and adapt, including commercially, with credit to [PaisaTools](https://paisatools.co.in).

Estimates for planning, not financial advice. Check your own loan terms with your lender.


## Cite
PaisaTools (2026). DOI: [10.5281/zenodo.23349745](https://doi.org/10.5281/zenodo.23349745)
