# openmmawsem
An implementation of the AWSEM coarse-grained protein folding forcefield in OpenMM

Example:
1r69.

steup simulation folder:
```
python3 YOUR_OPENAWSEM_LOCATION/mm_create_project.py 1r69 --frag
```

run the simulation:
```
python3 mm_run.py 1r69
```

compute energy and Q:
```
python3 mm_analysis.py 1r69 > energy.dat
```  
In comparison with the previous version, the q_value calculation inside the code has been modified in accordance with the default CACA Q as defined as Qw and Qo. There is a Qflag inside the newly added function (0 for Qw, 1 for Qo)
