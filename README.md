# directory_to_look
directory 

this is a small code to solve a problem on PTC CREO. 
When you open a CREO assembly models, it looks for components files in the same folder where you saved the assembly model. This works for small assemblies. if you have a big project with components in different folders, CREO won't find the components. 
If you are not using a PLM this is a problem. for this reason PTC created a configuration called search_path. Thanks to this configuration you can create a file, commonly called search.pro, inside of which  are present the different directory where CREO searches for the diffent assembly's pieces.

This is great, but what if you work in a big team who is constantly updating its inventory/directory name?
This program solves this problem.

Once launched, it needs in input the main directory where to look for assembly's parts and the directory where the config.pro file is present. Afterwards it automatically searches for directories and saves them in a file.pro and updates the config.pro file.
eB aware that the search.pro file must be in the same directory of the config.pro file.
