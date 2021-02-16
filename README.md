# cons
ISPF command to issue system console commands

CONS is a REXX exec intended to be defined in the ISPF command table to issue  
system commands using SDSF.                                                    
                                                                               
Example command syntax (from any ISPF panel)                                   
                                                                               
Command ===> CONS D OMVS,O                                                     
                                                                               
Add to the ISPF command table:                                                 
                                                                               
Verb:   CONS                                                                   
Trunc:  4                                                                      
Action: SELECT CMD(%CONS &ZPARM)                                               
Description: Issue system console commands                                     
