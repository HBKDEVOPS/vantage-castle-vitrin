<p align="center">
  <img src="ekran/vitrin-hero.gif" alt="Vantage Castle: an animated tour of the My board, Map, Commodities and Commodity Network screens" width="100%">
</p>

# Vantage Castle

[Türkçe](README.md)

**How do commodity prices show up in a company's margin? On one screen, with the source next to every number.**

Vantage Castle puts the input commodity cost and the output price of Borsa Istanbul companies on the same axis and places, beside them, the gross margin the company has actually reported. Did a company's raw-material basket get more expensive, and did the price of its product cover it: both are visible side by side. The margin calculated from input cost, and its interval, are recorded before the financial statement is published; when the realised value arrives, it is added beside them. The measurement is thereby fixed by the record.

- **My board (Panom).** Your own tracking screen; you choose the windows.
- **Map.** World news linked to companies' commodity exposure.
- **Companies.** Margin flow: input items, the input basket and the margin gap in one diagram.
- **Commodities.** Commodity prices, with the selected series' chart, its source and unit.
- **Changes.** What has changed since the date you choose, on one page.
- **Bulletin.** The weekly bulletin: commodity moves, margins and the effect matrix.
- **Projection.** The arithmetic effect of a commodity move on the gross margin; a calculation, not a claim about direction.
- **Sectors.** Sector margins, the commodities tied to sectors and the input matching matrix.
- **Commodity Network.** Which commodity is tied to which sectors.
- **Supply Chain.** From which countries, and along which routes and transit points, a company's input commodities arrive in Türkiye (Türkiye-wide imports).
- **KAP, Data quality, Terms, Screening.** The filings list, each company's data status, a glossary and a one-table screening of all companies.

This repository is a showcase: it contains no code and no data. The page images were taken in the product's masked mode: share prices, KAP (Public Disclosure Platform) filings, financial statement tables, news headlines, electricity (EPİAŞ) and chokepoint (PortWatch) values, and account details do not appear in them; "—" or a blank stands in their place. The interface is in Turkish.

## Contents

