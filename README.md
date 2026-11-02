Data and code used to create graphics and see if datasets are a fit for my substack, which can be found through this link: https://substack.com/@lucasan1?utm_source=user-menu

Lots of data pertaining to the war in Ukraine is incomplete, as the war is still going on. Many of the graphics and datasets used here will not be published on my substack. 

Some examples of graphs I have created

### Ukrainian Deaths by Month
![Ukrainian Deaths by Month](substack/figures/04_ukrainian_deaths_by_month.png)

### Age at Death by Year and Personnel
![Age at Death by Year and Personnel](substack/figures/Age_at_Death_by_Year_and_Personnel_Category.png)

### Three Month Rolling Median Age at Death for PMCS and Conscripts
![Three Month Rolling Median Age PMC Conscript](substack/figures/Three_Month_Rolling_Median_Age_PMC_Conscript.png)

## Data Sources
- **Poteru:** Documented Russian military deaths, including age, rank, location, branch, PMC status, and conscript status.
- **VIINA:** Geolocated event and media-reporting from the war in Ukraine.

## Limitations
- Documented deaths are not equivalent to total deaths.
- Records from recent months may be incomplete.
- PMC, conscript, rank and branch labels depend on available public information.
- Geographic totals may reflect population size and uneven reporting.
- VIINA measures reported events and language, not every battlefield event.

## Repository Structure (10/23/26)
```text
myproject1/
├── casualty_analysis/
│   ├── data/
│   └── casualty_analysis.ipynb
│
├── substack/
│   ├── data/
│   ├── figures/
│   ├── dedovshchina.ipynb
│   ├── poteru.ipynb
│   ├── total_loss.ipynb
│   └── future.ipynb
│
├── .gitattributes
└── README.md
```
## Future Changes and Planned Progression

### For the currently empty casualty_analysis.ipynb:

- **[Mediazona Russian Military Deaths](https://en.zona.media/article/2026/09/21/casualties_eng-trl):** A verified named list of Russian military deaths compiled from public sources. I plan to examine differences across ages, regions, and recruitment categories, and compare these patterns with my existing casualty datasets.

- **[The Economist’s Casualty Estimates](https://github.com/TheEconomist/the-economist-ukraine-war-dead-and-wounded-estimates):** Combines reported casualty estimates, war-fire activity, and territorial changes to estimate Russian military deaths and total casualties. I plan to visualize these estimates over time, examine their uncertainty, and compare estimated deaths with confirmed named deaths.

### Other interesting datasets for the near future:

- **[The Economist’s War-Fire Model](https://github.com/TheEconomist/the-economist-war-fire-model):** Uses satellite temperature anomalies and machine learning to identify likely war-related fires in Ukraine. I plan to map changes in fighting intensity and compare them with reported conflict events in VIINA.

- **[UCDP Georeferenced Event Dataset](https://ucdp.uu.se/downloads/):** Records events of organized violence with dates, locations, actors, and fatality estimates. I plan to isolate events in Ukraine, map geographic and temporal patterns, and compare coverage with VIINA.


## Related Writing
https://lucasan1.substack.com/p/fear-moves-down-lies-move-up-what 