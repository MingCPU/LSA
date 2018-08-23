# S2MA
S2MA: Steric Substructure Match Algorithm for Bioactive Compound Screening

## Environment
Windows command line

## Fast user guide
**1. S2MA.exe and parameters**<br />
run `S2MA.exe` independently to get all parameters.

Important parameters are as below:<br/>
"-qsd": filepath, the `.sdf` file of the template/query molecule(s).<br/>
"-ssd": filepath, the `.sdf` file of substructure(s) defined on your own.<br/>
"-sd":filepath, the `.sdf` file of molecule(s) to be screened.<br/>
"-sscnt": integer, the number of defined substructures (default: 1)<br/>
"-CC": bool, true for outputting superimposing results of library molecules and the query molecules. (default: false)<br/>
"NW": 0 or 1, please set as 1 handly.

## A simple usage:
`> S2MA.exe -ssd substructure.sd -qsd query.sd -sd library.sd`

## Notes:
`HBA_Exclude.sdf`,`HBD_Exclude.sdf`,`NEG_Included.sdf`,`POS_Included.sdf` are necessary files, do not modify and keep them in the same folder with `S2MA.exe`.
