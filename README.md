# India Finance Excel Templates

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23349745.svg)](https://doi.org/10.5281/zenodo.23349745)


Free Excel templates for common Indian personal-finance decisions. Every sheet uses live formulas: change the yellow cells and the green cells recalculate.

| Template | What it answers | Live version |
|---|---|---|
| [reduce-emi-or-tenure-calculator.xlsx](reduce-emi-or-tenure-calculator.xlsx) | After a home-loan part-prepayment: reduce EMI or reduce tenure, and the interest each saves. After a rate change: raise the EMI or extend the loan (RBI reset rules, RBI/2023-24/55). Includes a letter to your bank. | [Reduce EMI or Tenure calculator](https://paisatools.co.in/reduce-emi-or-tenure-calculator) |
| [1-lakh-savings-planner.xlsx](1-lakh-savings-planner.xlsx) | How many months to save ₹1 lakh on your salary and saving rate, with or without interest, plus a 36-month tracker. | [1 lakh kaise jama kare](https://paisatools.co.in/blog/1-lakh-kaise-jama-kare) |
| [epf-interest-calculator.xlsx](epf-interest-calculator.xlsx) | EPF interest for one financial year from your current balance and monthly EPF credit, month by month the way EPFO computes it (interest on the balance at the start of each month; credited once at year end). Shows why the credit looks smaller than the headline rate. | [PF interest calculator](https://paisatools.co.in/pf-interest-calculator) |
| [full-and-final-settlement-calculator.xlsx](full-and-final-settlement-calculator.xlsx) | Full and final settlement from the employee's side: final-month salary, leave encashment, gratuity (5 years permanent; pro-rata after 1 year fixed-term), notice recovery, the legal deadline (two working days under Code on Wages s.17(2), in force 21 Nov 2025, via `WORKDAY`), days late, and tax (leave encashment ₹25 lakh, gratuity ₹20 lakh). | [Full and Final Settlement Checker](https://paisatools.co.in/fnf-settlement-calculator) |

| [home-loan-amortization-schedule-with-prepayment.xlsx](home-loan-amortization-schedule-with-prepayment.xlsx) | Month-by-month home loan schedule (up to 360 months) with a column for one-off prepayments, a cell for a regular extra amount each month, and a floating-rate column (type the new rate in the month your bank resets it; it carries forward). The EMI stays fixed, so prepayments shorten the loan and rate rises lengthen it; it shows the months saved and the interest saved against the same loan with no prepayments. | [EMI calculator](https://paisatools.co.in/emi-calculator) |
| [income-tax-calculator-fy-2026-27.xlsx](income-tax-calculator-fy-2026-27.xlsx) | Income tax for FY 2026-27 (AY 2027-28), new vs old regime side by side for a salaried resident: ₹75,000 / ₹50,000 standard deduction, age-wise old-regime exemption, 80C, 80D, HRA, home-loan interest and NPS 80CCD(1B) with their caps, the 87A rebate up to ₹12 lakh with marginal relief, surcharge and 4% cess. Every slab is a visible row, and a verdict line says which regime is cheaper. | [Income tax calculator](https://paisatools.co.in/income-tax-calculator) |

## How the numbers work
- Loans: standard reducing-balance amortisation at the annual rate ÷ 12, using Excel's `PMT` and `NPER`.
- "Reduce tenure" keeps the EMI and solves for the number of months; the last instalment is smaller, so a bank's schedule may differ by a few rupees and by the date it posts the prepayment.
- EPF: interest = balance at the start of each month × rate ÷ 12; a month's contribution earns from the next month; the year's interest is credited once at the end of March. Use the passbook EPF credit (employee + employer share), not the pension (EPS) part.
- Savings: months to goal with `NPER` on monthly deposits; the tracker compares planned and actual saving each month.

Worked check (amortization template): ₹30 lakh at 8.5% for 240 months, EMI ₹26,035. An extra ₹2,000 every month closes the loan in 202 months (38 sooner) and saves about ₹6.13 lakh of interest; a one-off ₹2 lakh in month 12 closes it in 206 months and saves about ₹6.88 lakh. If the rate resets to 9% from month 37, the same EMI needs 257 months; adding ₹2,000 a month brings it back to 211 and saves about ₹7.86 lakh.

Worked check (income tax template): ₹13 lakh gross salary gives taxable income of ₹12.25 lakh in the new regime; the slabs give ₹63,750, marginal relief caps it at the ₹25,000 above ₹12 lakh, so the tax is ₹26,000 with cess (₹66,300 without the relief). ₹18 lakh gross: new regime ₹1,50,800; old regime with ₹1.5 lakh 80C and ₹25,000 80D ₹2,96,400. Checked against the PaisaTools engine at six salaries.

Worked check (in the template defaults): ₹30 lakh, 240 EMIs left, rate 8.25% → 8.50%. Keeping the EMI at ₹25,562 stretches the loan to 253 EMIs; raising it to ₹26,035 keeps the end date and costs about ₹1.97 lakh less interest.

## Licence
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Use, share and adapt, including commercially, with credit to [PaisaTools](https://paisatools.co.in).

Estimates for planning, not financial advice. Check your own loan terms with your lender.


## Cite
PaisaTools (2026). DOI: [10.5281/zenodo.23349745](https://doi.org/10.5281/zenodo.23349745)
