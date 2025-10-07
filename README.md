# PDB database creation
CREATE PLUGGABLE DATABASE pa_pdb_28270;
  ADMIN USER Pacifique_plsqlauca_28270 IDENTIFIED BY "Pa@123456";
  FILE_NAME_CONVERT = ('/opt/oracle/oradata/ORCLCDB/pdbseed/', '/opt/oracle/oradata/ORCLCDB/pa_pdb_28270/');
![](https://github.com/i-paccy/new-plsql/blob/main/Screenshot%202025-10-07%20at%2020.46.48.png?raw=true)

ALTER PLUGGABLE DATABASE pa_pdb_28270 OPEN;
![Sample table](https://github.com/i-paccy/new-plsql/blob/main/1.png?raw=true)
ALTER PLUGGABLE DATABASE pa_pdb_28270 SAVE STATE;

![](https://github.com/i-paccy/new-plsql/blob/main/2.png?raw=true)

ALTER SESSION SET CONTAINER = pa_pdb_28270;

![](https://github.com/i-paccy/new-plsql/blob/main/3.png?raw=true)

GRANT DBA TO Pacifique_plsqlauca_28270;

![](https://github.com/i-paccy/new-plsql/blob/main/4.png?raw=true)

## SECOND QUESTION
CREATE PLUGGABLE DATABASE pa_to_delete_pdb_28270
  ADMIN USER Pacdelete_plsqlauca_28270 IDENTIFIED BY "Pa@123456789"
  FILE_NAME_CONVERT = (
    '/opt/oracle/oradata/ORCLCDB/pdbseed/',
    '/opt/oracle/oradata/ORCLCDB/pa_to_delete_pdb_28270/'
  );
![Table](https://github.com/i-paccy/new-plsql/blob/main/D1.png?raw=true)
![](https://github.com/i-paccy/new-plsql/blob/main/D2.png?raw=true)
![](https://github.com/i-paccy/new-plsql/blob/main/D3.png?raw=true)
![](https://github.com/i-paccy/new-plsql/blob/main/D4.png?raw=true)
![](https://github.com/i-paccy/new-plsql/blob/main/D5.png?raw=true)

ALTER PLUGGABLE DATABASE Pa_to_delete_pdb_28270 CLOSE IMMEDIATE;
![Table](https://github.com/i-paccy/new-plsql/blob/main/D6.png?raw=true)
