# Chord_intersection

Algorithm :

  We can iterate through the list of chords and keep track of the active chords at each radian measure. We can use a data structure like a balanced binary search tree (BST) to efficiently perform insertions and deletions while  iterating through the chords and  counting the intersections along the way.

  The algorithm here processes the start and end events of chords in a circle and maintains a sorted list of active chords using a balanced binary search tree. It iterates through the events and updates the active chords accordingly, counting intersections as 'end' events occur.
  
How to Run:
  1. Install the sortedcontainers library: 
    pip install sortedcontainers
  2. Copy and paste the provided Python code into your script or notebook.
  3. Modify the radian_measures and chord_identifiers lists with your chord data.
  4. Run the script in vscode or jupyter notebook or google colaboratory.


Big-O Runtime Estimate:
  The time complexity of the algorithm, intially was O(n^2). It was later optimized to O(n log n), where n represents the number of chords. The primary contributor to the complexity is the sorting of events. Other operations involve balanced binary search tree operations (specifically, using SortedDict from sortedcontainers), resulting in logarithmic complexity.
