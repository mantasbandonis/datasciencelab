Data Science SBWL Course V
Multi Label Classification with data from the Worldbank.

How to set up the environment:


1) 4 separate jupyter notebooks, data is shared by csv exports, tested pip environments can be found in folder environments


2) file system must be structured as noted below:

			- notebooks
				-preparation.ipynb
				-vectorisation.ipynb
				-ML.ipynb
				-LabelMyData.ipynb
				- single_cases.csv		# one column containing descriptions of datasaets, another column containing titles
			- output
			- input
				- fillerwords.txt		# must contain words and characters which should be removed from the text, comma seperated list
				- tags_clean.csv		# contains a column of all tags, their frequency and an identifier if a tag should be removed
			- token
				- token.txt				# token for accessing the API to download the JSON files, must be requested
 
				
3) for executing vectorisation.ipynb the word embedding model set up on the server of the Wirtschaftsuniversität Wien must be reachable
	- alternatively a local word embedding model must be set up 

4) notebooks must be run in following order:
			1. preparation.ipynb
			2. vectorisation.ipynb
			3. ML.ipynb
			4. LabelMyData.ipynb