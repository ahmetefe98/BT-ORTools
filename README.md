# Bachelor thesis: Comparison of several solution methods from the vehicle routing problem for the automation of order planning in maintenance

+ this folder includes the code and the results for my bachelor thesis
+ title: Comparison of several solution methods from the vehicle routing problem for the automation of order planning in maintenance
+ research question: Which solution methods from the vehicle routing problem available in Google OR-Tools achieve the best results for automating order planning in maintenance?

## Prerequisites

+ Python 3.9
+ Google OR-Tools (https://developers.google.com/optimization/install/python)

## Content

+ order_planning.ipynb: calculate an order plan with the given input data and parameters
+ data/original_datasets: includes the original data sets from Solomon (https://www.sintef.no/projectweb/top/vrptw/solomon-benchmark/) and Gehring & Homberger (https://www.sintef.no/projectweb/top/vrptw/homberger-benchmark/)
+ data/selected_datasets: includes only the instances that are of interest to us
+ convert_data.ipynb: convert the data from data/selected_datasets to time matrices and create random service times
+ data/data_for_comparison: includes the time matrices and service times
+ comparison_of_solution_methods.ipynb: compare the solutions methods provided by Google OR-Tools for route planning on the data sets from data/data_for_comparison the results are in the folder results
+ results: includes the files with the results of the comparison
+ create_results_matrix.ipynb: convert the results from the folder results to matrix form in folder results/results_matrix
+ results/results_matrix: includes the results of the comparison in matrix form (first solution strategy x local search strategy)
+ create_relative_results_matrix.ipynb: set all values from the results matrices in relation to the best value and saves it in folder results/results_matrix_relative
+ results/results_matrix_relative: includes the results in relation to the best value
+ evaluation.ipynb: evaluate the results from results/results_matrix_relative to determine the best combinations, best first solution strategy, and best local search strategy for each instance, grouped by the number of orders, grouped by the structure of orders, and overall. The results of the evaluation are in the folder evaluation
+ evaluation/for_each_instance: includes the results of the evaluation to determine the best combinations, best first solution strategy, and best local search strategy for each instance
+ evaluation/grouped_by_number_of_orders: includes the results of the evaluation to determine the best combinations, best first solution strategy, and best local search strategy grouped by the number of orders
+ evaluation/grouped_by_structure_of_orders: includes the results of the evaluation to determine the best combinations, best first solution strategy, and best local search strategy grouped by the structure of orders
+ evaluation/overall: includes the results of the evaluation to determine the best combinations, best first solution strategy, and best local search strategy overall


## Author

+ Ahmet Efe, email: ahmet.efe@stud.uni-heidelberg.de

06.02.2022 Heidelberg, Germany

