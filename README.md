# occupant-interactions-workspaces
Pilot data on identifying and contextualising occupant interactions within hybrid workspaces using the Cozie app on Apple smartwatches


The folder `data` contains all the data from the field experiment.

The field experiment involved:
9 participants working in the same office building in Singapore
5 Male and 4 Female
Ages ranging from 25 to 41

'Thesh_Onboarding.csv' - this file contains the onboarding survey responses. This includes demographic information, perceptions of office work and scheduling, and personality tests.

'Microsurvey_Dataframe.csv' - this file contains the total raw data collected from the Cozie app. This includes the microsurvey response and the associated metadata/environmental variables (timestamp, location, heartrate, etc.). This data file was used for the 

`sankey_plot.csv` - this file contains a subset of the microsurvey response data for plotting a sankey diagram. For every microsurvey response where a spontaneous interaction was conducted with a coworker or supervisor, the response for the subjective questions are recorded in the file. The questions are: "Please categorize the interaction," "Was the interaction valuable," "Did you initiate the interaction," and "Did this interaction impact your focus."

'simp_stack_df.csv' - this file contains the data used for plotting _ It contains the counts for each answer choice of the objective microsurvey questions. Question 1 is "Where are you currently located", 2 is "Where were you located at the time of the interaction?", 3 is "With whom?", and 4 is "Have you had a spontaneous interaction since your last survey?"

'Thesh_End_of_Day.csv' - this file contains the end-of-day survey responses. This includes approximate interaction counts and evaluations of the entire day's interactions.


The folder 'visualizations' contains the python files used for creating visualizations. Additionally, it contains the SVG files created directly from the code as well as the image-edited PNG files.

'Results_Figures.ipnyb' - this file contains the code to create two different stacked bar charts. The first compares the responses to the microsurvey question "Please categorize this interaction:" given by each participant. The second compares the total response breakdown from all the participants collectively for the objective microsurvey questions (using 'simp_stack_df.csv')

'Sankey_Figure.ipnyb' - this file contains the code to create a sankey plot for the flow of responses through the subjective microsurvey questions.




'


