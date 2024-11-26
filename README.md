# Ford-Fulkerson
The code provided solves an arrangement problem. The goal is to assign people to activities or places, ensuring that there are at least two leaders for each activity or place. Leaders must be both interested and experienced (value 2) if they wish to engage in the activity or visit the place. People who are not interested (0) will not be included in any team.

Assumptions:
The total demand of all places will always equal the total number of people available.

The assign function takes two inputs and returns a nested list.

Inputs
A list of numbers:
Represents the minimum number of people required for each place.
Example:
[1, 3, 4] means:

- The first place needs at least 1 person.
- The second place needs at least 3 people.
- The third place needs at least 4 people.

A list of lists of numbers:
Represents each person’s interest in each place:

- 0 means no interest.
- 1 means interested but no experience.
- 2 means interested and experienced.
Example:
places: [1, 3, 4] (3 places).
people: [[0, 1, 2], [1, 1, 2], [2, 2, 2]] (3 people).


Output
A nested list indicating the assignment of people to places. Each sublist corresponds to a place, containing the indices of the assigned people.

Example:

Input:
places: [2, 3]
people: [[2, 1], [2, 2], [1, 1], [2, 1], [0, 2]]
Output:
[[0, 3], [1, 4, 2]]
This means:

Index 0 and index 3 people are assigned to place 0.
Index 1, index 4, and index 2 people are assigned to place 1.

