# Graph Analysis (COL106) - Simulating Indivisual Social Interection

This repository contains the solution for Assignment 4 of the COL106 course, which focuses on graph analysis and algorithms.

## Problem Description

The assignment involves analyzing a graph representation of character co-occurrences in a dataset. The dataset consists of two CSV files:

- `nodes.csv`: Contains 327 nodes, where each node represents a character.
- `edges.csv`: Contains 9891 edges with weights, representing co-occurrences between characters. The weight of an edge indicates the number of times the characters have appeared together.

The goal is to implement various functions to extract meaningful information from the graph:

(a) `average`: This function calculates and prints the average number of characters each Marvel character is associated with. The output is a float value rounded to two decimal places.

(b) `rank`: This function prints a sorted list of all characters based on their co-occurrence count. The list is sorted in descending order of co-occurrence. In case of ties, characters are sorted in descending order of lexicographic order of the character strings. The output is a comma-separated list of character names.

(c) `independent_storylines_dfs`: This function implements Depth-First Search (DFS) to find independent storylines in the graph. An independent storyline is a set of characters that have no edges connecting them to characters in other storylines. The function prints the characters in each independent storyline as separate lines in the output. The storylines are sorted based on the number of characters, with the largest storyline appearing at the top. Within each line, character names are delimited by a comma and sorted in descending lexicographic order. In case of ties in the number of characters, the character names are sorted in descending lexicographic order.

## Running the Code

To run the code, follow these steps:

1. Clone the repository: `git clone https://github.com/AkshatGadhwal/Assignment4_Graphs_COL106.git`
2. Navigate to the project directory: `cd Assignment4_Graphs_COL106`
3. Compile the Java source files: `javac assignment4.java`
4. Run the program with the desired function and input files:

   - For the `average` function: `java assignment4 nodes.csv edges.csv average`
   - For the `rank` function: `java assignment4 nodes.csv edges.csv rank`
   - For the `independent_storylines_dfs` function: `java assignment4 nodes.csv edges.csv independent_storylines_dfs`

## Additional Notes

- The input files `nodes.csv` and `edges.csv` should be present in the same directory as the Java source files.
- The code implements the required functionalities and provides the expected output format.
- Please ensure that you do not use any forbidden imports as mentioned in the `allowed_imports.txt` file.

## Contributions

Contributions to this repository are welcome. If you find any issues or have improvements to suggest, please feel free to open a pull request.

## License

This repository is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

## Acknowledgments

Special thanks to the COL106 course instructors and teaching assistants for providing the assignment problem statement and guidance throughout the course.

Happy coding!
