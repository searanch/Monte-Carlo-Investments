# Monte-Carlo-Investments
Intial code for a Monte Carlo Simulation written in Julia, a luanguage that I have started to learn. This project is a very much a work in progress. Right now I'm using 20 chained functions. This certainly could be optimized to make the code more readable and have better performance. I also plan on adding visulizations. 

OVERVIEW

The Monte Carlo Model is a set of functions that simulate potential financial returns based on historical returns of the S&P 500 over 20 years. This project assumes an all-stock portfolio, starting with an initial investment of $10,000 and additional contributions of $21,000 each year.

USAGE

The project consists of 20 functions, y1 through y20, that simulate returns for each year, respectively, and a final function, make_model, that combines all 20 functions to produce a DataFrame with the total return for year 20. The odds function calculates the percentiles of the total return values in the DataFrame.

To use the model, simply call the make_model function:

make_model()

This will return a DataFrame with the total return for year 20.

To calculate the percentiles, call the odds function:

odds()

This will return the 10th, 70th, 80th, and 90th percentiles of the total return values.

DEPENDENCIES

This project requires the use of the Statistics.jl package, using Random.jl, Distributions.jl DataFrames.jl CSV.jl Plots, StatsPlots.jl
Contributing


Disclaimer:

This project is for educational purposes only and should not be used as a basis for making financial decisions. Historical returns are not indicative of future results, and past performance is not a guarantee of future success. Always consult a financial advisor before making investment decisions.
