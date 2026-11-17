# Method

[Türkçe](yontem.md)

This page describes the four basic quantities of Vantage Castle and the Commodity Margin Engine that makes the calculation. All of them are measurements and calculations; none is a view on a share. This is not investment advice. Beside the numbers, the source or the type of measurement is written. The measurement records are not in this repository; the method is described on this page on its own.

## 1. Input index

The weighted average price of the company's input commodity basket, built on a 01.01.2015 = 100 base. For most companies the weights are a rank assumption: first input 50%, second 30%, third 20%. For the few companies with a measured share, the measured share replaces the assumption. A component whose price series cannot be found drops out of the basket, the remaining weights are rescaled and the dropped share appears in the row as "input coverage". [Source: the product's calculation rule; the weights are a design choice]

Even if a commodity gets more expensive today, a company keeps producing from old stock for a while. Input prices are therefore taken back by the company's inventory turnover period; the period is the average of the last four to eight valid quarters and is held between 0 and 365 days. The output price is not taken back. [Source: the product's calculation rule]

## 2. Output index

For most companies, the relevant sub-item of the TÜİK (Turkish Statistical Institute) Domestic Producer Price Index; built on the same 01.01.2015 = 100 base. [Source: TÜİK Domestic Producer Price Index]

## 3. Price–cost gap (the "scissors")

The ratio of the output index to the input index. What is measured is price; it is not profit, sales volume or efficiency. The current value is shown together with its percentile in the company's own last five years of history; it is not presented as a number on its own. The value is read at the latest date on which every component of the basket is known. [Source: the product's calculation rule]

## 4. Realised gross margin

(Revenue − cost of sales) ÷ revenue; taken from the three-month current column of the financial report the company publishes on KAP, not derived from a cumulative difference. The product shows the realised margin beside the price–cost gap and puts no "therefore" between them: they are two separately observed series. [Source: the financial reports companies publish on KAP]

## 5. Projection: a calculation, not a verdict

The Projection page calculates the arithmetic effect of a commodity move on the financial-statement margin under "everything else held constant"; volume, unobserved cost items and price pass-through are assumed constant. The commodity input effect is taken from the move of the input basket over a given window, and the basket is read back by the inventory turnover period as in §1; in the product's settings the window is defined as 30, 90 and 180 days, and the example in the [margin flow diagram](../diagrams/marj-akisi.png) uses a 90-day window. [Source: the product's Projection page, 17.11.2026] Companies can absorb the effect through pricing, inventory, hedging and product mix. In past measurements no agreement distinguishable from a coin toss was found between the direction of the price–cost gap and the direction of the realised gross margin ([Honest findings](findings.md)). The product therefore does not report a share price or an investment direction; it shows, as a record, the margin calculated from input cost, the band and its difference from the realised margin. This is a calculation, not a referee and not investment advice; the realised value is added beside it afterwards. How the calculation is built is described in the [Commodity Margin Engine](method.md#commodity-margin-engine) section.

## Limits

- Most basket weights are an assumption; a measured share exists only for a few companies.
- The basket followed is not the whole of cost; labour and depreciation are not in the basket.
- Companies sharing the same input basket and the same output index have numerically identical price–cost gaps; the product marks this as an "identical series" and claims no difference between them.
- The forward-record measurement still rests on a very short history; a common quarterly shock may have moved all companies in the same direction.
## Commodity Margin Engine

Every number on the Projection page is calculated by the Commodity Margin Engine. Before a financial statement is published, the engine calculates, in the light of commodity moves and the company's own structure, where a company's gross margin could land in the next statement, and records it; when the realised value arrives, it is added beside the record. This is a calculation: it says nothing about a share price or an investment direction, it is not a referee and it is not investment advice. [Source: the product's Projection page and the team's method document; the document is not in this repository]

### What it calculates and what it does not

The engine answers a single question: "If everything else stays constant, by how many points does the known commodity move shift the company's gross margin?" The notice at the top of the page says so: "Bu bir hesaptır, yön iddiası değildir" (this is a calculation, not a claim about direction). Volume, the company's unobserved cost items and price pass-through are held constant. The engine nowhere produces a share price or a trading verdict. [Source: the product's Projection page, 17.11.2026]

### Three inputs

