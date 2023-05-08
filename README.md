Download Link: https://assignmentchef.com/product/solved-syde544-assignment-3-eeg-sensory-motor-rhythm-calculation
<br>
As we discussed in the lectures, one of the widely used BCI modality is Event-related Desynchronization and Event-related Synchronization (ERD/ERS), or Sensor-motor Rhythm (SMR). The SMR processing is nicely illustrated in the figure above [1].

In the above figure, time zero (t=0) is the time when a motor or sensory task is performed. For this exercise, the data file attached contains two types of sensory attention tasks: the subject was focusing her attention to stimulus coming from either left or right hand, while both hands were being stimulated by a tactile stimulator at t=0. For each of the two tasks, 60 repetitions (trials) were performed, with random intervals between consecutive trials. Here, for simplicity, we look at the general SMR frequency band, <em>i.e. </em>[8, 26] Hz, rather than specific sub-bands (line 16 of the main script).

The data file contains 62 EEG channels (62 rows). The channel map are shown below (1020 channel names on the left, and channel number on the right):




According to the figures, channel C3 is the 26<sup>rd</sup> row of the data matrix (line 32) and channel C4 is the 30<sup>th</sup> row of the data matrix (line 33). The 63<sup>rd</sup> row of the matrix indicates when a task was performed, and which task was performed. Such as, the starting time (t=0) for each trial was obtained between line 24 and line 26 of the main script. Other relevant parameters of the processing are clearly commented in the main script before line 26.

<strong> </strong>

<h2>Problem 1</h2>

Complete the Matlab function: <em>mySMRCalculation.m</em> (5 pts), following the steps illustrated in the first figure. DO NOT change the given input/output syntax of the function. Run the code to line 65, observe the generated graph and comment your observation (3 pts).

<h2>Problem 2</h2>

Finish the script up to line 78, so you can perform large Laplacian filtered version of C3 and C4 (3 pts), calculate the corresponding SMR values (1 pts), and generate the graph similarly to the provided code in Problem 1, by completing the code between line 81-103 (1 pts). Observe and comment on the generated graph, in relation to the observation you had for Problem 1 (3 pts).

<h2>Problem 3</h2>

Complete the Matlab function: <em>mySMRCalculationCSP.m</em> (10 pts), so you can perform common spatial pattern filtering, as we discussed in lecture [2]. Generate the graph similarly to the provided code in Problem 1 and 2, by completing the code between line 113-139 (1 pts). Observe and comment on the generated graph, in relation to the observation you had for Problem 1 and 2 (3 pts).




<strong><u>Reference:</u> </strong>

<ul>

 <li>Pfurtscheller and F. H. Lopes Da Silva, “Event-related EEG/MEG synchronization and desynchronization: basic principles.,” <em>Clin. Neurophysiol.</em>, vol. 110, pp. 1842–1857, 1999.</li>

 <li>Blankertz, R. Tomioka, S. Lemm, M. Kawanabe, and K. Muller, “Optimizing Spatial filters for Robust EEG Single-Trial Analysis,” <em>IEEE Signal Process. Mag.</em>, vol. 25, no. 1, pp. 41–56, 2008.</li>

</ul>


