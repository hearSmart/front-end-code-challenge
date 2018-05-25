# Front End Development Challenge

## Overview
You'll be building a fake web hearing screener app built in angular!

## Design and behaviour
In this repo there are 5 wav files for use in the app (100Hz, 250Hz, 440Hz, 1kHz, 10kHz). 

- The first screen will consist of a button with text START. 
- Upon clicking the START button - download the relevant audio files needed for the test. Show a progress bar for indicating download progress.
- When all the files have been downloaded, ask the patient for their first name and email address. Validation should be done on these two inputs. If the form is valid, the button titled NEXT becomes active. 
- Clicking NEXT makes the testing procedure start - In the center of the screen there is a button with an ear icon. 
- On completion of the test, a message should be shown to the user stating their final result (as percentage with category described in Result range categories) with their first name and email address.

The look and feel of the application is up to you, surprise us!

### Testing procedure

The patient will be presented with a set of tones (once per freqency, per ear), when the patient hears a tone, they should press the button to indicate they heard the tone. Between each frequency presentation a jitter from 300ms to 1s (period of silence) will be presented to the patient (the start of the test should also have a silence jitter). The tone should only be played for 1s. 

#### Example 
-- 740ms silence --- 1s of 100Hz tone (left ear)  --- 350ms silence --- 1s of 100Hz tone (right ear) --- 640ms silence --- 1s of 250Hz tone (left ear)  ... etc

#### Result range categories
A tone presentation is considered a pass if the user responds during the 1s of the tone presentation (not during jitter), otherwise that tone presentation is considered a fail. 
The result range categories are as follows: 
- 0 - 2 correct: Severe
- 3 - 5 correct: Moderate
- 6 - 8 correct: Mild
- 9 - 10 correct: Normal

### Remarks 

Treat this as a production ready application. Update the readme to include steps on how to build, run and test the app. 

You are encouraged to include some notes about the aspects you didn't get time to complete and how you would plan to further develop/improve the application given more time. Please include them in this readme rather than in an email so that others can see them when we share your work internally.

We are looking for in your submission:

- Good design decisions
- Creativity
- Originality
- Good user experience
- Code readability
- Modularity 
- Responsive design

### Bonus Marks
- Unit/e2e tests

### Restrictions
- Use Angular 6
- You may use any JS libraries you want
- You may not use any CSS frameworks


### Submission 
The results have to be shared as a git repository

You can either create a private repository on your favourite git hosting provider and then give access to:

- seline@hearxgroup.com
- thomas@hearxgroup.com

Or create a public repository and send the link to both of these email addresses
Or send the whole repository, zipped (including the .git directory) to both of these email addresses
Please only submit your work when it is completely done!
