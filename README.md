# LSA
LSA: a local-weighted structure alignment tool for pharmaceutical virtual screening

## Environment
Windows command line or Linux OS

## Fast user guide
**1. LSA.exe and parameters**<br />
run `LSA.exe` independently to get all parameters.

Important parameters are as below:<br/>
"-qsd": filepath, the `.sdf` file of the template/query molecule(s).<br/>
"-ssd": filepath, the `.sdf` file of substructure(s) defined on your own.<br/>
"-sd":filepath, the `.sdf` file of molecule(s) to be screened.<br/>
"-sscnt": integer, the number of defined substructures (default: 1)<br/>
"-CC": bool, true for outputting superimposing results of library molecules and the query molecules. (default: false)<br/>

## A simple usage:
the example files are in `example`, command line can be <br/>
`> LSA.exe -sd example/hdac8_library.sd -qsd example/hdac8_template.sd -ssd example/hdac8_sub.mol -CC true`

## Notes:
`HBA_Exclude.sdf`,`HBD_Exclude.sdf`,`NEG_Included.sdf`,`POS_Included.sdf` are necessary files, do not modify and keep them in the same folder with `LSA.exe`.
