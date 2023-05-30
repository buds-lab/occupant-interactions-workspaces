# occupant-interactions-workspaces
Pilot data on identifying and contextualising occupant interactions within hybrid workspaces using the Cozie app on Apple smartwatches

This study involved 4 levels of surveying: an onboarding survey, a microsurvey taken hourly from 9 AM to 7 PM on the Cozie app, an end-of-day survey taken daily, and an exit interview. The data from the first three surveys and associated visualizations are contained within this GitHub.


## Microsurvey Question Flow
The question flow used in the Cozie app is given in the image below:

![Cozie Question Flow PNG](https://github.com/buds-lab/occupant-interactions-workspaces/assets/68923702/7578316b-1144-4d9b-bc07-23414954f2b9)

The questions within the dotted line cover the subjective components of the interaction while the remaining questions cover the objective context of the interaction.

## Data
The folder `data` contains all the data from the field experiment.

The field experiment involved:
* 9 participants working in the same office building in Singapore
* 5 Male and 4 Female
* Ages ranging from 25 to 41

`Thesh_Onboarding.csv` - this file contains the onboarding survey responses. This includes demographic information, perceptions of office work and scheduling, and personality tests.

`Microsurvey_Dataframe.csv` - this file contains the total raw data collected from the Cozie app. This includes the microsurvey response and the associated metadata/environmental variables (timestamp, location, heartrate, etc.). This data file was used for "Categorization Breakdown."

`sankey_plot.csv` - this file contains a subset of the microsurvey response data for plotting "Subjective Question Sankey." For every microsurvey response where a spontaneous interaction was conducted with a coworker or supervisor, the response for the subjective questions are recorded in the file. The questions are: "Please categorize the interaction," "Was the interaction valuable," "Did you initiate the interaction," and "Did this interaction impact your focus."

`simp_stack_df.csv` - this file contains the data used for plotting "Objective Questions Bar Chart." It contains the counts for each answer choice of the objective microsurvey questions. Question 1 is "Where are you currently located", 2 is "Where were you located at the time of the interaction?", 3 is "With whom?", and 4 is "Have you had a spontaneous interaction since your last survey?"

`Thesh_End_of_Day.csv` - this file contains the end-of-day survey responses. This includes approximate interaction counts and evaluations of the entire day's interactions.


## Visualizations
The folder `visualizations` contains the python files used for creating visualizations. Additionally, it contains the SVG files created directly from the code as well as the image-edited PNG files.

`Results_Figures.ipnyb` - this file contains the code to create two different stacked bar charts (image files "Categorization Breakdown" and "Objective Questions Bar CHart"). The first compares the responses to the microsurvey question "Please categorize this interaction:" given by each participant. The second compares the total response breakdown from all the participants collectively for the objective microsurvey questions (using 'simp_stack_df.csv')


`Sankey_Figure.ipnyb` - this file contains the code to create a sankey plot for the flow of responses through the subjective microsurvey questions.




'