The engine looks at three things:

1. **The company's financials.** Quarterly revenue, cost of sales and gross profit published on KAP; the inventory turnover period; the effect of inflation accounting (IAS 29, "TMS 29" in Turkish practice).
2. **The company's commodities.** The official-series prices of the commodities in the company's input basket. Prices are read back by the inventory turnover period: today's price move reaches the financial statement only as the stock runs down.
3. **Input–output.** The price of the input basket and the output price series closest to what the company sells are put side by side; the difference between them forms the output effect in the calculation.

[Source: the product's Projection page, "Sebepler: sayı akışı" (reasons: number flow) section, 17.11.2026; the team's method document]

### Two methods, one screen

For every company the Projection · Commodity page shows the result of two methods in separate blocks: **"Emtia fiyatından" (from commodity prices)** and **"Şirket finansallarından" (from company financials)**, the latter marked "ön kayıtlı yöntem" (pre-registered method). The two blocks appear separately on screen. The team's method document ties which of the two is shown as the main figure to a selection rule written in advance, sector by sector. This selection rule is planned from the fourth quarter of 2026 and is not yet visible on screen. [Source: the product's Projection · Commodity and Realised pages, 17.11.2026; the team's method document]

### The "from commodity prices" method

It shows the path from the previous margin to the calculated margin step by step; the order in the screen's "Sebepler" (reasons) section is:

- **Input side.** Price change of the input basket → inventory lag (it shifts the window of the commodity change; it is not a separate margin term) → cost coefficient (how much of the change in the input basket shows up in cost) → change passed to cost → output pass-through ratio (how much of the cost change shows up in the selling price) → change passed to sales revenue → input effect on the gross margin.
- **Output side.** The difference between the output basket (the output price series, for most companies the relevant sub-item of the TÜİK Domestic Producer Price Index) and the input basket → output effect on the gross margin.
- **Result.** The previous quarter's margin + the input effect + the output effect = the calculated margin. The page's "Marj akışı" (margin flow) diagram draws the same order.

The base of this method is the previous quarter. [Source: the product's Projection · Commodity page, 17.11.2026; the team's method document]

### The "from company financials" method

This method starts from the company's own past financial behaviour:

- **Base.** The value of the same quarter a year earlier, so that seasonality does not enter the calculation.
- **Real input shock.** The price change of the input basket, stripped of the change in the consumer price index over the same window and read back by the inventory lag.
- **Two coefficients.** The input response (how much of the real shock shows up in cost) and the sales pass-through (how much of the real cost change shows up in real sales) are estimated from the company's own past quarters. The history that sets the coefficients ends on a date frozen in the pre-registration and does not change in the forward record.
- **Three arms.** The low arm assumes no pass-through to sales, the middle arm the company's past behaviour, the high arm the high pass-through observations in the company's history. On screen they appear as the "Senaryo hesabı (orta)" (scenario calculation, middle) and "Bant (alt – üst)" (band, low – high) rows; the band is the smallest and the largest of the three arms. The team's method document calls these three results "scenario arms"; because the names on screen are "Senaryo hesabı (orta)" and "Bant (alt – üst)", this document uses the name on screen.
- **Out of range.** If the calculated input shock falls outside the range of the history that set the coefficient, the value is not clipped or changed; the screen writes "aralık dışı" (out of range) and shows only the band.
- **Could not be measured.** If the data are not enough, the engine does not invent a number; it writes the reason: "kapsam düşük" (coverage low), "geçmiş yetersiz" (history insufficient), "taban doğrulanmadı" (base not verified), "girdi tepkisi ölçülemiyor" (input response cannot be measured), "benzer durum yok" (no similar case) or "girdi serisi yok" (no input series). These company-quarters are not dropped from the list; they are counted as "could not be measured".
- **Output check.** The change in sales derived from the financials is compared with the change in the market output price, and "piyasayla aynı" (same as the market), "piyasanın önünde" (ahead of the market) or "piyasanın gerisinde" (behind the market) is written. This check does not enter the calculation; because the sales amount also contains volume and product mix it carries an "approximate" label, and a "proxy" label if the series stands in for the company only indirectly.

