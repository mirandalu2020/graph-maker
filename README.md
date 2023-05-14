# Polynomial Approximation for Titration Data

This repository provides a Python implementation for using polynomial approximation to analyze and visualize titration data. The goal is to approximate the titration curve using polynomial functions, allowing for a better understanding and interpretation of the experimental data.

## Table of Contents
- Introduction
- Requirements
- Usage
- Credits

## Introduction

Titration is a common laboratory technique used to determine the concentration of a solution by reacting it with a standard solution of known concentration.  The resulting titration curve represents the relationship between the volume of the titrant solution added and the pH, conductivity, or some other measurable property of the solution being analyzed. Details of how a titration work can be viewed [here](https://en.wikipedia.org/wiki/Titration). If the titration is performed manually, a visual indicator can be used to apporximate the pH value. However, in order to quantify the data, the first or second derivative of the curve is used. Typically, a well-performed titration should resolve to curve closer to a sigmoid curve, where the inflection points are the pH vlaue of the given solution. 

The data sample used in this project comes from a titration experiment that was poorly collected. The solution was Na<sub>2</sub>SO<sub>3</sub>, which has two equilibrium pH as it can take on two protons. However due to human error, when collecting the data for the second equivalence point, the solution was not heated. As a result, the solution's pH data were altered due to water molecule in air, and the resulting curve does not fit to a standard titration curve and the first and second derivative were not well-defined without a mathematical equation. In this project, two mathematical models were used to fit the data, Sigmoid and Polynomial. 

A well-performed titration highly resembles the sigmoid curve, so for the first half of the data, a sigmoid curve was used to find the inflection point, and a polynomial curve was used to find the second infleciton point. A polunomial curve was chosen since a polynomial approximation is a mathematical method that allows us to approximate complex data with a polynomial function. By applying polynomial approximation to titration data, we can obtain a simplified representation of the titration curve, which can be useful for analysis, visualization, and prediction purposes.

This repository provides a Python script that takes titration data as input and performs polynomial approximation to generate a fitted curve. It also includes functions for plotting the original data and the fitted curve, allowing for easy visualization and comparison.

## Requirements 

To use the polynomial approximation script, you need to have the following installed:

Python 3.x
NumPy
Matplotlib
Scipy
  
## Credits
  
This project was done as a class project for CHE155 at UC Davis.
