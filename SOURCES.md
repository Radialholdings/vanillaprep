# Library sources and licenses

The library is plain-text copies of the sources below, converted with `library/build_library.py`. Every source
here is either in the public domain or under a Creative Commons Attribution-ShareAlike license (CC BY-SA), so the
library may be sold. Each source keeps its own license, which the app shows with every article: each article keeps
its source address, and Stack Exchange posts keep their authors' names. CC BY-SA text stays under CC BY-SA
(attribution and ShareAlike). This file travels inside the library. Licenses and terms were checked on 2026-10-24 (the trades, fitness, food and classic sources on 2026-10-30).

Non-commercial material (wikiHow, iFixit, the IFRC and WHO guides) and the Emergency Response Guidebook
("not for resale") are **not** included; see "Left out", below.

## Sources

| Source | What it covers | License | Where it comes from |
|---|---|---|---|
| Wikipedia, about 930,000 of the most-read articles | General knowledge | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/), Wikipedia contributors | Kiwix `wikipedia_en_top1m` |
| WikiMed | Medical encyclopedia (Wikipedia medicine) | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/), Wikipedia contributors | Kiwix `wikipedia_en_medicine` |
| WikEM | Emergency medicine | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/), WikEM contributors | Kiwix `wikem_en_all` |
| MedlinePlus (NLM-written pages only) | Health topics, lab tests, genetics | Public domain (U.S. National Library of Medicine) | Kiwix `medlineplus.gov_en_all`; licensed sections removed (see below) |
| FDA drug labels (openFDA) | Drug Facts for over-the-counter medicines; Medication Guides and patient information for prescription medicines. Manufacturer labels, not verified by the FDA, and they may be out of date | [CC0 1.0](https://open.fda.gov/license/) (public domain). Not endorsed by the FDA | openFDA bulk download; `library/fetch_fda_labels.py` |
| CDC Travelers' Health | Disease, water and food safety | Public domain (CDC). Includes the online CDC Yellow Book; its printed edition is published by Oxford University Press. | Kiwix `wwwnc.cdc.gov_en_all` |
| Ready.gov (FEMA) | Emergency preparedness by hazard | Public domain (FEMA) | Kiwix `ready.gov_en_all` |
| Military medicine manuals | Hospital Corpsman, First Aid (FM 4-25.11), Ship's Medicine Chest, field sanitation, preventive medicine, radiation protection | Public domain (U.S. government). Three volumes that reprint copyrighted material (Military Dermatology, War Psychiatry, FM 21-11) are left out. | Kiwix `irp.fas.org_en_military-medicine` |
| U.S. government survival and first-aid manuals | USAF AFH 10-644 SERE Operations, Army ATP 3-50.21 Survival, ATP 4-02.11 First Aid (2026), TC 21-3 Cold Weather, ATP 4-25.12 Field Sanitation, TB MED 577 Field Water, TB MED 507 Heat, FEMA Are You Ready?, FEMA CERT manual, Joint Trauma System Prolonged Casualty Care | Public domain (17 U.S.C. 105) | `library/fetch_manuals.py` |
| Nuclear War Survival Skills (Cresson Kearny, ORNL, 1979; 1987 edition) | Fallout shelter, water, ventilation | Oak Ridge National Laboratory report; the 1986 additions are copyright Cresson H. Kearny, reproduced with his notice, which is kept in the text | `library/fetch_manuals.py` |
| Risk and micromort references | Estimating risks of death: the Social Security life table (2023) restated in micromorts per year and per day, CDC's "Mortality in the United States, 2024" and "Deaths: Leading Causes for 2024", NHTSA's 2024 crash overview (deaths per mile driven), the National Weather Service's lightning odds; plus Wikipedia's articles on micromorts, Fermi estimates, life tables, relative risk and related topics | Government statistics: public domain (SSA, CDC, NHTSA, NWS). Wikipedia articles: [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) | `library/fetch_risk.py` (CDC and SSA files from the Internet Archive; their sites refuse scripted downloads) |
| USDA Complete Guide to Home Canning (2015) | Safe canning, botulism prevention | Public domain (USDA) | Kiwix `usda-2015_en` |
| Appropedia | Appropriate technology, sustainability | [CC BY-SA](https://creativecommons.org/licenses/by-sa/4.0/) 3.0 or 4.0 (per page) | Kiwix `appropedia_en_all` |
| Energypedia | Solar, batteries, cookstoves, biogas | [CC BY-SA](https://creativecommons.org/licenses/by-sa/4.0/) 3.0 or 4.0 (per page) | Kiwix `energypedia_en_all` |
| WikiCiv | Rebuilding technology from scratch | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) | Kiwix `wikiciv_en_all` |
| Stack Exchange: Home Improvement, The Great Outdoors, Seasoned Advice (cooking), Gardening, Lifehacks, Sustainable Living, Amateur Radio, Medical Sciences, Motor Vehicle Repair, Pets | Practical Q&A, with each post's author | CC BY-SA 2.5, 3.0 or 4.0 by post date ([Stack Exchange licensing](https://stackoverflow.com/help/licensing)) | Kiwix Stack Exchange ZIMs |
| U.S. Navy and Army trades manuals | Seabee Construction Electrician, Utilitiesman (plumbing, water), Builder, Construction Mechanic, Machinery Repairman; NEETS electricity modules 1–5; Army Carpentry (TM 3-34.47) and Concrete and Masonry (TM 3-34.44); OSHA tool, electrical, generator, ladder and chainsaw safety | Public domain (U.S. government work); Navy manuals carry Distribution Statement A, "approved for public release; distribution is unlimited". Several are 1990s editions: check current electrical and building codes. No agency endorsement or logos | `library/fetch_skills.py` |
| Lessons in Electric Circuits (Tony R. Kuphaldt) | DC, AC, semiconductors, digital, reference, experiments | [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/), Tony R. Kuphaldt (current ibiblio editions; older copies under the Design Science License are not used) | `library/fetch_skills.py` |
| Army and HHS fitness, sleep and mental readiness guides | FM 7-22 Holistic Health and Fitness (with Change 2), ATP 7-22.02 drills and exercises, NIA's exercise guide for older adults, the Physical Activity Guidelines for Americans, NHLBI's guide to healthy sleep | Public domain (U.S. government work). Text only: the NIA guide's photos may be licensed stock | `library/fetch_skills.py` |
| Exercise library (free-exercise-db) | About 870 exercises: level, equipment, muscles, steps | [The Unlicense](https://unlicense.org/) (public domain). Text only; the dataset's images are not included | `library/fetch_skills.py` |
| Armed Forces Recipe Service | Department of Defense recipe cards for 100 portions, with nutrition analysis | Public domain (U.S. government work) | `library/fetch_skills.py` |
| Nutrition facts (USDA FoodData Central, SR Legacy) | Energy, protein, fat, carbohydrate, vitamins and minerals per 100 g for about 7,800 foods, with common household amounts | [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/). U.S. Department of Agriculture, Agricultural Research Service. FoodData Central, 2019. fdc.nal.usda.gov | `library/fetch_skills.py` |
| Classic manuals before 1929 | Dan Beard (shelters, camp-lore), Horace Kephart (camping and woodcraft, camp cookery), forging and smithing, woodworking for beginners, camp and household cooking, farm mechanics, Cobbett's Cottage Economy | Public domain in the U.S. (published before 1929). Texts from Project Gutenberg volunteers and Internet Archive scans; Project Gutenberg's license and trademark are removed, as its terms require for commercial reuse | `library/fetch_skills.py` |

## Left out

Non-commercial or not-for-resale, so left out of this (sellable) library:

- **UK Medicines A to Z (NHS)** — its terms ask for copies to be refreshed every 7 days and no charge for access.
- **wikiHow** and **iFixit** — CC BY-NC-SA 3.0 (non-commercial).
- **IFRC** International First Aid Guidelines, and the **WHO** guides (WHO-ICRC Basic Emergency Care; Managing
  Complications in Pregnancy and Childbirth; Guidelines for Drinking-water Quality) — non-commercial.
- **Emergency Response Guidebook 2024** — reproduction is permitted by the participating governments, but not for resale.

Free to read but not to sell, so left out (from the October 2026 content review):

- **BCcampus / SkilledTradesBC trades textbooks** and many LibreTexts / Open Textbook Library trades titles — CC BY-NC-SA.
- **NCTSN Psychological First Aid** (copyright NCTSN) and **WHO Psychological First Aid** — commercial use needs written permission.
- **Navy NOFFS** — developed with a contractor (EXOS); reuse terms unclear.
- **Darebee** workouts (no use in apps), **Good and Cheap** (CC BY-NC-SA), **The Conversation** articles (CC BY-ND).
- **USDA MyPlate Kitchen** — no bulk export, and recipes from outside partners belong to those partners.
- **Canning books from 1917–1920** on Project Gutenberg — public domain, but they teach cold-pack and water-bath methods for
  low-acid foods that USDA now calls unsafe; the library has USDA's current canning guide instead.

The license log, `library/LICENSE_LOG.csv`, lists every downloaded item with its address, license, the date it was checked
and its attribution (`python3 library/fetch_skills.py --log library/LICENSE_LOG.csv` writes it again).

Left out for mixed or reserved rights (as in the original project):

- MedlinePlus sections licensed to NLM by third parties: the A.D.A.M. Medical Encyclopedia (`/ency/`),
  ASHP drug information (`/druginfo/meds/`) and Natural Medicines (`/druginfo/natural/`).
- Kiwix "zimgit" collections (post-disaster, water, food, medicine, knots): they bundle PDFs from many
  publishers with mixed rights.
- Military Dermatology and War Psychiatry (Textbook of Military Medicine) and FM 21-11 (1988): they reprint
  copyrighted figures and text. FM 4-25.11, which replaced FM 21-11, is included.
- Hesperian books (*Where There Is No Doctor* and others): digital use needs written permission.
- MSF clinical guidelines, the Sphere Handbook, the USAMRIID Blue Book, Red Cross manuals and commercial
  survival books: all rights reserved.
