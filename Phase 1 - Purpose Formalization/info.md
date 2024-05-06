# Purpose Formalization

## Project Purpose

Our project objective is to merge Ulaanbaatar's _street network data_
into a cohesive knowledge graph. This graph will enable users to easily
navigate from one location to another within Ulaanbaatar, offering clear
and dependable routes.

## Scenarios definition:

- **Scenario 1:** UB has a dense architectural layout, thus it's
  walk-able to most places like schools, and hospitals.

- **Scenario 2:** Residents of Ulaanbaatar enjoy escaping the city's
  air pollution by hiking to various nearby trails and scenic spots.

- **Scenario 3:** Because of the country's prime location bridging
  Central and East Asia, Ulaanbaatar hosts a variety of Asian
  restaurants and pubs like Korean, Japanese, Uzbek and so on.

## Personas:

- **Persona 1:** Freshman Bataa is going to the National University of
  Mongolia for the first time from his home located in Sansar and he
  quite doesn't know the path to get there.

- **Persona 2:** Dondog, a 40-year-old hiker, enjoys discovering
  various hiking spots in the vicinity of Ulaanbaatar.

- **Persona 3:** Bocca, visiting professor residing near the city
  center, is passionate about culinary exploration.

## Competency Questions (CQs):

- **SQ 1:** Recommend Bataa possible paths to National University of
  Mongolia from his home in Sansar.

- **SQ 2:** Give Dondog route information from his current location to
  nearby hiking spots.

- **SQ 3:** Recommend Bocca, restaurants and pubs near his home.

## Concepts identification:

::: {#tab:adjusted}
Scenarios Personas CQ's Entities Properties Focus classification Popularity classification

---

1 1 1 Bataa's home, NUM id: int, paths: int\[\], `start_destination`: int, `end_destination`: int, length: double Contextual Contextual
2 2 2 Dondog's home, hospital id: int, paths: int\[\], `start_destination`: int, `end_destination`: int, length: double Contextual Contextual
3 3 3 Restaurants id: int, paths: int\[\], `start_destination`: int, `end_destination`: int, length: double Core Common

: Concepts identification Table
:::

## ER model definition:

![ER Model](images/new_er.png){#fig:example width="100%"}
