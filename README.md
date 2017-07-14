# Classifier
This project contains an algorithm based on a decision tree where each node spawns n more where n is the number of catagories in the classification problem.  
  
At each node, each variable is analysed with 17 different functions, looking for windows in these functions where the purity of events that fit into one catagory is high(inclusion) or low(exclusion).
The events in the inclusive window are given a high probability of being in the given catagory while those in the exclusive window are given a low probability of being in the given catagory.
The data is then split into n branches that lead to new nodes, one for each of the catagories to be classified.  
  
The catagories being refered to here are those of the classification problem and must be discrete. In the training data, they must be labelled as ascending integers starting from 0.  
Purity of a window is the number of events within the window that fit into a catagory, divided by the total number of events in that window. Hence a purity close to 1 suggest a window has been found that is a strong suggestor of an event being of that catagory.
