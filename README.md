This project explores a graduate employability dataset to identify which student characteristics have the strongest impact on job placement outcomes.
The goal is to understand what truly matters: GPA? Communication skills? IQ? Projects? Or other attributes?


Each row represents one student, with fields including:
	•	IQ
	•	Previous Semester Result
	•	CGPA (converted to a 4.0 scale)
	•	Academic Performance
	•	Internship Experience
	•	Extra-Curricular Score
	•	Communication Skills
	•	Projects Completed
	•	Placement (Yes / No)


GPA Conversion
The dataset used a 10-point CGPA scale. I standardized it using:

\text{GPA\_4} = \left( \frac{\text{CGPA}}{10} \right) \times 4

Which features are the strongest predictors of whether a student gets placed?
This is answered using:
	•	Random Forest classification
	•	Permutation feature importance
	•	Accuracy evaluation
	•	Visual analysis

  
