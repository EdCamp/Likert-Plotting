# Likert-Plotting
Simple code using HH package (program R) to visualize before/after likert surveys

Set up to read in simple .csv file containing likert responses to pre/post survey questions.
Column 1 should be responder id. Column 2 should be pre/post ("pre" or "post")
Columns 3:dim(df)[2] (i.e. 3:number of columns) should be ONLY responses to question.  Other covariates should be stripped for analysis. 

Input

setwd and dat should obviously match file path and name respectively
ncovcol is assumed to always be 2.  Can be changed if other covariates exist
nquest should calculate correctly assuming all covariates to LEFT of questions, and ncovcol set correctly
nlikert is the number of scales of the likert question
colunames(xx) is where you need to changge the likert scale questions
