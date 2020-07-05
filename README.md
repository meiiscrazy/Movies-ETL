# Movies-ETL
# Challenge Analysis Assumptions
Assumption 1: We are assuming both csv's have a column named "imdb_id" which is why we inserted the try-except block incase a csv does not have "imdb_id" column.
Assumption 2: This function only works if the person running the function has all files necessary to run the function, so we're assumming whoever is running the function has all the necessary files. 
Assumption 3: We are assuming all the files we have are clean, if not our function will help clean the data for us
Assumption 4: When cleaning out the movie data file, we included some key values to try and find alternative titles. We need to assume that we listed out all the key values and alternative titles. If we did not get all of the key values then our data would be need more cleaning.
Assumption 5: Because I tested out this function multiple times, the database may already include a table called "movies" or "ratings". Assuming the database isn't cleared, I added ```if_exists="replace"``` to the code in case my database isn't clear. 
