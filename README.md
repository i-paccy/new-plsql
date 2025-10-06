# PDB database creation 
create PLUGGABLE DATABASE &&Pa_PDB_28270;
ADMIN USER &&Pacifique_plsql_28270 IDENTIFIED BY "Pl@123";
![Sample table](https://github.com/i-paccy/new-plsql/blob/main/Screenshot%202025-10-06%20at%2019.35.59.png?raw=true)

## SECOND QUESTION
CREATE PLUGGABLE DATABASE &&Pa_to_delete_pdb_28270;
ALTER PLUGGABLE DATABASE Pa_to_delete_pdb_28270 CLOSE IMMEDIATE;
