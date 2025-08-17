# EdTech-Case-Study
Case Study for a Data Scientist position at Oviva

Background
LEARNIFY provides digital learning tools for K-12 students, which are adopted by schools and
recommended by teachers to their students.
To boost platform usage, LEARNIFY runs targeted engagement campaigns with schools and
teachers using a dedicated outreach team.
Over the past year, the team experimented with various interventions to increase the number of
student activations from each school. The resulting data was collected but not yet analyzed.

Data
- Each row in activations.csv represents a student activation, i.e., a student signing up
for and using LEARNIFY on their teacher’s recommendation.
- Each row in interventions.csv represents an intervention on a school.
- Time window: Data spans 2024-01-01 to 2024-12-31.

Assumptions
- The number of activations per school over time is modeled as Poisson-distributed, i.e.,
Ni~Poisson(𝛌i), where i denotes the school.
- Interventions have a non-negative and immediate effect on 𝛌i.
- No decay in intervention effectiveness over time.
- No interaction effects among interventions.
- All schools are assumed to be active (no dropout/churn) throughout the observation
window.

Questions answered:
1. How effective are the interventions?
Estimate the expected additional student activations per month per intervention by
providing a lower and upper confidence/credibility bound for each intervention.

2. Onsite school visits incur higher costs (travel & time) than virtual workshops.
How confident are you that onsite visits are worth continuing, considering they must be
at least twice as effective as virtual workshops to be cost-justified?


Hint: Given that schools might vary in total number of teachers and pupils, mind that each
school will have a different baseline activation rate
