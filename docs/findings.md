# Honest findings

[Türkçe](bulgular.md)

Vantage Castle's most important design decision is what it does not say. The measurements below tried to find out whether margin or a change in share price series can be derived from commodity prices; none found a significant relationship. The product therefore expresses no view; it shows what it measures side by side.

The measurements that use share prices are internal work done on commodity, margin and share price series. "No relationship" here means "could not be found with this data and this method"; it is not proof that no relationship exists.

## Paths tried and dropped (six measurements)

The "Data" column shows what kind of data the measurement rests on. These are the product's own internal measurements; their detailed records and numbers are not in this repository.

| # | Measurement | Result | Data |
|---|---|---|---|
| 1 | Regression pipeline: from the commodity change to the change in margin and in the share price series, company by company and in a single model | No significant power; explanatory power in the out-of-sample period is negative, that is, worse than a simple average | Commodity, margin and share price series |
| 2 | Does the direction of the price–cost gap match the direction of the realised gross margin in the same period? | The agreement could not be distinguished from a coin toss; no lag or alignment correction passed the threshold | Price–cost gap and KAP margin, past years |
| 3 | Sector-neutral reverse-ordered two-group difference: the difference in the change of the share price series between a group made of the companies with the most favourable gap measure and a reverse-ordered group made of those with the least favourable | The difference could not be distinguished from noise | Price–cost gap and share price series |
| 4 | Pricing-in measurement: when the gap changed markedly, how did the share price series separate from sector peers? | No relationship found | Price–cost gap and share price series |
| 5 | Inventory turnover: does the inventory turnover period change together with commodity prices? | No relationship found; the constant inventory turnover assumption is therefore kept | Commodity price and KAP financial reports |
| 6 | KAP event study: after a filing, does the share price series separate from its sector more than normal? | Looks only at the size of the separation, not its direction | KAP filings and share price series |

Two further paths were dropped: the "episode table", which matched periods of large change in the price–cost gap with the following margin, was removed (it would have shown an unproven relationship as proven), and the attempt to convert financial statements to a common base with consumer prices failed and was not applied to the tables.

## News direction label measurement (not on the product's pages)

News items were given a direction label and it was checked whether the price series then moved in the same direction; the plan was written and frozen before labelling began. Result: the agreement between the label direction and the following price series direction could not be distinguished from a coin toss at any of the three horizons (short, medium and long trading-day horizons); none of the three passed the significance threshold written in advance. Agreement between the labellers was moderate, so the result was recorded as "weak evidence of absence", not "no relationship for certain". This measurement does not enter the product; the labels are not shown on any screen. [Measurement: the team's internal measurement, 10.10.2026; news labels and share price series]

## Forward-record measurement (not a referee)

Calculations are made and recorded before the financial statement is published; when the realised value arrives, it is added beside them. The first forward-record measurement was made for the third quarter of 2026. This measurement is not a referee: no method choice or pass/fail verdict is drawn from it. Its numbers are not in this repository; the product's screens show the record and the realised value side by side ([Commodity Margin Engine](method.md#commodity-margin-engine)).

## How these findings shaped the product

The product reports no share price or investment direction, gives no trade instructions, and makes no claim about a state or a direction such as "the gap has narrowed, there is margin pressure"; it puts the input index, the output index, the price–cost gap and the realised gross margin side by side without implying causality. It shows, as a record, the margin calculated from input cost, the band and its difference from the realised margin; this is a calculation, not a referee and not investment advice. This is not a stylistic preference but the result of the measurements above. The system shows what it measures side by side and leaves the interpretation to the reader.