- [What it does](#vantage-castle)
- [Screens](#screens): [My board](#my-board-panom) · [Map](#map) · [Companies](#companies) · [Commodities](#commodities) · [Changes](#changes) · [Bulletin](#bulletin-bülten) · [Projection](#projection-projeksiyon) · [Sectors](#sectors-sektörler) · [Matching matrix](#matching-matrix-eşleşme-matrisi) · [Commodity Network](#commodity-network) · [Supply Chain](#supply-chain) · [KAP](#kap) · [Data quality](#data-quality-veri-kalitesi) · [Terms](#terms-terimler) · [Home page](#home-page-ana-sayfa) · [Sign in](#sign-in-giriş) · [Sign up](#sign-up-kaydol) · [About us](#about-us-hakkımızda) · [Screening](#screening-tarama)
- [Method](#method)
- [Honest findings](#honest-findings)
- [Architecture](#architecture)
- [Team](#team)
- [What it does not do](#what-it-does-not-do)
- [Licence and attributions](#licence-and-attributions)

The Method, Findings, Architecture and Team sections each have a short summary; the full text is inside the "Details" box.

## Screens

The pages are given in the order of the product's left-hand menu and by the file number of the images (01, 02, …). The images contain no share prices, KAP filings, financial statement tables, news headlines, electricity (EPİAŞ) or chokepoint (PortWatch) values, or account details; "—" or a blank stands in their place. The interface is in Turkish.

### My board (Panom)

Your own tracking screen; you choose the windows. Favourite companies, a commodity chart, a heat calendar, exchange rates and bulletins on one board. You save your layout and switch between layouts with Alt+1–9. You pick windows from companies, commodities and your pages; a new window goes to the first free place.

![My board: commodity lists, price chart, commodity card and heat calendar](ekran/01-panom.png)

### Map

World news linked to companies' commodity exposure. Whichever commodity a news item affects, the companies that carry that commodity in their input basket appear side by side on the map. The arrows show the direction of the relationship the news describes; they are not a claim of effect. In the image the news headlines appear as "—"; the map, news clusters, arrows, chokepoints and crisis files remain.

![Map page: news clusters, relationship arrows, chokepoints and crisis files](ekran/02-harita.png)

### Companies

The selected company's page: margin flow, input and output index, input prices, the Projection summary and the financial table on one page. Share price, volume, KAP and financial statement values appear as "—" in the image.

![Companies page: margin flow, input and output index, input prices, Projection summary and financial table; values shown as "—"](ekran/03-sirketler.png)

Margin flow: the output price is taken as 100; the input items flow in from the left as separate bands, each with its share in the basket written beside it. The bands join in the input basket; once the basket's share is taken from the output, what remains goes to the margin gap box. Macro quantities such as the interest rate and the exchange rate sit outside the basket, in a separate corridor. The "Bugün" (today) view shows the latest record; in the "Ya şöyle olursa" (what if) view you give the change of an input item yourself and the flow is redrawn with the same calculation (output price held constant). The basket share comes from the gross margin in the financial report the company publishes on KAP, and the item weights from the product's calculation rule ([Method §1 and §4](#method)). The numbers in the flow derive from the gross margin the company publishes on KAP, so they appear as "—" in the image; the thickness of the bands shows only the layout.

![Margin flow panel of the Companies page: input items, input basket and margin gap; numbers shown as "—"](ekran/03-sirketler-marj-akisi.png)

The order of the flow, in a diagram that carries no values: the commodity input effect and the commodity output effect are added to the previous margin; the result is the calculated margin. Its labels are in Turkish. The 90-day window in the input effect is an example (in the product's settings the window is 30, 90 and 180 days; details in [Method §5](#method)).

![Margin flow diagram](sema/marj-akisi.png)

### Commodities

Commodity prices, with the selected series' chart, its source and unit. The page has a commodity card strip, a commodity list, the selected series' chart, a heat calendar and a horizon chart.

![Commodity page: commodity card strip, commodity list, butane chart, heat calendar and horizon chart](ekran/04-emtia.png)

### Changes

What has changed since the date you choose. Commodity prices, unusual moves, exchange rates and bulletins are on one page over the range you pick; every row leads to its source. The image shows the 90-day range.

![Changes page, 90-day range: commodity prices, unusual moves, exchange rates and bulletins](ekran/05-degisimler.png)

### Bulletin (Bülten)

The weekly bulletin: commodity moves, published financial statements, companies' gross and net margins, the commodity–company effect matrix and the Projection records on one page. The numerical measurements are produced automatically; a published bulletin is not changed afterwards, and a correction is made in a new issue. Margins and numbers appear as "—" in the image.

![Bulletin page: weekly bulletin summary, margin table, commodity moves and commodity–company effect matrix; numbers shown as "—"](ekran/06-bulten.png)

### Projection (Projeksiyon)

It calculates the arithmetic effect of a commodity move on the gross margin under "everything else held constant"; the notice at the top of the page says that this is a calculation and carries no claim about direction ([Method §5](#method)). The page has five views; numbers appear as "—" in the images.

**Commodity (Emtia).** The effect of the commodity move on the margin, step by step, on the input and the output side; the margin flow runs from the previous margin to the calculated margin.

![Projection, Commodity view: margin flow and a step-by-step breakdown of the input and output effects](ekran/07-projeksiyon-emtia.png)

**Macro (Makro).** The effect of the exchange rate and inflation on the gross margin; in the image these effects read "henüz hesapta değil" (not yet calculated).

![Projection, Macro view: exchange rate and inflation effects not yet calculated](ekran/07-projeksiyon-makro.png)

**Operational (Operasyonel).** The effect of volume, capacity and hedging; in the image these effects read "henüz hesapta değil" (not yet calculated).

![Projection, Operational view: volume, capacity and hedge effects not yet calculated](ekran/07-projeksiyon-operasyonel.png)

**Scenario calculation (Senaryo hesabı).** You give the change for the input basket and the output basket (a slider or a percentage box); everything else stays constant and the margin flow is redrawn with the same calculation.

![Projection, Scenario calculation view: sliders for the input and output basket, margin flow and step-by-step breakdown](ekran/07-projeksiyon-senaryo.png)

**Realised (Gerçekleşen).** For companies that have published their financial statements it places the recorded calculation beside the realised margin; for a company with no record there is no model output, and the latest quarter's realised margin is shown as a reference ([Method §7](#method)).

![Projection, Realised view: recorded calculation beside the realised margin for companies that have published; values shown as "—"](ekran/07-projeksiyon-gerceklesen.png)

### Sectors (Sektörler)

Choosing a sector shows the sector's gross margin, the change in the margins of the companies in it, and the commodities tied to the sector; in the image the margin charts read "henüz hesapta değil" (not yet calculated) and the sector–commodity matrix remains. In the matrix the number is the count of companies carrying that commodity in their basket; the shade is their share among the sector's companies.

![Sectors page: sector selector, margin panels and the matrix of commodities tied to sectors](ekran/08-sektorler.png)

### Matching matrix (Eşleşme matrisi)

It shows, in one table, whether each company's each input is matched directly or by a proxy series. The rows are companies (ticker and sector) and the columns are commodities; the three counters at the top count the companies with a full match (no proxy), with at least one proxy match, and with no input data at all. The sector and commodity selectors and the "Tümü" (all), "Sadece doğrudan" (direct only) and "Sadece proxy" (proxy only) buttons filter the table. An asterisk is a proxy match and "—" means no data. In the image the numbers in the counters and the cells appear as "—"; the table scrolls sideways, so only its left part is in the frame. [Source: the product's Matching matrix page]

![Matching matrix: companies in rows, commodities in columns; an asterisk marks a proxy match; numbers shown as "—"](ekran/08-eslesme-matrisi.png)

### Commodity Network

Which commodity is tied to which sectors, in a single network view. The links come from the companies' input baskets; most basket weights are an assumption ([Method §1](#method) and [Limits](#method)).

![Commodity Network: commodities on the upper layer, companies on the lower layer; dashed lines are proxy matches](ekran/09-emtia-agi.png)

### Supply Chain

From which countries of origin, and along which routes and transit points, the selected company's input commodities arrive in Türkiye. The page is an eight-step walk-through: 1 Company (Şirket), 2 Inputs (Girdiler), 3 Domestic and country (Yerli ve ülke), 4 Routes (Yollar), 5 Transits (Geçişler), 6 One country (Bir ülke), 7 One point (Bir nokta), 8 Transit share (Geçiş payı); the images (example: Ereğli) show the fifth step, the question "which transits are on the route, and how many ships pass per day?". The page shows Türkiye-wide imports; it does not mean the company's own supplier, and most shares carry an "approximate" label. Box sizes follow the input's share in the basket and its share within imports; most basket weights are an assumption ([Method §1](#method)). [Source: the explanatory text on the product's Supply Chain page]

![Supply Chain page, Ereğli, step 5 Transits: route map, layered network and the company's own statement panel](ekran/10-tedarik-zinciri.png)

**Route map.** A schematic sea map: lines from the countries of origin to Türkiye (iron ore and bituminous coal in separate colours) and the transit points on the way (Gibraltar, Suez, Bab el-Mandeb, the Turkish Straits). The lines are schematic, not an actual voyage; domestic production and land or pipeline imports are not drawn on the map and stand as separate branches in the network. The table below the map holds the daily transit counts of the chokepoints (IMF PortWatch medians); in the image in this repository these counts appear as "—".

![Route map and chokepoint table; transit counts shown as "—"](ekran/10-tedarik-guzergah.png)

**Layered network.** The flow is given in company, input, domestic share plus country of origin, and transit point columns; hovering over a link or a node says what it carries and the route is highlighted on the map.

![Layered network: company, input, domestic share and country of origin, transit point columns](ekran/10-tedarik-ag.png)

**The company's own statement.** This panel at the bottom of the page shows the supplier countries and the self-sufficiency statement from the company's own document separately from the Türkiye-wide data; the two sides are not calculated from each other. In the image in this repository the panel's fields appear as "—".

### KAP

The page listing KAP filings, which can be filtered by company, sector and filing type. The image shows no filings; the list is empty.

![KAP page: filters and an empty filing list](ekran/11-kap.png)

### Data quality (Veri kalitesi)

Is each company's data good enough for the calculation? Every company's data passes a screening: those that remain enter the calculation, those with a warning enter with a note, those eliminated do not, and those followed only on the output side are marked separately; each company's input coverage is written beside it.

![Data quality page: data status and input coverage per company](ekran/12-veri-kalitesi.png)

### Terms (Terimler)

Short definitions of the words on the screens; clicking a term opens its calculation and reading note.

![Terms page: glossary with short definitions](ekran/12-terimler.png)

### Home page (Ana sayfa)

The product's public home page: it explains what the product measures, gives a short tour of the pages and answers frequently asked questions. The image is the full length of the page (about 11 MB), so it is not shown inline: [ekran/13-anasayfa.png](ekran/13-anasayfa.png).

### Sign in (Giriş)

The sign-in page for users with an account; the form is empty in the image.

![Sign-in page: empty e-mail and password fields](ekran/14-giris.png)

### Sign up (Kaydol)

The account application page: the application goes to administrator approval, and the page says what an account opens and what it does not. The form is empty in the image.

![Sign-up page: empty application form; what an account opens and what it does not](ekran/15-kaydol.png)

### About us (Hakkımızda)

What the product is, what it does, what it does not do and how it approaches data, in four boxes.

![About us page: what Vantage Castle is, what it does, what it does not do, how it approaches data](ekran/17-hakkimizda.png)

### Screening (Tarama)

All companies in one table: the 90-day input and output change, the price–cost gap (90-day change, five-year historical position, size of the move) and the data status; companies sharing an identical series are grouped. Values appear as "—" in the image.

![Screening page: input, output and price–cost gap columns and data status per company; values shown as "—"](ekran/19-tarama.png)

## Method

Four quantities sit side by side: the **input index** (the weighted price of the company's basket of input commodities, base 01.01.2015 = 100, read back by the inventory turnover period), the **output index** (for most companies, the relevant sub-item of the TurkStat Domestic Producer Price Index), the **price–cost gap** (output index over input index) and the **realised gross margin** (from the quarterly financial report the company publishes on KAP). No "because" is put between them; they are separately observed series. The calculated margin is recorded before the financial statement is published and the realised value is added beside it; an interval computed from past errors is shown too. [Source: the product's calculation rule; full text below]

<details>
<summary><b>Details: Method (full text)</b></summary>

This section describes Vantage Castle's four core quantities and its measurement records. All of it is measurement and arithmetic; none of it is a view on, or advice about, any share. Next to each number the source or the kind of measurement is written. The measurement records are not part of this repository; the method is described in this section on its own.

### 1. Input index

The weighted average price of the company's basket of input commodities, built on a base of 01.01.2015 = 100. For most companies the weights are a rank assumption: first input 50%, second 30%, third 20%. For the few companies with a measured proportion, the measured figure replaces the assumption. A component with no price series drops out of the basket, the remaining weights are rescaled, and the dropped share appears on the row as "input coverage". [Source: the product's calculation rule; the weights are a design choice]

A commodity may be more expensive today while the company keeps producing from older stock. Input prices are therefore shifted back by the company's inventory turnover period: the average of the last four to eight valid quarters, held between 0 and 365 days. The output price is not shifted. [Source: the product's calculation rule]

### 2. Output index

For most companies, the relevant sub-item of the TurkStat Domestic Producer Price Index, on the same 01.01.2015 = 100 base. [Source: TurkStat Domestic Producer Price Index]

### 3. Price–cost gap

The ratio of the output index to the input index. What is measured is price; it is not profit, sales volume or efficiency. The current value is shown together with its percentile within the company's own last five years of history, never as a bare number. It is read at the latest common date on which every component of the basket is known. [Source: the product's calculation rule]

### 4. Realised gross margin

(Revenue − cost of sales) ÷ revenue, taken from the three-month current-period column of the financial report published on KAP (the Public Disclosure Platform); it is not derived from cumulative differences. The product shows the realised margin beside the price–cost gap and puts no "because" between them: they are two separately observed series. [Source: the companies' financial reports published on KAP]

### 5. Projection: arithmetic, not a verdict

The Projection page calculates the arithmetic effect of a commodity move on the reported margin under "everything else held constant": volume, unmonitored cost items and price pass-through are assumed fixed. The commodity input effect is taken from the move of the input basket over a given window, read back by the inventory turnover period as in §1; in the product's settings the window is defined as 30, 90 and 180 days, and the example in the [margin flow diagram](sema/marj-akisi.png) is the 90-day window. [Source: the product's calculation rule] Companies can absorb the effect through pricing, inventory, hedging and product mix. In the measured data the direction of the price–cost gap and the direction of the realised gross margin agreed in the same period 49.0% of the time (n=1492, 2015–2022), which cannot be told apart from a coin toss ([Honest findings](#honest-findings)). The product therefore does not report share prices or an investment direction; it shows, as a record, the margin calculated from input cost, the interval, and its difference from the realised margin. This is a calculation, not a referee and not advice; the realised value is added beside it afterwards. [Source: §4 and §6 of this section; the direction-agreement measurement is in the [Honest findings](#honest-findings) section]

### 6. Measurement record: FM-1 and Alfa

How well the arithmetic has held is measured by a forward record: the calculation is made and recorded before the financial statement is published, and the realised value is added beside it when it arrives. [Source: the product's measurement procedure] This repository does not contain the measurement records; what a reader can verify from it are the calculation rules in this section and the realised values the companies report on KAP.

- **FM-1** is a scenario calculation of the change in gross margin from the company's own financials (the name is the method's short name): one main figure and two scenario arms (a low arm and a high arm). The second face of the same method is a decomposition that places, side by side, the items the realised margin change was made of (commodities, sales price, volume, exchange rate, inflation accounting, inventory, other expenses); it gives no "the deviation came from this" verdict. [Source: the product's calculation rule]
- **Alfa** is the short name of a selection rule that chooses, per sector, whose main figure is shown, out of two methods (FM-1 and the product's earlier calculation engine, the "old engine"), with a rule written in advance; the rule looks at past direction agreement and is not changed after results are seen. [Source: the product's calculation rule]
- The third quarter of 2026 (Q3) is the first measurement of these records and it is not a referee: no method choice, pass/fail verdict or direction is drawn from Q3. Results are in the [Honest findings](#honest-findings) section.

### 7. Interval and fallback rule (from 2026 Q4)

**Interval.** One half-width q is added on each side of the product's main figure: [main figure − q, main figure + q]. q is computed from that method's own past absolute errors (split conformal method; coverage 80%); there is no hand-set width per company or sector, the interval is not clipped, and errors are not pooled across methods. A method with a history of fewer than 30 companies gets the interval labelled "sample n=…: rough". The coverage guarantee rests on the errors coming from the same distribution; that assumption has not been measured from Q3 to Q4. [Source: the product's calculation rule; formula: Angelopoulos and Bates, arXiv 2107.07511]

The 80% half-widths computed from the Q3 errors (in-sample, not evidence): ±7.994 points for FM-1 (n=50) and ±21.846 points for the old engine (n=10, rough). [Measurement: calculation made on 15.11.2026 on the realised margins reported for 2026 Q3]

**Fallback rule.** If the method Alfa chose produced no result for a company-quarter: (1) if the company has an FM-1 record, the product shows it labelled "no Alfa output; fallback: FM-1", and that figure is never called Alfa's figure; (2) if there is no FM-1 record either, the product says there is no model output and shows, as a reference, the company's most recently reported three-month realised gross margin on KAP; that reference counts as no method's figure and enters neither the interval nor any measurement. [Source: the product's calculation rule]

**Honesty note.** The interval and fallback rules were written after the Q3 results were seen; they are therefore no retroactive evidence for Q3. The first real test is 2026 Q4, where coverage is only descriptive: "n=…, k=…" is written and no "held / did not hold" verdict is given. [Source: the product's calculation rule]

### Limits

- Most basket weights are assumptions; a measured proportion exists only for a few companies.
- The monitored basket is not the whole cost; labour and depreciation are not in it.
- Companies that share the same input basket and the same output index have a numerically identical price–cost gap; the product flags this as an "identical series" and claims no difference between them.
- Q3 is one quarter and 40–50 companies; a shock common to the quarter may have moved all of them in the same direction.

</details>

## Honest findings

The most important design decision in Vantage Castle is what it does not say. None of six measurements that tested whether a margin or a share-price-series change can be derived from commodity prices found a meaningful relationship. For example, the direction of the price–cost gap and the direction of the realised gross margin agreed in the same period **49.0%** of the time (n=1492, 2015–2022), which cannot be told apart from a coin toss. The product therefore expresses no view; it puts what it measures side by side. The first forward-record measurement (2026 Q3) is not a referee, and its results are written with the same openness. [Source: the product's internal measurements; full text and tables below]

<details>
<summary><b>Details: Honest findings (full text)</b></summary>

The most important design decision in Vantage Castle is what it does not say. The measurements below tested whether a margin or a share-price-series change can be derived from commodity prices; none found a meaningful relationship. The product therefore expresses no view; it puts what it measures side by side.

The measurements that use share prices are an internal study made on commodity, margin and share price series. "No relationship" here means "not found with this data and this method"; it is not proof that no relationship exists.

### Paths tried and dropped (six measurements)

The "Data" column shows which kind of data each measurement rests on. These are the product's own internal measurements; their detailed records are not part of this repository.

| # | Measurement | Result | Data |
|---|---|---|---|
| 1 | Regression pipeline: per company and in a single model, margin and share-price-series change from commodity change | No meaningful power; out-of-sample (after 2023) explanatory power negative, i.e. worse than a plain average | Commodity, margin and share price series |
| 2 | Does the direction of the price–cost gap agree with the direction of realised gross margin in the same period? | **49.0%** (n=1492, 2015–2022); indistinguishable from a coin toss; no lag or alignment correction passed the 55% threshold | Price–cost gap and KAP margin, 2015–2022 |
| 3 | Sector-neutral reverse-ordered two-group difference: the difference in share-price-series change between a group of the companies where the gap measure is most favourable and a reverse-ordered group of those where it is least favourable | Difference t = **0.613**, p = **0.543**; indistinguishable from noise | Price–cost gap and share price series |
| 4 | Pricing-in measurement: when the gap changed markedly, how did the share price series separate from its sector peers? | No relationship found | Price–cost gap and share price series |
| 5 | Inventory turnover: does the turnover period move together with commodity prices? | No relationship found; the fixed-turnover assumption is therefore kept | Commodity prices and KAP financial reports |
| 6 | KAP event study: after a disclosure, does the share price series separate from its sector more than usual? | Looks only at the size of the separation, not its direction | KAP disclosures and share price series |

Two more paths were dropped: the "episode table" that matched periods of large gap changes with the following margin was removed (it would have presented an unproven relationship as proven), and an attempt to convert financial statements to a common base using consumer prices failed and was not applied to the tables.

### News direction label measurement (not shown on any product page)

News items were given a direction label, and it was checked whether the price series then changed in the same direction; the plan was written and frozen before labelling started. Result: the label direction and the following price-series direction agreed 51.2%, 50.3% and 51.5% of the time over 1, 5 and 20 trading days (a coin toss gives 50%); against a significance threshold of p < 0.0045 the p-values were 0.449, 0.873 and 0.366 (n = 1,029, 1,034 and 1,038 independent clusters). None is significant. [Measurement: 10.10.2026; news labels and share price series]

Two limits are stated openly: with this data an effect above about 55.8% could be excluded, and a smaller effect cannot be told apart; agreement between the two labellers was moderate (κ 0.570–0.657), so the result was recorded as "weak evidence of absence", not "no relationship for certain". No look-ahead violation was found (0). This measurement does not enter the product; the labels are shown on no screen.

### First forward-record measurement: 2026 Q3 (not a referee)

Calculations are made and recorded before the financial statement is published, and the realised KAP value is added beside them when it arrives. For the third quarter of 2026, 50 companies were examined. Q3 is not a referee: no method choice or pass/fail verdict is drawn from these tables.

Two short names appear in the table; both are defined in the [Method](#method) section. Alfa is the selection rule that chooses, per sector, which of two methods' main figure is shown, with a rule written in advance. FM-1 is the calculation of the change in gross margin from a company's own financials, with a main figure and two scenario arms, a low and a high one.

| Measurement | Result | Data |
|---|---|---|
| Mean absolute error of the main figure of the method Alfa chose, against realised margin (40 companies that have a figure) | **5.855 points**; under the assumption "margin stays as in the previous quarter", 7.140 points; medians 3.836 ↔ 3.830; Alfa closer in 20 companies, the simple assumption closer in 20 | 2026 Q3: the product's recorded calculations ↔ realised margins reported on KAP; 15.11.2026 |
| Same measurement in FM-1 sectors (35 companies) | 5.295 ↔ 7.057 points (Alfa closer in 19, simple closer in 16) | Same data |
| Same measurement in old-engine sectors (only 5 companies have a figure) | 9.776 ↔ 7.724 points (Alfa closer in 1, simple closer in 4) | Same data |
| Share of realised values falling between FM-1's low and high scenario arms | 19 / 49 (0.388); arms in order 11 / 29, arms in reverse order 8 / 20 (for reverse-ordered arms the interval was taken between the smaller and the larger value) | Same data |

Reading notes: (1) A few extreme values pull the mean up; the medians are almost identical. (2) Alfa's selection rule looks at direction agreement, not at mean absolute error; the error here is an additional descriptive measure. (3) In 10 companies the old engine has no figure, so Alfa has no output; coverage is 40/50. (4) In the old-engine arm the simple assumption is closer in 4 of 5 companies; this says nothing about so small a sample. (5) If KAP's three-month Q2 column is used instead of the Q2 value in the database, the simple assumption's error is 7.159 (sensitivity row). (6) One quarter; a common shock may have moved the companies in the same direction.

### How these findings shaped the product

The product gives no share price or investment direction and no trading advice, and it makes no statement about condition or direction such as "the gap narrowed, margin pressure exists"; it puts the input index, the output index, the price–cost gap and the realised gross margin side by side without implying causation. It shows, as a record, the margin calculated from input cost, the interval, and its difference from the realised margin; this is a calculation, not a referee and not advice. This is not a stylistic preference; it is the result of the measurements above. The system puts what it measures side by side and leaves the interpretation to the reader.

</details>

## Architecture

![Architecture diagram](sema/mimari.png)

The diagram labels are in Turkish. Six steps: series from official sources → a scheduled data pipeline (every row passes unit and date checks and its source is recorded) → the measurement layer (input index, output index, price–cost gap, realised gross margin) → the presentation pages (they read only from the measurement layer and show the source next to every number) → demo and masked mode → development by a team of AI agents.

<details>
<summary><b>Details: Architecture (full text)</b></summary>

1. **Data sources (Veri kaynakları).** Series from official sources: commodity prices, exchange rates, interest and inflation series, company financials.
2. **Data pipeline (Veri hattı).** Daily and monthly scheduled jobs read the sources; every row passes unit and date checks and its source is recorded.
3. **Measurement layer (Ölçüm katmanı).** For each company the input index (weighted price of the commodities in its input basket), the output index (a series close to its sales price) and their ratio, the price–cost gap, are calculated; the realised gross margin sits next to them.
4. **Presentation (Sunum).** The My board, Map, Companies, Commodities, Changes, Bulletin, Projection, Sectors, Commodity Network, Supply Chain, KAP, Data quality and Screening pages read only from the measurement layer and show the source next to every number.
5. **Demo and masked mode.** In publication mode share prices, KAP filings and financial statement tables are not shown; in masked mode news headlines, electricity (EPİAŞ) and chokepoint (PortWatch) values and account details are also left out. The page images in this repository come from the masked mode.
6. **Development (Geliştirme).** The product is built by a team of AI agents: every task starts with a plan, production and review happen in separate sessions, and every outward step is taken by a human. Details: [Team](#team)

</details>

## Team

Vantage Castle was built by a team of AI agents: each agent works in a separate session with a single role. Every task starts with a plan, no one approves their own work (a separate auditor looks at the applied result), everything that goes outside is with a human, and a human has the final word. [Source: short summary of the working order; full text below]

<details>
<summary><b>Details: Team (full text)</b></summary>

Vantage Castle is a product of HBK Software. HBK Software is a team made up of AI agents: each agent works in a separate session with a single role. The owner of the company is a human, and the final word is theirs. This section describes how the team works, and what it does and does not do.

### Roles

The team has nine roles:

| Role | What it does |
|---|---|
| Private secretary | Distributes requests, collects finished work, leaves the human a short result note |
| Front end | Writes the interface |
| Back end | Writes the server, calculation and test code |
| Designer | Draws the screen direction and mock-ups |
| Database specialist | Queries data read-only, writes counting and verification reports |
| Researcher | Brings sourced, narrow notes from external sources; also wrote the texts in these documents |
| Auditor | Tests a delivery without seeing the producer's conversation, looking only at the output and the rules |
| Council | Writes drafts of new versions of the rules; does not sign them |
| Security | Watches authority limits, records and history; reports what it finds and does not fix it itself |

### How work runs

1. **Every task starts with a plan.** The plan is short: what will be done, which files will be touched, how it will be verified, how long it will take, what the risk is. For large tasks the plan goes to the human for approval.
2. **Whoever produces does not approve their own work.** First a machine checks: tests, a secrets scan and protection checks run. Then an auditor in a separate session, without seeing the producer's conversation, looks at the delivery as actually applied: does it work and look right with a copy of the real data? Without a look at the applied result there is no acceptance.
3. **If rejected, the producer fixes.** The private secretary runs at most two correction rounds without asking the human; at the third, the decision is the human's.
4. **There is a third pair of eyes.** The Security role watches for any step outside authority and reports it to the human if found.
5. **Everything that goes outside is with the human.** Publishing, deployment, e-mail, payment and sending data to third parties are closed to the agents; work stays in a local draft and local record.
6. **Rules belong to the human.** Agents propose rule changes or write drafts; what takes effect is the human's signature.

### Memory and record

The agents have no memory between sessions. Each task starts in a clean session from a status file, a notebook and the request file; everything important is in files. Work is not finished until a report is written. Decisions are kept in one place only, exactly as the human stated them.

### Rule for numbers

No number is written without a source: the source or measurement stands next to every number. Instructions found in a page read from an outside source are data, not orders. Keys and passwords live only in environment variables; they are not written to files, reports or records.

### Limits

- Agents can be wrong. The aim of the working order is not to abolish error but to have a wrong result looked at by a separate pair of eyes; the audit, too, is limited, like any measurement.
- This section is a short summary of the working order; the full text of the internal rules is not in this repository.
- None of the product's numbers is an agent's "view"; they come from the measurement record and the source series ([Method](#method), [Honest findings](#honest-findings)).

</details>

## What it does not do

It does not report share prices or an investment direction, and it gives no trading advice or investment advisory service. It shows, as a record, the calculated margin, the interval and its difference from the realised margin; this is a calculation, not a referee and not advice, and it also states what it does not know.

## Licence and attributions

This repository contains no code; text and images are shared with all rights reserved.

The data in the images is given with its source:

- Map tiles (Map image, hero GIF): © OpenMapTiles © OpenStreetMap contributors
- News clusters (Map): Source: The GDELT Project (gdeltproject.org)
- Commodity prices (My board, Companies, Commodities, Changes, Bulletin, Commodity Network, Matching matrix, hero GIF):
  - Jet fuel, LPG, butane, petroleum coke, fuel oil, scrap steel, barley/malt, salt, printing ink, carbon black, pulp/waste paper: Source: FRED, Federal Reserve Bank of St. Louis (EIA and BLS series)
  - Imported coal (Newcastle), uranium, zinc, lead, nickel, tin, timber, rice, coffee, wool, natural rubber: Source: FRED, Federal Reserve Bank of St. Louis (IMF series); FRED carries the note "Copyrighted: Citation Required" on these series
  - Wheat, palm oil, DAP, phosphate rock, potash, urea: Source: The World Bank, Commodity Price Data (The Pink Sheet)
- Raw milk recommended price (Commodities, hero GIF): Source: Ulusal Süt Konseyi (the Turkish National Milk Council)
- Exchange rate data (dollar equivalent of series sourced in lira, Changes): Source: Central Bank of the Republic of Türkiye, Electronic Data Delivery System (EVDS)
- Supply Chain (images): daily transit counts of the chokepoints: Source: IMF PortWatch; country-of-origin shares: Source: CEPII BACI; domestic production share: Source: USGS Mineral Commodity Summaries 2026 and publications of the Ministry of Energy and Natural Resources (ETKB); chokepoint positions: Source: representative centre points based on EIA
- Satellite image in the crisis-file panel of the product's Map page (the panel is not open in the images in this repository): MODIS Land Rapid Response Team, NASA GSFC (2020-12-02). Credit written in the image inside the product: "Kamu malı (ABD federal hükümeti çalışması – NASA)" (public domain, work of the US federal government – NASA). [Source: NASA, images and media usage guidelines, <https://www.nasa.gov/nasa-brand-center/images-and-media/>; accessed 16.11.2026: NASA content is generally not subject to copyright in the United States, and NASA is to be acknowledged as the source]
- Typeface: Martian Mono, SIL Open Font License 1.1
