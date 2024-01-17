# directory_to_look
directory 

this is a small code to solve a problem on PTC CREO. 
when you open a CREO assembly models, he looks for components files in the same folder where you saved the assembly model. this works for small assemblies. if you have a big project with components in different folders, CREO won't find the components. 
if you are not using a PLM this is a problem. for this reason PTC created a configuration called search_path. thanks to this configuration you can create a file, commonly called search.pro, inside of which  are present the different directory where CREO searches for the diffent assemblies'pieces.

this is great, but what if you are consantly changing because you are a big team who needs to constnaly update its inventory? 

Once launched, given the program the main directory where to look, it automatically searches for directories and saves them in a file.pro and updates the config.pro file.
be aware that the search.pro file must be in the same directory of the config.pro file.
