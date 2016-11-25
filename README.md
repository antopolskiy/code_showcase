# Overview
This is a sample of my data analysis/coding project. Some are related to my work, others I persue in my free time out.

# Projections description
#### Rat behavior: mixed trial analysis

This piece of code analyses behavioral data from a rat experiment. The rat is trained to disriminate vibrations, which are applied to the whiskers. After received the stimulus, the animal can make one of two exclusive choices: attempt to drink from the left water well (further denoted as "go left") or attempt to drink from the right water well (further denoted as "go right"). If the decision is correct (which is determined by a rule binding a certain type of stimulus to a certain side, more on that below), the rat receives a reward in a form of water or diluted juice. If the decision was incorrect, nothing happens. In any case, the rat is free to receive the next stimulus, and thus the process repeats. On average, rats make around 200-300 such attempts ("trials") in ~1 hour, before they are satiated and ready to be put back in their home cage.

The stimuli presented to the rats are noisy vibrations (white noise bandpass filtered in the range 10-150 Hz), modulated by sinusoidal envelopes. Here are the examples of two such stimuli, created by applying 5 Hz (top) and 1 Hz (bottom) envelopes to white noise: 

![Creation of the stimuli](stim_creation.png)

In this project, rats were trained to discriminate 2-second-long noisy stimuli: 5 Hz modulated (must go right to get reward) and 1 Hz modulated (must go left to get reward). At the point of interest for this project, rats reliably discriminated these stimuli with the performance of 70%.
