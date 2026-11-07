# FAFF | Financial analysis and cash planning for retail and wholesale

**An Excel model for reading financial statements, spotting cash pressure and reviewing repayment capacity.** FAFF connects two years of historical financial analysis with a rolling 13-week cash forecast, monthly break-even analysis, peer comparisons and a lender-facing summary. It is available in English and Arabic, with a clean template and a worked example in each language.

| Version | Start here if you want to… |
| --- | --- |
| [English template](./FAFF_English.xlsx) | Enter your own business data in a clean workbook. |
| [Arabic template — النموذج العربي](./FAFF_Arabic.xlsx) | Use the same workflow in a right-to-left Arabic workbook. |
| [English XAZ demo](./FAFF_English_XAZ.xlsx) | Follow a fully populated fictional wholesaler through the model. |
| [Arabic XAZ demo — المثال التطبيقي](./FAFF_Arabic_XAZ.xlsx) | Walk through the same fictional business in Arabic. |

**Read in order** · [Development](#how-faff-developed) · [Getting started](#getting-started) · [XAZ case study](#xaz-case-study) · [Ratio dictionary](#ratio-dictionary) · [Operating and credit KPIs](#operating-and-credit-kpis) · [Benchmarks](#how-benchmarking-works) · [Validation](#validation-and-limitations)

## The three questions behind FAFF

1. **How is the business performing?** Read the three financial statements together. Sales growth, margin, working capital and operating cash can move in different directions.
2. **Can we pay what is due, when it is due?** Start with available bank cash and dated receipts and payments. Annual earnings and year-end cash cannot tell you which week payroll or supplier settlements will put cash under pressure.
3. **Can the business service its commitments and the proposed loan?** Compare next-12-month cash available for debt service with scheduled principal, interest or profit charges and included lease payments. Review timing, covenants and evidence alongside the ratio.

The workbook separates these questions from a fourth one: **how complete is the evidence?** A business can have complete records, reconcile to the bank and still face a cash shortage. It can also start cash planning before it has two years of financial statements.

## How FAFF developed

| Phase | Work and result |
| --- | --- |
| 1. Financial statement analysis | Started with the MAKCO exercise. Built linked balance sheet and income statement analysis, period-over-period movements, common-size statements and grouped ratios. |
| 2. Cash flow and inventory | Added an indirect-method cash flow statement, free cash flow and cash-quality measures. Expanded inventory, receivables and payables analysis for trading businesses. |
| 3. Saudi localization | Separated Zakat, income tax and VAT where relevant. Added local reporting inputs, related-party exposure, leases and evidence-based reconciliation. Used Savola disclosures as a reporting-structure stress test during development. |
| 4. Founder and lender workflows | Added the rolling weekly forecast, contribution and break-even analysis, overdue and supplier registers, credit schedules, the earnings bridge and summaries for different readers. |
| 5. Calculation and evidence review | Checked denominator guards, blank-template messaging, zero and negative equity, current/prior period coverage, adjustment years and dated bank evidence. Separated operating completeness from historical reconciliation and contribution readiness. |
| 6. XAZ demonstration | Built a fictional Saudi wholesaler with statements, bank evidence, trading records, proposed borrowing and a fictional peer sample. Tested both the baseline and changes to collections, funding, costs, suppliers, financing and evidence. |
| 7. Arabic release and English alignment | Localized the workbook into Arabic with right-to-left presentation, aligned the navigation, input and output groups, reconciliation totals and chart explanations across languages, then compared the two XAZ builds. |

**Project owner** · Omar Alsaadi. I used OpenAI Codex to help upgrade the Excel model, implement and review formulas and controls, localize the workbook and automate regression and cross-language checks.

## Getting started

Open the workbook in desktop Microsoft Excel and allow it to recalculate. Start on **Introduction and Requirements**. Follow the input and output tab colors and the cell-level instructions. Enter amounts in a consistent reporting unit across statements, operating inputs and credit schedules. Keep dates, days, percentages, transaction counts and per-share figures in their own units.

| Step | Enter or verify | Where to read the result |
| --- | --- | --- |
| 1. Set the assessment basis | In **Founder Inputs**, select retail or wholesale and enter the business scope, reporting unit, assessment date, reviewer, first stored week, available opening bank cash, evidence date and minimum reserve. | **Founder View** shows evidence readiness and, as the forecast is completed, the cash outlook. |
| 2. Build the cash forecast | Enter dated cash receipts and cash payments on **Weekly Cash Forecast**. Enter supplier obligations in the linked supplier ledger and overdue items in their register on **Founder Inputs**. Check the completed weeks against independent closing bank balances. | **Founder View** shows first reserve breach, first negative week, low point, runway and priorities. **Important Charts** shows the weekly path and cash bridge. |
| 3. Test monthly economics | Enter one month's net revenue, true variable costs and total fixed costs in **Founder Inputs**. Use the same month and business scope throughout. | **Founder View** shows contribution, break-even sales and the surplus or gap after fixed costs. |
| 4. Enter historical statements | Set the current year and any prior year in **Assumptions**. Enter the detailed financial statement lines in **Historical Financial Data**. Compare the calculated totals with separately sourced totals if available. | **Balance Sheet**, **Income Statement**, **Cash Flow Statement**, **Fundamental Analysis** and the five ratio sheets. **Assumptions** shows reconciliation coverage by year. |
| 5. Review debt and earnings | Enter actual schedules, facility terms, covenant evidence and the next-12-month projection on **Credit Schedules**. Record documented earnings adjustments on **Earnings Bridge**, with approval, fiscal year and effects on Zakat, tax and non-controlling interests as applicable. | **Company Summary** shows continuity and repayment indicators. **Credit Schedules** shows the supporting service, maturity and covenant detail. |
| 6. Add comparison evidence | Enter eligible peer data in the optional benchmark block on **Founder Inputs**. Use the same metric definition, period, business model and peer scope. Add Saudi sales and payment indicators if reliable data is available. | **Founder View** shows validated peer bands or the applicable fallback. **Benchmarks** documents historical screening profiles. |

**Record each amount once.** Enter detailed line items in the historical input sheet and let the workbook calculate subtotals. When a source amount is included in a detailed line, keep it out of overlapping “other” lines. For example, if retained earnings already include the current year's profit, enter a confirmed zero on the separate current-profit line. Use the reported-totals comparison fields for independently sourced totals from accounts or reports. They are comparison figures. This is an internal tie-out that can be done from the company's own records.

**Use zero for confirmed zero and blanks for missing evidence.** A complete forecast needs deliberate zero entries where applicable. A missing prior year limits comparisons. An unavailable optional peer table leaves the core cash and historical analysis usable. Avoid replacing formulas with manual inputs or re-entering values in linked output tables.

## XAZ case study

XAZ is a **fictional Saudi wholesaler**. The demonstration uses FY2024 and FY2025 statements and a cash review dated 6 November 2026. Amounts in this section are in **SAR thousands**, except ratios, dates and per-share values. The 20-company comparison sample is fictional too.

| Question | Demonstration result | What it tells the founder |
| --- | --- | --- |
| Did sales growth translate to earnings? | Revenue rose from 10,000 to 12,000, while gross margin fell from 28.0% to 25.0% and consolidated net profit fell from 690 to 530. FY2025 operating margin was 7.5%. | Check purchase prices, discounts, product mix and overhead. Gross profit in money rose from 2,800 to 3,000 even as the gross margin percentage fell. |
| Did earnings convert to cash? | Operating cash flow fell from 645 to 130. Free cash flow after lease principal fell from 145 to −470. | Review changes in stock and receivables alongside capex and lease commitments. |
| Where does cash run tight? | Active opening available cash was 320. The 200 reserve was first breached in the week starting 16 November 2026. The first negative week started 11 January 2027. The minimum was −17 and the forecast ended at 24. | The closing number hides the negative week. At the low point, 17 closes the modeled cash deficit and 217 restores the full reserve, before any contingency. |
| How does runway compare? | Average net burn before funding was about 132 per month, implying roughly 2.42 months of runway from active opening cash. | Use the dated weekly path to plan payments. Runway averages the whole window and can hide earlier pressure. |
| Does the month cover fixed costs? | Revenue 1,000 less variable costs 750 produced contribution of 250, or 25%. Fixed costs of 280 left a 30 shortfall. Break-even revenue was 1,120. | At the same cost structure and sales mix, the month needed 120 more revenue or a 30 improvement in contribution or fixed costs. |
| Can XAZ service the proposed borrowing? | CFADS of 700 against 620 existing and 160 proposed service produced 0.90× DSCR. Headroom was −220 at the 1.25× model screen. One covenant breached. Eligible undrawn facilities were 300. | At 1.25×, 700 of available cash supports 560 of annual service. The proposed total is 780. The 300 of facility availability is shown separately from cash already in the bank. |
| What does the peer example show? | Gross margin of 25.0% was above the fictional wholesale median of 23.0% and below P75 of 27.9%. Credit-sales DSO was about 76.0 days, inventory days 89.2 and GMROI 1.36×. | A business can outperform the peer median on margin while cash is tied up in receivables and stock. |
| What evidence passed? | All six operating evidence checks were complete, 56 year-specific historical checks passed and contribution evidence was complete. | The poor cash and repayment outcomes stayed visible even with complete evidence. |
| What did the historical screen flag? | The overall score was about 51.9% across 26 scored ratios, with 7 flags among 17 computable red-flag tests. The profitability group scored 100%, while cash flow scored about 7.1%. | A score groups signals that can point in different directions. Review the underlying flags and the actual cash forecast. |

### What changed under stress

| Change in a test copy | Observed result |
| --- | --- |
| Increase scheduled customer collections | Ending cash rose from 24 to 674 and the forecast cleared its breaches. Historical profit remained 530. |
| Remove confirmed owner funding of 100 | Ending cash fell to −76 and minimum cash fell to −117. |
| Reduce monthly variable costs | Contribution after fixed costs improved to +20 and break-even revenue fell to about 933.33. Weekly ending cash stayed at 24 because only the monthly economics inputs changed. |
| Reduce supplier payments in the ledger | Ending cash rose to 74 and minimum cash to 33. The negative week cleared, while the reserve remained at risk. |
| Lower proposed loan service | Modeled DSCR improved from about 0.90× to 1.00×. At that level CFADS covers the included service exactly, with zero cushion. |
| Invalidate opening cash evidence | Readiness and the cash conclusion responded to the missing verification. A verified cash conclusion depends on the opening evidence. |

## Reading the statements

- **Balance sheet** records assets, liabilities and equity at a point in time. In the common-size view, each line is expressed relative to total assets. Compare the composition of assets and funding as well as the totals.
- **Income statement** records revenue and costs on an accrual basis. Common-size profit and loss lines use revenue as their base. Profit can include sales that customers have yet to pay.
- **Cash flow statement** separates operating, investing and financing activity. The indirect operating section reconciles profit to operating cash through non-cash adjustments, reclassifications and working-capital changes. The workbook also presents cash-flow lines relative to revenue and derives several free cash flow measures. [IFRS Foundation — IAS 7 Statement of Cash Flows](https://www.ifrs.org/issued-standards/list-of-standards/ias-7-statement-of-cash-flows/)
- **Horizontal analysis** shows the amount change as current less prior. Where a valid comparable base exists, percentage change relates the difference to the prior base. Read the actual change, trend and threshold status separately. For example, falling collection days can be favourable while a falling cash ratio calls for a liquidity review.
- **Historical reconciliations** check statements and evidence by declared year. Examples include balance sheet balancing, allocation of profit, opening and closing cash ties, common-size totals, Zakat and income-tax roll-forwards, combined cash paid and parent equity. Missing required evidence stays visible. Out-of-scope periods are marked separately.
- **Saudi reporting inputs** keep Zakat, income tax, VAT and related-party effects distinct. Where roll-forward data is supplied, reconcile opening liabilities, current charges or reversals, payments and other movements to the reported closing liability. Use the company's applicable accounting and statutory treatment for the underlying entries.

## Ratio dictionary

These are the workbook's measures. Some have multiple conventions in practice. **The denominator matters.** Confirm whether a balance is closing or average, whether sales include cash sales, whether a debt measure includes leases and whether an earnings measure is consolidated or parent-only.

**Notation** · CFO = cash flow from operations. COGS = cost of goods sold. EBIT = earnings before interest and taxes, using operating profit where specified. EBITDA proxy = operating EBIT plus same-scope operating depreciation and amortisation supplied in Historical Financial Data. PBT = consolidated profit before Zakat and income tax. PP&E = property, plant and equipment. Capex and payments in the definitions below are positive outflow amounts unless stated otherwise.

### Liquidity and asset quality

| Ratio or KPI | FAFF definition | How to interpret it |
| --- | --- | --- |
| Current ratio | Current assets ÷ current liabilities. | Short-term balance sheet coverage. Check how much is stock or overdue receivables. |
| Quick ratio | (Cash and cash equivalents + net trade receivables) ÷ current liabilities. | More liquid coverage under the workbook's narrower definition. |
| Cash ratio | Cash and cash equivalents ÷ current liabilities. | Immediate cash relative to short-term obligations at the reporting date. |
| Adjusted current ratio | (Current assets − current related-party trade and other receivables) ÷ current liabilities. | Tests reliance on related-party collection. |
| Adjusted quick ratio | (Cash and cash equivalents + third-party trade receivables) ÷ current liabilities. | Narrow coverage without related-party trade receivables. |
| Acid-test ratio, textbook form | (Current assets − inventory) ÷ current liabilities. | Can still include other current assets that are slower to realise. Compare with FAFF's quick ratio. |
| Net working capital | Current assets − current liabilities. | Short-term balance sheet cushion in money. |
| Net working capital / total assets | Net working capital ÷ total assets. | Scales the cushion to the size of the balance sheet. |
| Related-party receivables / current assets | Current related-party trade and other receivables ÷ current assets. | Exposure inside the current asset pool. |
| Total related-party receivables / assets or equity | Mapped current and non-current related-party receivables ÷ total assets or total equity. The separate founder governance view also shows a parent-equity basis. | Measures exposure relative to resources or loss-absorbing capital. Check which equity basis is shown. |
| Defensive interval | (Cash + net trade receivables) ÷ estimated daily cash operating cost. The cost proxy uses COGS and selected operating expenses less D&A, divided by period days. | Approximate days covered by defensive assets. A dated forecast provides a more direct view of payment timing. |

### Efficiency and working capital

Historical turnover uses the balance basis shown in the sheet. The founder peer indicators use matching average balances where specified. When averaging two balances, use opening plus closing divided by two, with consistent scope.

| Ratio or KPI | FAFF definition and interpretation |
| --- | --- |
| Days sales outstanding (DSO), historical | Trade receivables ÷ total revenue × period days. A broad collection proxy. |
| Sales-based DSO, peer view | Average trade receivables ÷ all sales × period days. Cash sales can pull the result below credit-sales DSO. |
| Credit-sales DSO | Average matching trade receivables ÷ annual credit sales × period days. Compare with credit terms and the ageing report. |
| Days inventory outstanding (DIO) | Inventory ÷ COGS × period days. The founder peer view uses average inventory. Measures time that cash is tied up in inventory. |
| Days payables outstanding (DPO), historical or COGS proxy | Trade payables ÷ COGS × period days, using the applicable historical or average balance. COGS is a proxy for purchases. |
| DPO, credit-purchases basis | Average matching trade payables ÷ annual credit purchases × period days. Compare with supplier terms and overdue balances. |
| Operating cycle | DSO + DIO. Estimates time from holding stock through collecting the sale. |
| Cash conversion cycle (CCC) | DSO + DIO − DPO. Estimates the funding gap after supplier credit. Use consistent component definitions. |
| Receivables turnover | Revenue ÷ trade receivables. Higher turnover generally indicates less receivables investment per unit of sales. |
| Payables turnover | COGS ÷ trade payables. Higher turnover can indicate faster payment or a different purchase mix. |
| Inventory turnover | COGS ÷ inventory. Read alongside stockouts, seasonality and ageing. |
| Gross margin return on inventory (GMROI) | Gross profit ÷ inventory at carrying cost. The founder peer measure uses average inventory. Shows gross profit earned per unit invested in stock. |
| Total asset turnover | Revenue ÷ total assets. Measures revenue generated per unit of assets. |
| Current asset turnover | Revenue ÷ current assets. Relates sales to the current resources supporting them. |
| Equity turnover | Revenue ÷ positive total equity. A high result can reflect a thin equity base. |
| Working-capital turnover | Revenue ÷ positive net working capital. Can be unstable near zero. |
| Fixed-asset turnover | Revenue ÷ PP&E. Compare firms with similar lease, ownership and outsourcing models. |
| Cash turnover | Revenue ÷ cash and cash equivalents. A high result can coexist with low cash resilience. |

### Profitability, returns and DuPont

| Ratio or KPI | FAFF definition and interpretation |
| --- | --- |
| Gross profit margin | Gross profit ÷ revenue. Shows how much of each sales unit remains after COGS. |
| Operating profit margin / operating EBIT margin | Operating profit ÷ revenue. Measures the trading result after operating costs and before separately presented financing and statutory charges. |
| Net profit margin | Consolidated net profit ÷ revenue. Includes financing, non-operating and statutory effects reflected in profit. |
| Operating EBITDA proxy margin | (Operating EBIT + same-scope operating D&A) ÷ revenue. Compare definitions before using it across companies. |
| Operating expense ratio | (General and administrative + marketing + R&D expense) ÷ revenue. Covers the specified overhead lines. |
| Combined Zakat and income-tax burden | Combined charge ÷ consolidated pre-Zakat and income-tax profit. Read the underlying charge and PBT, especially in a loss or reversal year. |
| Separate monetary-position loss / revenue | Separate reported monetary-position loss, expressed as an expense, ÷ revenue. Relevant when the financial statements include this line. |
| Return on assets (ROA) | Consolidated net profit ÷ total assets on the sheet's historical balance basis. |
| Parent return on equity (ROE) | Profit attributable to the parent ÷ positive parent equity. Matches the numerator and ownership claim. |
| Return on capital employed (ROCE) | Operating EBIT ÷ (total assets − current liabilities). Relates operating profit to the workbook's capital base. |
| Earnings per share (EPS) | Reported EPS taken from the income statement inputs. For adjusted EPS, the bridge divides adjusted parent profit by the relevant weighted-average shares after unit alignment. |
| Parent net margin | Profit attributable to the parent ÷ consolidated revenue. A component of the parent ROE bridge. |
| DuPont asset turnover | Consolidated revenue ÷ total assets. |
| DuPont equity multiplier | Total assets ÷ positive parent equity. |
| Three-step DuPont ROE | Parent net margin × asset turnover × equity multiplier. The intermediate denominators cancel to parent profit ÷ parent equity when the components are valid. |
| Parent profit / consolidated PBT | Parent net profit ÷ consolidated pre-Zakat and income-tax profit. Blends statutory and ownership effects. |
| Consolidated PBT / operating EBIT | Consolidated PBT ÷ operating EBIT. Captures financing and other below-operating effects together. |
| Five-step DuPont ROE | Parent profit / consolidated PBT × consolidated PBT / operating EBIT × operating EBIT margin × asset turnover × equity multiplier. |
| DuPont reconciliation | Direct parent ROE minus five-step ROE. A non-zero difference calls for checking definitions and scope. |
| Revenue, EBIT, net profit and EPS growth | Current-period movement in each measure relative to its comparable prior-period base, subject to validity guards. Inspect the absolute change alongside the rate, especially with losses or small bases. |
| Adjusted consolidated net margin | Adjusted consolidated profit ÷ revenue. |
| Adjusted parent profit | Parent profit after approved, year-matched adjustments and applicable Zakat, income tax and non-controlling-interest effects. Keep the reported result visible. |
| Adjusted EPS | Adjusted parent profit ÷ appropriate weighted-average shares, using consistent units. |

### Leverage and finance-cost coverage

| Ratio or KPI | FAFF definition and interpretation |
| --- | --- |
| Debt ratio | Total liabilities ÷ total assets. Here “debt ratio” includes non-borrowing liabilities. |
| Equity ratio | Total equity ÷ total assets. Shows the equity share of funding. |
| Debt-to-equity | Total liabilities ÷ positive total equity. |
| Interest-bearing debt / equity | Mapped short- and long-term borrowing and lease liabilities ÷ positive total equity. |
| Short-term liabilities / equity | Current liabilities ÷ positive total equity. |
| PP&E / equity | Net PP&E ÷ positive total equity. Indicates fixed asset investment relative to equity. |
| Interest coverage | Operating EBIT ÷ finance costs. A zero charge or reversal needs separate interpretation. |
| Textbook finance-cost coverage | (Consolidated net profit + finance costs) ÷ finance costs, using the workbook's textbook variant. The numerator differs from operating EBIT. |
| EBITDA / finance costs | Operating EBITDA proxy ÷ finance costs. This earnings-based measure omits debt principal and working-capital cash needs. |
| Net debt / net cash | Mapped borrowing and lease liabilities − cash and cash equivalents. Negative results indicate net cash on this definition. |
| Net debt / EBITDA | Net debt ÷ positive operating EBITDA proxy. Compare with actual maturity dates and covenants. |
| Net debt / EBIT | Net debt ÷ positive operating EBIT. |
| Short-term share of liabilities | Current liabilities ÷ total liabilities. Measures maturity concentration across all liabilities. |
| Self-financing ratio | (Restricted reserves appropriated from profits + retained earnings + separately presented current profit, if applicable) ÷ paid-in share capital. |

### Cash flow and free cash flow

Free cash flow depends on the question. Start with reported CFO, deduct cash capex, then show lease principal separately when it sits in financing. Cash after borrowing can improve even if the operating business generates less cash.

| Ratio or KPI | FAFF definition and interpretation |
| --- | --- |
| CFO / net profit | CFO ÷ positive consolidated net profit. Cash conversion of reported earnings. |
| CFO / EBITDA | CFO ÷ operating EBITDA proxy. Differences can reflect working capital, cash statutory charges and classification. |
| CFO margin | CFO ÷ revenue. Cash generated by operations per unit of sales. |
| Cash-flow accruals ratio | (Consolidated net profit − CFO) ÷ total assets. A positive value means reported profit exceeds operating cash for the period. |
| Working-capital change / CFO | Signed cash-flow effect of working-capital movements ÷ CFO. Check the signs of both values. |
| CFO growth and adjusted CFO growth | Current versus prior reported or evidenced adjusted CFO relative to its comparable base. |
| Absolute adjusted CFO gap | Absolute value of (adjusted CFO ÷ reported CFO − 1), when the reclassification is reviewed and the base supports the calculation. |
| Capex | Cash outlay on PP&E and intangibles as mapped to the cash flow statement. |
| Free cash flow (FCF) | Reported CFO − cash capex. |
| FCF margin | FCF ÷ revenue. |
| Capex / CFO | Cash capex ÷ CFO. Review the raw values when CFO is negative or small. |
| Capex / revenue | Cash capex ÷ revenue. Investment intensity relative to sales. |
| Capex / D&A | Cash capex ÷ reported depreciation and amortisation used in the cash flow statement. Timing and asset mix matter. |
| FCF after lease principal | FCF − lease principal classified in financing. |
| FCF margin after lease principal | FCF after lease principal ÷ revenue. Useful for comparing lease-heavy businesses on an explicitly stated basis. |
| FCF growth | Change in FCF relative to the valid comparable prior-period base. |
| Cash after capex and net borrowing | FCF + signed net borrowing movements, including short-term movements and lease principal on the workbook's basis. An equity-cash-flow proxy. |
| Cash retained after dividends | Cash after capex and net borrowing − cash dividends paid. The separate after-lease-and-dividends measure starts from FCF after lease principal. |
| Adjusted CFO and FCF | Reported CFO plus approved, evidenced analyst reclassification add-backs. Adjusted FCF deducts cash capex from adjusted CFO. |
| Operating cash flow ratio | CFO ÷ current liabilities. |
| CFO / total liabilities | CFO ÷ total liabilities. |
| CFO / interest-bearing debt | CFO ÷ mapped borrowings and lease liabilities. A period flow relative to a balance, distinct from annual scheduled service coverage. |
| Dividend cover by FCF | FCF ÷ cash dividends paid. |
| Dividend payout | Cash dividends paid ÷ positive consolidated net profit. |
| Cash self-funding | CFO ÷ (capex + dividends + net debt repayment when net financing movements represent repayment). |
| Net change in cash before FX / opening cash | Net cash movement before foreign exchange effects ÷ opening cash. |
| Inflation erosion of cash / opening cash | Cash monetary erosion amount ÷ opening cash, where a relevant IAS 29 cash adjustment is supplied. |
| Historical cash interest cover | CFO with cash interest and cash Zakat/tax charged in operating cash added back, divided by mapped cash interest across operating and financing sections. |
| Historical DSCR | CFO with operating-classified interest added back, divided by mapped cash interest plus disclosed gross principal service. Requires supporting service disclosure. The next-12-month credit DSCR below uses a separate projection. |

## Operating and credit KPIs

### Cash continuity and evidence

| Measure | Definition or action |
| --- | --- |
| Available opening cash | Verified bank cash less restrictions at the first stored week. Later weeks roll forward from dated records. Historical statement cash is a separate reporting figure. |
| Weekly closing available cash | Opening cash + customer receipts + confirmed funding − weekly cash payments. Payments include payroll, rent and core operations, suppliers, statutory amounts, debt and leases, interest or profit charges, capex, owner withdrawals and other payments. |
| 52-week register and active window | Stores dated actual and forecast data. The active view takes 13 consecutive weeks from the selected start. Advance the selector while keeping the original dates attached to records. |
| Reserve breach, cash shortfall and low point | First weekly close below the reserve, first close below zero and the lowest close in the active window. The funding-to-reserve measure is the amount needed to bring the low point back to the reserve. |
| Monthly burn and cash runway | Monthly burn before funding = (13-week cash payments − operating receipts) ÷ 13 × 52 ÷ 12. Runway = verified active opening cash ÷ positive monthly burn. For tight weeks, review day-by-day payment timing. |
| Bank reconciliation difference | Independently entered Actual closing bank cash − calculated Actual closing cash. Check the absolute difference against the bank tolerance in reporting units. The opening verification uses dated evidence and the entered initial bank cash. |
| Supplier cash and overdue balances | The supplier ledger feeds dated supplier cash payments. Track overdue customer, supplier, payroll, statutory and debt items in the applicable records with evidence, deadlines and payment arrangements. Deactivate a replaced commitment so the same instalment is counted once. |
| Six operating checks | Opening bank cash, 13-week inputs, forecast review, supplier ledger completeness, overdue evidence and bank reconciliations. The last check distinguishes initial verification from completed Actual weeks. |
| Contribution readiness and historical coverage | Contribution evidence has its own status. Historical checks separately report whether required year-specific checks were exercised and whether any mismatch was found. |
| Priority actions | The dashboard ranks actions by urgency from cash, overdue, contribution, stock and other available evidence. Read the underlying item, owner and due date before acting. |

### Unit economics, stock and local trading indicators

| Measure | Definition or action |
| --- | --- |
| Contribution and contribution margin | Net revenue − true variable costs. Divide contribution by net revenue for the margin. Include variable delivery, commissions and payment fees once. |
| Break-even revenue | Fixed costs ÷ positive contribution margin. With a non-positive margin, raising sales on the same assumptions cannot cover positive fixed costs. |
| Contribution after fixed costs | Contribution − fixed costs. Positive is a surplus under the entered monthly assumptions. |
| Collection and payment terms gaps | Compare observed collection and payment days with contractual or internal targets. Investigate ageing and overdue amounts before treating a timing difference as a missed payment. |
| Slow or obsolete stock | Carrying value identified through inventory ageing and recovery review. It is an exposure measure. |
| Stock after additional write-down | Net carrying value less the confirmed incremental write-down. Review net realisable value and previous provisions. A write-down reduces carrying value without creating a cash payment. |
| Owner-pay adjusted operating profit | Reported operating profit less the entered net increase in operating expenses to normalise owner remuneration. |
| E-commerce sales share | Net e-commerce sales ÷ comparable net reported sales, aligned for period, returns and VAT. |
| Electronic consumer payment share | Electronic consumer transactions ÷ total consumer transactions, by **count**, on the same retail scope and dates. |

### Repayment and financing

| Measure | Definition or action |
| --- | --- |
| Cash available for debt service (CFADS) | Enter reviewed next-12-month cash after operating costs, cash Zakat/tax and required cash capex, before included debt and lease service. Align the dates to the commitment schedule. |
| Existing and proposed debt service | Scheduled in-scope next-12-month cash service on existing commitments, plus quoted cash service for proposed financing. Read payment dates and individual amounts as well as the annual total. |
| Forward DSCR | CFADS ÷ (existing service + proposed service). At 1.00× projected cash exactly covers the included service. |
| Cash service headroom | CFADS ÷ required DSCR screen − total included service. Negative headroom is the service amount above the screen at the given CFADS. |
| Eligible undrawn facilities | Remaining availability on confirmed, committed and eligible facilities, subject to their terms. A draw enters the cash forecast when separately confirmed. |
| Covenant breach count and status | Count of failed tests against each agreement's direction, limit, definition and test date, alongside review status. |
| Weighted average principal maturity | Sum of scheduled principal × years to maturity ÷ included scheduled principal. |
| Current debt and lease portion | Current borrowings and lease liabilities ÷ total mapped borrowings and lease liabilities. |
| Evidence age and available bank cash | Days between evidence and assessment dates. Bank cash less restrictions is compared with the opening evidence on the matched date and scope. |

## How benchmarking works

FAFF shows three distinct comparisons. **Analyst screening profiles** classify historical ratios against transparent limits or target bands. A composite summarises the measures that qualify under the scoring logic and remains indicative. **Company operating targets** use the firm's own payment terms, minimum reserve and other policy inputs. **Peer bands** use reviewed comparison evidence for metrics where a direction is meaningful.

### How the historical score and flags are calculated

The scorecard averages the points earned per eligible ratio. The default points are **1.00 for Strong**, **0.75 for Above range**, **0.50 for Acceptable** and **0 for Weak**. The overall score pools the eligible ratios across groups. Missing and information-only measures are excluded from scoring. Review the count of scored ratios alongside the result. “Above range” can indicate an unusually large balance and deserves a look at the underlying assets and business needs.

The separate red-flag screen uses both levels and changes. It checks related-party exposure to equity and current assets, collection days, current ratio, year-over-year cash change, finance-cost cover and debt-to-equity. It also tests the percentage-point change in statutory burden and gross margin, net-margin decline during revenue growth, net-profit growth lagging operating EBIT growth, and monetary-position loss relative to revenue. Cash and stock flags cover CFO conversion, dividend cover, negative FCF after lease principal, the absolute adjusted CFO gap, adjusted CFO growth and the change in inventory days. The flag count uses computable tests. “Computable” requires the relevant inputs and a usable denominator.

### How to read the peer bands

For a peer comparison, match retail or wholesale, business scope, geography, size, reporting period and calculation basis. Record the sample size, source, date, reviewer and any exclusions. Enter **P25**, **median (P50)** and **P75** in numerical order. P25 is the value at the 25th percentile, rather than a judgement about quality. On a gross-margin metric, the strongest quartile is at the high end. On collection days, faster collection corresponds to the low end. DPO is displayed for context because a long payment period can reflect either agreed supplier terms or financial stress.

If reviewed peers are unavailable, leave the optional inputs blank. The workbook can show published international references for gross and operating margins. Its Statistics Canada 2024 references are retail gross **26.7%** and operating **5.7%**, and wholesale gross **17.1%** and operating **5.0%**. Treat them as Canadian sector aggregates. Saudi SME quartiles require a separate, comparable company sample. [Statistics Canada — retail survey](https://www150.statcan.gc.ca/t1/tbl1/en/tv.action?geocode=A000011124&pid=2010008301), [Statistics Canada — wholesale survey](https://www150.statcan.gc.ca/n1/daily-quotidien/260408/dq260408a-eng.htm)

In Saudi Arabia, local context can help explain changes in channels or payments. SAMA's national electronic-payment statistics are market context for transaction-count comparisons. GASTAT's wholesale and retail methodology explains its e-commerce sales growth indices, which measure change and have a different denominator from a company's e-commerce share. [Saudi Central Bank — electronic payments](https://www.sama.gov.sa/ar-sa/MediaCenter/News/Pages/news-1139.aspx), [GASTAT — wholesale and retail trade statistics](https://www.stats.gov.sa/en/w/methodology-and-quality-report-for-wholesale-and-retail-trade-statistics-4.1)

## Where to look first

1. **Founder View** · Check cash urgency, the first breach date and the three highest-priority actions. Then review contribution, peer position and evidence.
2. **Company Summary** · Read continuity and repayment capacity alongside CFADS, debt service, covenant status and facility availability. Check the source schedules before relying on the result in a credit discussion.
3. **Important Charts** · Start with available cash versus reserve and the weekly cash bridge. Next read monthly revenue versus break-even, operating cash quality and free cash flow. The remaining charts show liquidity, finance-cost coverage, working-capital days, margins, asset quality, capital structure, returns, turnover and historical screening results.
4. **Fundamental Analysis and ratio sheets** · Trace a flagged result to the relevant ratio, threshold, underlying statement and period.
5. **Model Review and XAZ Demo Guide** · Use the review tab for model notes and missing inputs. The XAZ workbook also includes the fictional data and scenario walkthrough.

## Validation and limitations

| Release verification | Result |
| --- | --- |
| English clean template | 397 assertions passed across eight suites. |
| English XAZ demo | 81 baseline assertions and 16 scenario assertions passed. |
| Newer bilingual release features | 22 assertions passed for historical reconciliation, margin comparisons and Saudi trading indicators. |
| English–Arabic XAZ comparison | Baseline plus six scenarios. Compared 68,770 numeric/date values and 289 mapped statuses, with no reported differences or unexpected formula errors. |

The tests cover the release fixtures and the scenarios described here. Forecast results depend on the dates, amounts and evidence users enter. Stress-test collections, supplier payments and financing separately and keep records of what changed. The model supports financial analysis and credit review. A lending decision also depends on verified borrower data, lender policy, covenants, collateral and other underwriting evidence. Screening settings such as the illustrative **1.25× DSCR** are editable assumptions. For statutory reporting and filing, apply the rules and accounting framework relevant to the business.

The founder workflow is designed for retail and wholesale. Manufacturing, production and service businesses can have different cost structures, working-capital patterns and peer definitions. Those use cases require their own operating assumptions and validation.
