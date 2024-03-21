# AHP-ANP-Decision-making-Software
This project started after being challenged by my professor to translate our decision-making class into a viable digital alternative.

This piece of software implements Multi-Criteria Decision Making (MCDM) methods, specifically the Analytic Hierarchy Process (AHP) and the Analytic Network Process (ANP) to provide sophisticated platforms for evaluating various options against a set of criteria. This kind of tool is valuable in helping decision-makers assess complex scenarios where multiple, often conflicting, criteria need to be considered.

Brief How-To-Guide:


How it Works:
#Input:
The input_matrix function prompts you to enter values for a pairwise comparison matrix. This matrix represents how much more important one element is over another.

#Normalization:
The comparison matrix values are normalized to ensure that each element reflects its relative importance. This is done by dividing each entry by the sum of its column, resulting in each column summing to one.

#Priority Vector:
The calculate_priority_vector function computes the priority vector by averaging the normalized values of each row. This vector represents the relative weights of the criteria or alternatives.

#Consistency Check:
The consistency_ratio function checks if the judgments made in the pairwise comparison matrices are consistent. It calculates the largest eigenvalue of the matrix (λ max), the Consistency Index (CI), and then the Consistency Ratio (CR) using the Random Index (RI) values. A CR less than 0.1 generally indicates a reasonable level of consistency.

#Aggregating Priorities:
Finally, the priority vectors for the alternatives are aggregated with respect to the criteria weights to obtain a final score for each alternative. The alternative with the highest score is considered the best option according to the AHP.
