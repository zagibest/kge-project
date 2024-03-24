### Project Purpose

Our project objective is to merge Ulaanbaatar's _street network data_ into a cohesive knowledge graph. This graph will enable users to easily navigate from one location to another within Ulaanbaatar, offering clear and dependable routes.

### Scenarios definition:

- **Scenario 1:** UB's Cultural and Historical Landmarks
- **Scenario 2:** Urban Expansion and Non-Mapped Areas
- Scenario 3: Enhancing tourists experience
- Scenario 4: Accessible navigation for people with disabilities
- Scenario 5: UB’s common places like schools, hospitals etc

### Personas:

- **Persona 1:** Freshman Bataa is going to the National University of Mongolia for the first time from his home located in Sansar and he quite doesn’t know the path to get there.
- **Persona 2:** Dondog, 68 years old senior who suffers from Alzheimer's disease can’t memorize his path from his home to the hospital.
- Persona 3: Bocca, visiting professor residing near the city center, is passionate about culinary exploration.
- Persona 4: Sarnai has wheelchair teacher who lives in UB., relies on public transportation and walking to navigate the city.

### Competency Questions (CQs):

- SQ 1: Recommend Bataa possible paths to National University of Mongolia from his home in Sansar.
- SQ 2: Give Dondog route information from his current location to either his home or the hospital.
- SQ 3: Recommend Bocca, restaurants near his home.
- SQ 4: Provide Sarnai with routes and places that are accessible by a wheelchair.

### Concepts identification:

| Scenarios
| Personas | CQ’s | Entities | Properties | Focus classification | Popularity classification |
| --- | --- | --- | --- | --- | --- | --- |
| 5 | 1 | 1 | Bataa, home, university | id: int, name: string, coordinates: [lat: int, long: int] | Contextual | Contextual |
| 5 | 2 | 2 | Dondog,home,hospital | id: int, name: string, coordinates: [lat: int, long: int] | Contextual | Contextual |
| 3 | 3 | 3 | Restaurants near city center | id: int, name: string, coordinates: [lat: int, long: int] | Core | Common |
| 4 | 4 | 4 | Accessible routes | id: int, name: string, coordinates: [lat: int, long: int] , accesibility_info: string | Core | Common |

### ER model definition:

### Report on First Phase Methodology Work:

In the initial phase of our project, we made several important decisions regarding the integration of Ulaanbaatar's street network data into a unified knowledge graph. Each decision was thoroughly considered, weighing its advantages and limitations. Here's a clear overview of the rationale behind our choices:

1. **Choice: Data Selection**
   - _Reasoning:_ We chose to prioritize Ulaanbaatar's street network data due to its pivotal role in facilitating city navigation.
   - _Strengths:_ Utilizing street network data allows us to provide accurate and efficient route recommendations, aligning with our project goal of seamless navigation.
   - _Weaknesses:_ Potential challenges may arise from data availability and accuracy, requiring careful validation and quality assurance.
2. **Choice: Scenario Definition**
   - _Reasoning:_ We outlined five specific scenarios to guide our project's scope, covering a wide range of user needs and situations.
   - _Strengths:_ Scenario definition ensures that we address diverse navigation challenges comprehensively.
   - _Weaknesses:_ Broader scenarios could introduce complexity, necessitating prioritization to effectively manage resources.
3. **Choice: Persona Selection**
   - _Reasoning:_ We developed four personas representing different user groups and navigation scenarios to inform our development process.
   - _Strengths:_ Personas offer valuable insights into user needs, guiding the creation of user-friendly features.
   - _Weaknesses:_ While personas provide useful guidance, they may not capture every user preference, requiring ongoing feedback collection and adjustment.

### Conclusion

Our decisions in the first phase reflect a strategic approach to integrating Ulaanbaatar's street network data into a navigation-focused knowledge graph. By carefully considering the pros and cons of each choice, we aim to develop a reliable solution that caters to the varied needs of Ulaanbaatar's residents and visitors.
