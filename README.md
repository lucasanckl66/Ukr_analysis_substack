Data and code used to create graphics and see if datasets are a fit for my substack, which can be found through this link: https://substack.com/@lucasan1?utm_source=user-menu

Lots of data pertaining to the war in Ukraine is incomplete, as the war is still going on. Many of the graphics and datasets used here will not be published on my substack. 

## Examples of Graphs Created

### Ukrainian Deaths by Month
![Ukrainian Deaths by Month](substack/figures/04_ukrainian_deaths_by_month.png)

### Age at Death by Year and Personnel
![Age at Death by Year and Personnel](substack/figures/Age_at_Death_by_Year_and_Personnel_Category.png)

### Three Month Rolling Median Age at Death for PMCS and Conscripts
![Three Month Rolling Median Age PMC Conscript](substack/figures/Three_Month_Rolling_Median_Age_PMC_Conscript.png)

## Data Sources
- **Poteru:** Documented Russian military deaths, including age, rank, location, branch, PMC status, and conscript status.
- **VIINA:** Geolocated event and media-reporting from the war in Ukraine.
- **Confirmed Ukrainian Military Personnel Losses — Olivier Hubert:** Daily losses of the Ukrainian military according to the UALosses
- **Confirmed Russian Military Officers Losses — Olivier Hubert:** Daily losses of the Russian military according to the Killed in Ukraine Project
- **2022 Russia Ukraine War, Losses, Oryx + Images -Petro Ivanuik:** Equipment losses for both sides based on Oryx by scraping Ukrainian losses and Russian losses pages

## Limitations

### Poteru

- Includes publicly documented deaths rather than all Russian military deaths. Reporting delays make recent months particularly incomplete.
- Age, rank, branch, PMC status, and conscript status depend on available information. Missing labels should not automatically be interpreted as a negative classification.
- Differences between groups may reflect uneven reporting. Death counts alone cannot establish mortality risk without knowing how many personnel served in each group.

### VIINA

- Tracks news reports rather than every battlefield event. Coverage reflects media access, editorial priorities, and reporting restrictions.
- Automated event classifications can contain errors, and accuracy varies across categories.
- The one-per-day filter can merge separate incidents of the same type in the same location. Report dates may also differ from the dates incidents occurred.

### Confirmed Ukrainian Military Personnel Losses — Olivier Hubert / UALosses

- Relies on publicly available death announcements and other open sources, leaving unreported deaths outside the count.
- Reporting delays and missing demographic information can distort monthly totals and age distributions.
- Geographic coverage is uneven. Direct comparisons with Russian death databases require matching time periods, definitions, and inclusion criteria.

### Confirmed Russian Military Officers Losses — Olivier Hubert / Killed in Ukraine

- Covers documented officer deaths rather than all Russian military personnel, so its patterns cannot automatically be generalized to the wider force.
- Publication dates can differ substantially from estimated death dates, making recent periods incomplete.
- Rank-specific totals do not establish relative mortality risk without information on the number of officers serving at each rank.

### Equipment Losses — Petro Ivanuik / Oryx

- Includes visually documented equipment losses rather than all losses. Differences in available footage can affect comparisons between sides.
- Destroyed, damaged, abandoned, and captured equipment are different outcomes and should not all be interpreted as permanent destruction.
- Scraped copies may lag behind Oryx updates or retain extraction errors. The date evidence appears does not necessarily establish the date of the loss.

### Mediazona Russian Military Deaths

- The named list is a minimum documented count, separate from Mediazona's statistical estimates of total deaths.
- Delayed announcements and uneven public reporting affect comparisons across months, regions, and recruitment categories.
- Records may overlap with Poteru and other named-death databases. Counts should not be added together without identifying duplicate individuals.

### The Economist’s Casualty Estimates

- Provides model-based estimates rather than a verified count. Results depend on the accuracy of the underlying casualty estimates and model assumptions.
- Daily changes should not be treated as precisely measured daily losses. Uncertainty intervals should accompany the estimates.
- The model currently estimates Russian losses. Its total casualty estimates include killed and wounded and should not be compared directly with death-only counts.

### The Economist’s War-Fire Model

- Detects heat signatures associated with likely war activity, rather than every battle or strike. Weather, satellite timing, and insufficient heat can prevent detection.
- Classification can mistake civilian fires for war activity or miss actual war-related fires. Extreme heat also limits classification.
- Fire detections are an indirect indicator of fighting intensity, not a direct measure of casualties, successful strikes, or territorial gains.

### UCDP Georeferenced Event Dataset

- Covers lethal organized violence meeting UCDP's inclusion rules, rather than every military incident. Its event totals are therefore not directly equivalent to VIINA's.
- Dates and coordinates vary in precision; some represent broader periods or areas rather than exact days and locations.
- Fatality figures are estimates. Low, best, and high estimates should be considered, and recent coverage depends on the dataset version used.

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