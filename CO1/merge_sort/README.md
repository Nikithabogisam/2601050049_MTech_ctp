Description
This project contains a Python script that determines the proximity of students based on their 2D coordinate positions. It implements a closest pair algorithm (using Euclidean distance) to analyze a set of student coordinates and identify the two students who are standing closest to each other.

Algorithm
The core logic of the system follows this step-by-step algorithm:

Start
Initialize Data: Define a list of students and their corresponding (X, Y) coordinate positions.
Display Positions: Print the current positions of all students.
Calculate Distances: Iterate through all possible pairs of students and calculate the Euclidean distance between them.
Find Minimum: Compare the calculated distances to find the smallest value, keeping track of the two students associated with that minimum distance.
Display Result: Print the names of the two closest students and the distance between them.
Input and Output
--- Student Positions ---
Ravi : (2, 3)
Sita : (10, 15)
John : (4, 5)
Anu : (20, 25)
Rani : (8, 12)

--- Closest Students ---
Students: Ravi and John
Distance: 2.83
