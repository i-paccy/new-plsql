# PDB database creation
CREATE PLUGGABLE DATABASE pa_pdb_28270;
  ADMIN USER Pacifique_plsqlauca_28270 IDENTIFIED BY "Pa@123456";
  FILE_NAME_CONVERT = ('/opt/oracle/oradata/ORCLCDB/pdbseed/', '/opt/oracle/oradata/ORCLCDB/pa_pdb_28270/');
![](https://github.com/i-paccy/new-plsql/blob/main/Screenshot%202025-10-07%20at%2020.46.48.png?raw=true)

ALTER PLUGGABLE DATABASE pa_pdb_28270 OPEN;
![Sample table](https://github.com/i-paccy/new-plsql/blob/main/1.png?raw=true)
ALTER PLUGGABLE DATABASE pa_pdb_28270 SAVE STATE;



ALTER SESSION SET CONTAINER = pa_pdb_28270;

GRANT DBA TO Pacifique_plsqlauca_28270;


## SECOND QUESTION
CREATE PLUGGABLE DATABASE &&Pa_to_delete_pdb_28270;
ALTER PLUGGABLE DATABASE Pa_to_delete_pdb_28270 CLOSE IMMEDIATE;
![Table](https://github.com/i-paccy/new-plsql/blob/main/Screenshot%202025-10-06%20at%2020.26.41.png?raw=true)

ALTER PLUGGABLE DATABASE Pa_to_delete_pdb_28270 CLOSE IMMEDIATE;
![Table](https://github.com/i-paccy/new-plsql/blob/main/Screenshot%202025-10-06%20at%2020.42.38.png?raw=true)
