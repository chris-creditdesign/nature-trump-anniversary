# nature-trump-anniversary

Data investigation for Nature Trump anniversary 2026 feature article.

## NIH Keywords

From NIH Reporter, for years 2021, 2022, 2023, 2024 and 2025 select Funding Mechanism as "Research Project Grants” and Award Type as “New”.

For each year download a csv file containing "Project terms” and “Total Cost” for each grant.

Remove rows where Project Terms or Total Cost are empty.

2021
- Rows removed: 532
- 11,279 grants
- 28,914 unique keywords
- Total funding: $6,121,521,522

2022
- Rows removed: 519
- 11,921 grants
- 29,244 unique keywords
- Total funding: $7,449,682,187

2023
- Rows removed: 521
- 11,647 grants
- 29,677 unique keywords
- Total funding: $6,506,773,772

2024
- Rows removed: 409
- 10,603 grants
- 29,390 unique keywords
- Total funding: $6,166,728,801

2025
- Rows removed: 322
- 8,493 grants
- 28,094 unique keywords
- Total funding: $5,819,319,619

Total unique keywords across all years: 41,742

For each keyword per year, calculate:
- Number of grants containing the keyword
- Percentage of grants containing the keyword
- Total funding for grants containing the keyword
- Proportion of funding attributed to grants containing the keyword

For years 2021, 2022, 2023, 204 calculate the average percentage of grants containing the keyword and average proportion of funding attributed to grants containing the keyword.

i.e.
2021 = 5%
2022 = 10%
2023 = 15%
2024 = 20%

Average = (5 + 10 + 15 + 20) / 4 = 12.5%

Remove any results where the percentage of grants or the proportion of funding is less that 0.1%.

## NSF

Download JSON files for 2021, 2022, 2023, 2024 and 2025 from: https://www.nsf.gov/awardsearch/download-awards