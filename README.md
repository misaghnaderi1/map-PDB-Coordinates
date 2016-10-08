# map-PDB-Coordinates
This only works for exactly similar PDB coordinates in two PDB files

In here I'm getting the Chain_ID of the coordinates that are presented in another PDB as the pocket. 
Any other attribute could be easily retrieved while the entire PDB file was in the Pandas DataFrame format. protein.df or pocket.df

Instead of using coordinates as floats I have combined them into a string to be able to use .isin(). 
If the coordinates are not exactly the same then they can be used as floats and distance can be calculated for two sets of coordinates to find corresponding sets. 

