# Bechdel-Test Analysis of Oscar-Nominated Films
![Bechdel Test](https://upload.wikimedia.org/wikipedia/en/b/bf/Dykes_to_Watch_Out_For_%28Bechdel_test_origin%29.jpg)

## Abstract
The Bechdel Test is a sequence of three questions designed to assess the presence of women in movies. It highlights the underrepresentation and overall gender asymmetry in fiction, using easily detectable metrics to evaluate gender bias. This study investigates the application of the Bechdel test to a selection of 20 Oscar-nominated films, aiming to automate the evaluation of gender representation within their scripts.

The film industry stands as a powerful cultural force, shaping perceptions and influencing social interactions across the globe. It serves not only as a source of entertainment but also as a mirror reflecting the complexities of the human experience. In recent years, the call for greater representation has intensified, collecting different opinions and representation-based metrics of evaluation. The Bechdel Test, devised by Alison Bechdel, provides a set of criteria for gender portrayal in films, assessing if they feature at least two named female characters who engage in a conversation about something other than a male character.

The objective of this study was to automate the analysis of 20 films spanning multiple genres to ascertain the prevalence and characteristics of those conforming to Bechdel Test criteria. The list of movies analyzed can be found in Appendix 1. Films were selected among those nominated for an Oscar, as this was considered an appropriate metric to indicate that a film was well-received by both the public and critics. Additionally, it is noted that none of the selected films have female directors.

## Goal
This project aims to shed light on gender representation in film through an automated approach to the Bechdel Test. The findings will contribute to the ongoing discourse on gender equity in the film industry, providing insights that can inform future productions and assessments of representation in cinema.

## Methodology
Utilizing a systematic data management approach, various sources were leveraged to create a dataset encompassing different facets of each film, including cast, dialogue, and thematic content. Methodologically, the research involved the creation, categorization, and analysis of this dataset, employing both qualitative and quantitative methodologies to derive meaningful insights.

## Data Collection

### Research Questions
The research question that shaped this analysis adheres to the criteria outlined by the Bechdel test, which served as a guiding framework. The whole concept of this test is enclosed in the following text of a Bechdel’s comic:
> “I only go to a movie if it satisfies three basic requirements. One: it has to have at least two women in it, who, two, talk to each other about, three, something besides a man.”

The analysis was therefore conducted in order to select the films that positively met the following criteria:
1. Does it contain two women?
2. Do the (at least) two women interact with each other in at least one scene?
3. Is the interaction about something other than a man?

### Data Sources and Data Extraction
The data collected for this project encompasses various components sourced from multiple online platforms. The components were categorized into script data, gender, actors, and additional pertinent details:

- **Scripts**: Crucial data for the analysis of dialogue and scene content. The scripts were retrieved from the Internet Movie Script Database (IMSD) using a custom extraction function developed to obtain the script text for each title, which was then parsed and divided into different scenes. The Beautiful Soup library was used for web scraping.
  
- **Cast**: Information about the cast helped identify the actors and their respective roles and was sourced from the Internet Movie Database (IMDB). Utilizing web scraping techniques, the full credits page of each film was accessed to extract the cast list, including data inherent to the names and the corresponding roles.

- **Gender**: The determination of the gender of actors was performed utilizing the Names Dataset Library and NLP techniques.

