**How to use FunctionAnalysis.py**

 * Enter the repo folder in the command line (make sure your isolated stacktrace csv file is in the folder)

 * The required arguments are the name of your csv file, followed by whether or not you want to exclude kernel and runtime functions

 * an example would be `python FunctionAnalysis.py my_csv_file.csv true`

 * This will print out a list of functions followed by the number of times this function appears in your stacktrace table.

 * Use this information to determine which functions are being called more/less

 * There is also an optional argument that is reserved for the name of a function you want to analyze

 * an example would be `python FunctionAnalysis.py my_csv_file.csv false syscall.write"`

 * This will print out a list of functions that follow that function anywhere in the stack trace table, so if you see a function getting called more often then you expect you can enter that function into the command line and see what other functions it is leading to

(NOTE: if you want to enter a series of functions as your search argument separate them by ';')  
