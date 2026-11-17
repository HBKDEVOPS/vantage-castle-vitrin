# Method

[Türkçe](yontem.md)

This page describes Vantage Castle's four core quantities and its measurement records. All of it is measurement and arithmetic; none of it is a view on, or advice about, any share. Next to each number the source or the kind of measurement is written. The measurement records are not part of this repository; the method is described on this page on its own.

## 1. Input index

The weighted average price of the company's basket of input commodities, built on a base of 01.01.2015 = 100. For most companies the weights are a rank assumption: first input 50%, second 30%, third 20%. For the few companies with a measured proportion, the measured figure replaces the assumption. A component with no price series drops out of the basket, the remaining weights are rescaled, and the dropped share appears on the row as "input coverage". [Source: the product's calculation rule; the weights are a design choice]

A commodity may be more expensive today while the company keeps producing from older stock. Input prices are therefore shifted back by the company's inventory turnover period: the average of the last four to eight valid quarters, held between 0 and 365 days. The output price is not shifted. [Source: the product's calculation rule]

## 2. Output index

For most companies, the relevant sub-item of the TurkStat Domestic Producer Price Index, on the same 01.01.2015 = 100 base. [Source: TurkStat Domestic Producer Price Index]

## 3. Price–cost gap

The ratio of the output index to the input index. What is measured is price; it is not profit, sales volume or efficiency. The current value is shown together with its percentile within the company's own last five years of history, never as a bare number. It is read at the latest common date on which every component of the basket is known. [Source: the product's calculation rule]

## 4. Realised gross margin

(Revenue − cost of sales) ÷ revenue, taken from the three-month current-period column of the financial report published on KAP (the Public Disclosure Platform); it is not derived from cumulative differences. The product shows the realised margin beside the price–cost gap and puts no "because" between them: they are two separately observed series. [Source: the companies' financial reports published on KAP]

## 5. Projection: arithmetic, not a verdict

The Projection page calculates the arithmetic effect of a commodity move on the reported margin under "everything else held constant": volume, unmonitored cost items and price pass-through are assumed fixed. The commodity input effect is taken from the move of the input basket over a given window, read back by the inventory turnover period as in §1; in the product's settings the window is defined as 30, 90 and 180 days, and the example in the [margin flow diagram](../sema/marj-akisi.png) is the 90-day window. [Source: the product's calculation rule] Companies can absorb the effect through pricing, inventory, hedging and product mix. In the measured data the direction of the price–cost gap and the direction of the realised gross margin agreed in the same period 49.0% of the time (n=1492, 2015–2022), which cannot be told apart from a coin toss ([findings](findings.md)). The product therefore does not report share prices or an investment direction; it shows, as a record, the margin calculated from input cost, the interval, and its difference from the realised margin. This is a calculation, not a referee and not advice; the realised value is added beside it afterwards. [Source: §4 and §6 of this page; the direction-agreement measurement is on the [findings](findings.md) page]

## 6. Measurement record: FM-1 and Alfa

How well the arithmetic has held is measured by a forward record: the calculation is made and recorded before the financial statement is published, and the realised value is added beside it when it arrives. [Source: the product's measurement procedure] This repository does not contain the measurement records; what a reader can verify from it are the calculation rules on this page and the realised values the companies report on KAP.

- **FM-1** is a scenario calculation of the change in gross margin from the company's own financials (the name is the method's short name): one main figure and two scenario arms (a low arm and a high arm). The second face of the same method is a decomposition that places, side by side, the items the realised margin change was made of (commodities, sales price, volume, exchange rate, inflation accounting, inventory, other expenses); it gives no "the deviation came from this" verdict. [Source: the product's calculation rule]
- **Alfa** is the short name of a selection rule that chooses, per sector, whose main figure is shown, out of two methods (FM-1 and the product's earlier calculation engine, the "old engine"), with a rule written in advance; the rule looks at past direction agreement and is not changed after results are seen. [Source: the product's calculation rule]
- The third quarter of 2026 (Q3) is the first measurement of these records and it is not a referee: no method choice, pass/fail verdict or direction is drawn from Q3. Results are on the [findings](findings.md) page.

## 7. Interval and fallback rule (from 2026 Q4)

**Interval.** One half-width q is added on each side of the product's main figure: [main figure − q, main figure + q]. q is computed from that method's own past absolute errors (split conformal method; coverage 80%); there is no hand-set width per company or sector, the interval is not clipped, and errors are not pooled across methods. A method with a history of fewer than 30 companies gets the interval labelled "sample n=…: rough". The coverage guarantee rests on the errors coming from the same distribution; that assumption has not been measured from Q3 to Q4. [Source: the product's calculation rule; formula: Angelopoulos and Bates, arXiv 2107.07511]

The 80% half-widths computed from the Q3 errors (in-sample, not evidence): ±7.994 points for FM-1 (n=50) and ±21.846 points for the old engine (n=10, rough). [Measurement: calculation made on 15.11.2026 on the realised margins reported for 2026 Q3]

**Fallback rule.** If the method Alfa chose produced no result for a company-quarter: (1) if the company has an FM-1 record, the product shows it labelled "no Alfa output; fallback: FM-1", and that figure is never called Alfa's figure; (2) if there is no FM-1 record either, the product says there is no model output and shows, as a reference, the company's most recently reported three-month realised gross margin on KAP; that reference counts as no method's figure and enters neither the interval nor any measurement. [Source: the product's calculation rule]

**Honesty note.** The interval and fallback rules were written after the Q3 results were seen; they are therefore no retroactive evidence for Q3. The first real test is 2026 Q4, where coverage is only descriptive: "n=…, k=…" is written and no "held / did not hold" verdict is given. [Source: the product's calculation rule]

## Limits

- Most basket weights are assumptions; a measured proportion exists only for a few companies.
- The monitored basket is not the whole cost; labour and depreciation are not in it.
- Companies that share the same input basket and the same output index have a numerically identical price–cost gap; the product flags this as an "identical series" and claims no difference between them.
- Q3 is one quarter and 40–50 companies; a shock common to the quarter may have moved all of them in the same direction.
