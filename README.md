Download Link: https://assignmentchef.com/product/solved-cs4375-homework-4-machine-learning-algorithms-in-c
<br>
For this homework you will be implementing 2 machine learning algorithms in C++ and comparing the results and performance to the equivalent functions in R.

For this homework you can work with one other person or work alone if you prefer.

Steps:

<ol>

 <li> Perform logistic regression on the given data set in an <u>R script </u>(not Rmd) using R library functions. Evaluate with the metrics indicated in details below. Your R script should also include at least 2 graphs and 4 R functions for data exploration.</li>

 <li> Write a C++ program to implement logistic regression from scratch, and evaluate with the metrics indicated in details below.</li>

 <li>Perform naive Bayes on the given data set in an <u>R script </u>(not Rmd) using R library functions. Evaluate with the metrics indicated in details below. Your R script should also include at least 2 graphs and 4 R functions for data exploration.</li>

 <li> Write a C++ program to implement naive Bayes from scratch, and evaluate with the metrics indicated in details below.</li>

 <li> Report. Write a summary of the accuracy and performance (run time) of the two approaches. Include screen shots of the R runs and the C++ runs for each algorithm. Cite references (any format) you used for the algorithm, including coding examples. Include screen shots of your R graphs. No particular format is required for either the report or references.</li>

</ol>

Turn in your 2 R scripts, 2 cpp files, data files, and report, zipped together.

Notes:

<ul>

 <li>Indicate in your summary how you computed run times. Here are some suggestions:</li>

 <li>For the R scripts you can use proc.time() at the start and end of the machine learning part of the script and subtract the difference.</li>

 <li>For the C++ programs, your IDE may give run time, otherwise measure from terminal.</li>

 <li>Windows: <u>https://stackoverflow.com/questions/673523/how-do-i-measure-execution-timeof-a-command-on-the-windows-command-line</u></li>

 <li>Mac: <u>https://stackoverflow.com/questions/26466572/mac-os-x-shell-script-measure-timeelapsed</u></li>

</ul>

<u>Note:</u> The timing for the R code should be only that portion running the algorithm, not parts that run data exploration functions or create graphs.

<h1>Details: Logistic Regression</h1>

<ul>

 <li>Data: plasma in library HSAUR. You will need to export it using write.csv() for your C++ program.</li>

</ul>

Use all the data (32 observations) to build the model.

<ul>

 <li>R script:

  <ul>

   <li>train a logistic regression model on all the data, ESR~fibrinogen, using glm() o print the coefficients of the model o build the model “from scratch” in R as shown in the book o make sure you get the same coefficients in each approach o note that we are not doing test set evaluation on this data</li>

  </ul></li>

 <li>C++ program:

  <ul>

   <li>implement in C++ the same steps for logistic regression from scratch o feel free to use whatever data structures you like: arrays, vectors, etc.</li>

   <li>if you have a linux system, you may want to check out the Armadillo library for matrix multiplication: <u>http://arma.sourceforge.net/</u></li>

   <li>feel free to use whatever programming paradigm you like, but make your C++ code fast</li>

  </ul></li>

</ul>

<h1>Details: Naïve Bayes</h1>

<ul>

 <li>Data: Titanic data set “titanic_project.csv” on Piazza. Use the first 900 observations for train, the rest for test.</li>

 <li>R script:

  <ul>

   <li>train a naïve Bayes model on the train data, survived~pclass+sex+age o print the model, which will show all the probabilities learned from the data o test on the test data</li>

   <li>print metrics for accuracy, sensitivity, specificity</li>

  </ul></li>

 <li>C++ program:

  <ul>

   <li>implement naïve Bayes in C++; the code in the book should help o train/test on the same data as in the R script; output the same metrics o feel free to use whatever data structures you like: arrays, vectors, etc. o Here is a great video that gives a conceptual picture of naïve Bayes with Gaussian predictors: <u>https://www.youtube.com/watch?v=r1in0YNetG8</u></li>

   <li>The following formula shows how to calculate the likelihood of a continuous predictor. The book gives hints as well..</li>

  </ul></li>

</ul>

<ul>

 <li>Report o Write a summary of the two implementations, R and C++. Did you get the same results?</li>

</ul>

How do the run times compare? How did you measure execution time?

<ul>

 <li>Include screen shots of the output of each program o Include screen shots of the run times of each program o Write out the algorithm you used for training the classifier o Cite all references used o No required format for the report</li>

</ul>

<ul>

 <li>Be prepared to demo your code.</li>

</ul>