In the internal evaluation the criterion is direction; the screen has no count of right or wrong directions, no rate and no success sentence. [Source: the team's pre-registered method document; the product's Projection · Commodity page, 17.11.2026]

### Decomposition: an internal research method (not yet in the product)

The team's method document describes how, after a financial statement is published, a company's actual gross margin change is split into parts: commodity and raw material, selling price and product mix, volume, exchange rate, inflation accounting (IAS 29), inventory effect and other expenses. This is an internal research method; it is not yet in the product and no decomposition appears on any screen. The method document is not an execution order: execution starts with a separate request and a human decision. According to the document, the parts are built from quantities that can be read openly in the notes of the financial report on KAP; volume (units) is taken from the company's interim operating report or from the sales-volume disclosure on KAP, and the price is derived from them, because the financial statements give no unit volume. Whether every company's interim operating report gives quarterly unit volume has not been verified. A part that cannot be read is not invented but written into a "remainder" row. The order is frozen from the start: first volume, then price, then cost. The difference between the official base and the decomposition base is written as a separate "base gap" row and is not mixed into the remainder. The decomposition is descriptive: it does not give a verdict that "the deviation came from this". [Source: the team's method document v1.3, §5, §6, §9, §10 and open point §11.2; the document is not in this repository]

### Reference margin on screen today; interval and fallback rule planned (not yet on screen)

**On screen today: reference margin.** If there is no model output for a company-quarter, the screen states that there is no model output and shows, as a reference, the company's most recently published three-month realised gross margin on KAP (Projection · Realised). This reference is not counted as any method's figure and does not enter any measurement. [Source: the product's Projection · Realised page, 17.11.2026; the team's method document]

**Planned, not yet on screen: interval.** The team's method document and its interval annex provide that, from the fourth quarter of 2026, a single half-width q is added on both sides of the main figure for every company and every method: [main figure − q, main figure + q]. q is to be calculated from that method's own past absolute errors (split conformal method; coverage 80% (design choice)); there is no hand-set width for a company or a sector, no clipping, and no pooling of errors across methods. For a method with a short history the interval is expected to come with the label "örnek n=…: kaba" (sample n=…: rough). The coverage guarantee rests on the assumption that the errors come from the same distribution; this assumption has not been measured. Today's screen has no such interval, no q and no such label: it shows only the "Bant (alt – üst)" (band, low – high) row, which, as described above, is the smallest and largest of the three arms and is not an interval calculated from past errors. [Source: the team's method document and interval annex v1.0, in force from 2026 Q4; formula: Angelopoulos and Bates, arXiv 2107.07511; the product's Projection · Commodity page, 17.11.2026]

**Planned, not yet on screen: fallback rule.** According to the document, if the method chosen by the selection rule gave no result for a company-quarter: (1) if the "from company financials" result exists for that company, the product will show it with a "fallback" label, and the fallback figure will not be called the chosen method's figure; (2) if that does not exist either, the product states that there is no model output and shows the reference margin (the behaviour above, which is on screen today). Today's screen has no "fallback" label. [Source: the team's method document v1.3, in force from 2026 Q4; the product's Projection pages, 17.11.2026]

**Honesty note.** The interval and the fallback rule were written after the results of the first forward-record measurement were seen; they are therefore not retroactive evidence for that measurement. The first real test is the fourth quarter of 2026, and there coverage will be only descriptive: "n=…, k=…" is written and no "held / did not hold" verdict is given. [Source: the team's method document]

### What is not yet calculated

The **Macro** view of Projection (the effect of the exchange rate and inflation) and its **Operational** view (the effect of volume, capacity and hedging) are not yet calculated; the screen says so plainly with "henüz hesapta değil" (not yet calculated), and these effects enter none of the engine's numbers. [Source: the product's Projection · Macro and Operational pages, 17.11.2026]

### Limits

- Most basket weights are an assumption; the basket followed is not the whole of cost.
- The change in sales is an amount response: volume and product mix are not shown separately.
- For some companies coverage, history or base is not enough; the engine writes "could not be measured" there.
- Inflation accounting (IAS 29) and the lira column of companies whose functional currency is the dollar or the euro are separate special cases that affect the calculation; the method document keeps them apart explicitly.
- The method document and the pre-registrations are frozen before results are seen; a change is a new document and a new version, and the old version does not change.
