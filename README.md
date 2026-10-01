# Biochar Phosphorus Explorer

**[Open the Explorer](https://american-biochar-institute.github.io/phosphorus-explorer/)**

Biochar carries phosphorus inherited from the biomass it was made from, and how much depends
almost entirely on the feedstock. Wood biochar and manure biochar differ by roughly thirtyfold,
so a single number for "biochar" misleads.

This is every phosphorus value the American Biochar Institute has extracted from its reference
library, with the feedstock it came from, the reagent that measured it, and the study it is
printed in, plus 45 commercial products measured for the USDA-ARS Biochar Atlas. Filtering the
set recomputes the statistics, and each figure states what its data will and will not support.

## Who it is for

Anyone who needs the underlying numbers rather than a summary:

- **Producers and agronomists** weighing an application and needing to know what a given
  material will actually deliver per acre
- **Biochar manufacturers** placing their product against the published range for its feedstock
- **Researchers** looking for the measurement behind a figure, including the exact extractant
- **Policy and nutrient-planning staff** who need a defensible distribution rather than an average

It was assembled to support ABI's comments on the proposed revision of USDA-NRCS Conservation
Practice Standard 336, Soil Carbon Amendment (Docket NRCS-2026-0100), and is published here so
the evidence stands on its own.

## What is in it

`index.html` is self-contained: one file, no build step, and it opens offline in any browser.

| View | What it shows |
|---|---|
| Total phosphorus by feedstock | One mark per observation, log scale, nine feedstock classes |
| What each reagent recovers | Extractable phosphorus by reagent, and what each reagent is for |
| How much of a biochar's phosphorus any reagent recovers | Extractable as a percent of the same biochar's total |
| How much phosphorus an application actually delivers | Live application-rate slider against 25 lb P₂O₅/acre |
| What a source-coefficient relationship returns | The Elliott et al. 2006 relationship applied to biochar, with its limits |

A Source filter shows the published literature, the USDA-ARS products, or both (the default).

## The evidence base

- 2,191 extracted rows from 197 items in the ABI BIOCHAR reference library
- 486 headline total-phosphorus observations from 89 papers
- 621 headline extractable observations
- A value quoted from another paper is counted once, and the orthophosphate and pyrophosphate parts of
  one water extract are not counted beside their total
- 45 USDA-ARS Biochar Atlas commercial products, Ashworth laboratory totals (microwave nitric acid
  and hydrogen peroxide digest, run without a certified reference material)
- Every literature row carries the feedstock as the paper names it, the production temperature,
  the exact digestion or extractant, the value and unit as printed, and a page or table reference

Counts are a floor, not a census. The library holds more items than have been read, and the
selection favored papers about phosphorus over papers that merely report it in a methods table.

## Conversion used throughout

```
lb P2O5/acre = total P (mg/kg dry) x dry short tons/acre x 0.004582
```

where `0.004582 = 2000 x 2.29137 / 1e6` and `2.29137 = 141.944 / (2 x 30.973762)`.

## What this does not establish

The dataset holds no water-extractable phosphorus value measured to the Kleinman et al. 2007
protocol that Maryland and Pennsylvania name. **ABI has found no accepted phosphorus source
coefficient for biochar**, none is offered here, and the nominal values in the last view illustrate direction and
magnitude only. The Elliott et al. 2006 relationship they use was calibrated with a 200:1 water
extraction, which differs from the 100:1, one-hour Kleinman et al. 2007 method; no biochar row in the
dataset follows either protocol in full. Neither these distributions nor any loading figure establishes runoff safety for
a particular field. The 25 lb P₂O₅/acre line is an ABI proposal for unfortified biochar, counted
cumulatively over any rolling three-year period, not an adopted NRCS threshold.

## Related explorers

- [Biochar Nitrogen Explorer](https://github.com/American-Biochar-Institute/nitrogen-explorer)
- [Biochar Potassium Explorer](https://github.com/American-Biochar-Institute/potassium-explorer)

## Reuse and corrections

Figures may be reproduced with attribution. Please cite the page and the date it was built,
since the dataset is revised as more of the library is read.

> American Biochar Institute. Biochar Phosphorus Explorer. Built September 30, 2026.
> https://github.com/American-Biochar-Institute/phosphorus-explorer

Corrections and additions are welcome: open an issue, or write to info@biochar.org.

## About

The American Biochar Institute is a 501(c)(3) nonprofit developing standards and markets for
biochar across agricultural, industrial, and built-environment sectors.
[biochar.org](https://biochar.org)
