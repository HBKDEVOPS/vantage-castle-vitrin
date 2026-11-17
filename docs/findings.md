# Honest findings

[Türkçe](bulgular.md)

The most important design decision in Vantage Castle is what it does not say. The measurements below tested whether a margin or a share-price-series change can be derived from commodity prices; none found a meaningful relationship. The product therefore expresses no view; it puts what it measures side by side.

The measurements that use share prices are an internal study made on recorded series. "No relationship" here means "not found with this data and this method"; it is not proof that no relationship exists.

## Paths tried and dropped (six measurements)

The "Data" column shows which kind of recorded series each measurement rests on. These are the product's own internal measurements; their detailed records are not part of this repository.

| # | Measurement | Result | Data |
|---|---|---|---|
| 1 | Regression pipeline: per company and in a single model, margin and share-price-series change from commodity change | No meaningful power; out-of-sample (after 2023) explanatory power negative, i.e. worse than a plain average | Commodity, margin and share price series |
| 2 | Does the direction of the price–cost gap agree with the direction of realised gross margin in the same period? | **49.0%** (n=1492, 2015–2022); indistinguishable from a coin toss; no lag or alignment correction passed the 55% threshold | Price–cost gap and KAP margin, 2015–2022 |
| 3 | Sector-neutral reverse-ordered two-group difference: the difference in share-price-series change between a group of the companies where the gap measure is most favourable and a reverse-ordered group of those where it is least favourable | Difference t = **0.613**, p = **0.543**; indistinguishable from noise | Price–cost gap and share price series |
| 4 | Pricing-in measurement: when the gap changed markedly, how did the share price series separate from its sector peers? | No relationship found | Price–cost gap and share price series |
| 5 | Inventory turnover: does the turnover period move together with commodity prices? | No relationship found; the fixed-turnover assumption is therefore kept | Commodity prices and KAP financial reports |
| 6 | KAP event study: after a disclosure, does the share price series separate from its sector more than usual? | Looks only at the size of the separation, not its direction | KAP disclosures and share price series |

Two more paths were dropped: the "episode table" that matched periods of large gap changes with the following margin was removed (it would have presented an unproven relationship as proven), and an attempt to convert financial statements to a common base using consumer prices failed and was not applied to the tables.

## News direction label measurement (not shown on any product page)

News items were given a direction label, and it was checked whether the price series then changed in the same direction; the plan was written and frozen before labelling started. Result: the label direction and the following price-series direction agreed 51.2%, 50.3% and 51.5% of the time over 1, 5 and 20 trading days (a coin toss gives 50%); against a significance threshold of p < 0.0045 the p-values were 0.449, 0.873 and 0.366 (n = 1,029, 1,034 and 1,038 independent clusters). None is significant. [Measurement: 10.10.2026; news labels and share price series]

Two limits are stated openly: with this data an effect above about 55.8% could be excluded, and a smaller effect cannot be told apart; agreement between the two labellers was moderate (κ 0.570–0.657), so the result was recorded as "weak evidence of absence", not "no relationship for certain". No look-ahead violation was found (0). This measurement does not enter the product; the labels are shown on no screen.

## First forward-record measurement: 2026 Q3 (not a referee)

Calculations are made and recorded before the financial statement is published, and the realised KAP value is added beside them when it arrives. For the third quarter of 2026, 50 companies were examined. Q3 is not a referee: no method choice or pass/fail verdict is drawn from these tables.

Two short names appear in the table; both are defined on the [method](method.md) page. Alfa is the selection rule that chooses, per sector, which of two methods' main figure is shown, with a rule written in advance. FM-1 is the calculation of the change in gross margin from a company's own financials, with a main figure and two scenario arms, a low and a high one.

| Measurement | Result | Data |
|---|---|---|
| Mean absolute error of the main figure of the method Alfa chose, against realised margin (40 companies that have a figure) | **5.855 points**; under the assumption "margin stays as in the previous quarter", 7.140 points; medians 3.836 ↔ 3.830; Alfa closer in 20 companies, the simple assumption closer in 20 | 2026 Q3: the product's recorded calculations ↔ realised margins reported on KAP; 15.11.2026 |
| Same measurement in FM-1 sectors (35 companies) | 5.295 ↔ 7.057 points (Alfa closer in 19, simple closer in 16) | Same data |
| Same measurement in old-engine sectors (only 5 companies have a figure) | 9.776 ↔ 7.724 points (Alfa closer in 1, simple closer in 4) | Same data |
| Share of realised values falling between FM-1's low and high scenario arms | 19 / 49 (0.388); arms in order 11 / 29, arms in reverse order 8 / 20 (for reverse-ordered arms the interval was taken between the smaller and the larger value) | Same data |

Reading notes: (1) A few extreme values pull the mean up; the medians are almost identical. (2) Alfa's selection rule looks at direction agreement, not at mean absolute error; the error here is an additional descriptive measure. (3) In 10 companies the old engine has no figure, so Alfa has no output; coverage is 40/50. (4) In the old-engine arm the simple assumption is closer in 4 of 5 companies; this says nothing about so small a sample. (5) If KAP's three-month Q2 column is used instead of the Q2 value in the database, the simple assumption's error is 7.159 (sensitivity row). (6) One quarter; a common shock may have moved the companies in the same direction.

## How these findings shaped the product

The product gives no share price or investment direction and no trading advice, and it makes no statement about condition or direction such as "the gap narrowed, margin pressure exists"; it puts the input index, the output index, the price–cost gap and the realised gross margin side by side without implying causation. It shows, as a record, the margin calculated from input cost, the interval, and its difference from the realised margin; this is a calculation, not a referee and not advice. This is not a stylistic preference; it is the result of the measurements above. The system puts what it measures side by side and leaves the interpretation to the reader.
