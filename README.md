# Placement Pricing Model

An Excel pricing calculator I built to understand how staffing firms price client placements. It turns a candidate's pay rate into a client bill rate, then checks whether the deal still hits a gross margin target after markups, discounts, and rebates.

**Note:** All wage and client data in this workbook is illustrative. I built it to learn placement pricing mechanics, not from any company's real data.


## What's inside

| Tab | What it does |
|---|---|
| Rate Card | Pay rates for 12 roles at Entry, Mid, and Senior levels |
| Assumptions | Burden rate, 28% target gross margin, standard hours, and markup tiers |
| Quote Builder | Pick a client, role, level, and discount, and it prices the placement end to end |
| Client Rate Card | Applies a client's negotiated discount and volume rebate to every role and level, with a margin check on each |
| Placements | Sample placement log |
| Summary | Totals and a pivot table by practice |

## How the pricing works

1. Looks up the pay rate using a two-way INDEX/MATCH (role picks the row, level picks the column)
2. Finds the markup tier with a VLOOKUP approximate match
3. Builds the bill rate, then applies the client discount
4. Adds burden to get total cost, then calculates gross profit and margin
5. Flags whether the quote meets the 28% target and shows the lowest rate and biggest discount allowed

## Skills used

Excel: INDEX/MATCH, VLOOKUP (approximate match), SUMIFS, pivot tables, data validation, scenario modeling
