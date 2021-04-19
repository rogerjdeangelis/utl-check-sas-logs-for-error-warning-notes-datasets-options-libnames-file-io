# utl-check-sas-logs-for-error-warning-notes-datasets-options-libnames-file-io
Check sas logs for error warning notes datasets options libnames file-io
    Check sas logs for error warning notes datasets options libnames file-io;                                                               
                                                                                                                                            
    This requires the Classic 1980s SAS editor.                                                                                             
        You can run the log check from a function key. keystroke or a mouse action.         
    Here is how.                                                                        
                                                                                        
    if the cwd, curent workinf directory, is C;/utl and                                 
    you put this on a function key                                                      
                                                                                        
    home;log;home;file c r;gsubmit '%utl_logcurchk(.\c.log,.\c.txt);'                    
                                                                                        
    Here is what wil happen                                                             
                                                                                        
       1. The current contents of the log will be saved in c:/utl/c.log                 
       2. gsubmit '%utl_logcurchk(c:/utl/c.log);'  will run the macro                   
       3. Editor window 'note i.i' will popup witht he results of the logchecl          
       4. Editor window 'note h.h' will have the log                                    
                                                                                        
                                                                                                                                        
    If editor windows 'note i.i;'(log check), and 'note h.h;'(orginal log) do not pop up in                                                 
    your interactive session then just type note h.h and note i.i on any 1980s clean classic command line;                                  
                                                                                                                                            
    github                                                                                                                                  
    https://tinyurl.com/ydxazovx                                                                                                            
    https://github.com/rogerjdeangelis/utl-check-sas-logs-for-error-warning-notes-datasets-options-libnames-file-io                         
                                                                                                                                            
    Also see                                                                                                                                
    https://tinyurl.com/y77ed56c                                                                                                            
    https://documentation.sas.com/?docsetId=proc&docsetTarget=p0sf63lx4fs2m5n14qv1bn8p863v.htm&docsetVersion=9.4&locale=en                  
                                                                                                                                            
    SAS Forum                                                                                                                               
    https://tinyurl.com/y7fjmo8y                                                                                                            
    https://communities.sas.com/t5/New-SAS-User/Count-all-created-referenced-tables-in-a-SAS-Program/m-p/658935                             
                                                                                                                                            
    *_                   _                                                                                                                  
    (_)_ __  _ __  _   _| |_                                                                                                                
    | | '_ \| '_ \| | | | __|                                                                                                               
    | | | | | |_) | |_| | |_                                                                                                                
    |_|_| |_| .__/ \__,_|\__|                                                                                                               
            |_|                                                                                                                             
    ;                                                                                                                                       
                                                                                                                                            
    d:/log/sample.log;                                                                                                                      
                                                                                                                                            
    1          The SAS System      11:26 Thursday, September 5, 1996                                                                        
                                                                                                                                            
    NOTE: Copyright (c) 1989-1995 by SAS Institute Inc., Cary, NC, USA.                                                                     
    NOTE: SAS (r) Proprietary Software Release 6.11  TS020                                                                                  
                                                                                                                                            
                                                                                                                                            
                                                                                                                                            
    This message is contained in the SAS news file, and is presented upon                                                                   
    initialization.  Edit the files "news" in the "misc/base" directory to                                                                  
    display site-specific news and information in the program log.                                                                          
    The command line option "-nonews" will prevent this display.                                                                            
                                                                                                                                            
                                                                                                                                            
                                                                                                                                            
    NOTE: AUTOEXEC processing beginning; file is /mercury/src/BMS/srs2/u05/autoexec.srs.                                                    
                                                                                                                                            
    NOTE: SAS initialization used:                                                                                                          
          real time           3.711 seconds                                                                                                 
          cpu time            0.508 seconds                                                                                                 
    MPRINT(UTLOPTS):   NOTES NOOVP CMDMAC MEMSIZE=0 ERRORS=2 SOURCE2 MLOGIC MPRINT NOCENTER                                                 
    LS=91 PS=63 MTRACE NUMBER FULLSTIMER NODATE;                                                                                            
    MPRINT(UTLOPTS):   RUN;                                                                                                                 
    ....                                                                                                                                    
                                                                                                                                            
    *            _               _                                                                                                          
      ___  _   _| |_ _ __  _   _| |_                                                                                                        
     / _ \| | | | __| '_ \| | | | __|                                                                                                       
    | (_) | |_| | |_| |_) | |_| | |_                                                                                                        
     \___/ \__,_|\__| .__/ \__,_|\__|                                                                                                       
                    |_|                                                                                                                     
    ;                                                                                                                                       
                                                                                                                                            
    Scrubbed log in d:/log/sample.txt                                                                                                       
                                                                                                                                            
    Original log in note h.h;                                                                                                               
    Scrubbed log in note i.i;                                                                                                               
                                                                                                                                            
    FULL_PATH  d:/log/sample.txt                                                                                                            
    LOG_TIME   11:26 Thursday, September 5, 1996                                                                                            
    SCRUB_TIME 11:30 Monday, June 15, 2020                                                                                                  
    ERROR      28                                                                                                                           
    WARNING    17                                                                                                                           
    NOTES      15                                                                                                                           
    DATASETS   2                                                                                                                            
    OPTIONS    0                                                                                                                            
    FILE_IO    15                                                                                                                           
    ----------------------------------------------------------------------------------------------------------------------                  
    ERROR      ERROR: Format DIFDLR not found or couldn't be loaded.                                                                        
    ERROR      ERROR: File UIN12.U05CA002.DATA does not exist.                                                                              
    ERROR      ERROR: Variable CALC_YTD not found.                                                                                          
    ERROR      ERROR: File UIN22.U05CA002.DATA does not exist.                                                                              
    ERROR      ERROR: File UIN12.U05CA003.DATA does not exist.                                                                              
    ERROR      ERROR: File UIN11.U05AA002.DATA does not exist.                                                                              
    ERROR      ERROR: File UIN22.U05BA002.DATA does not exist.                                                                              
    ERROR      ERROR: File UIN21.U05DA002.DATA does not exist.                                                                              
    ERROR      ERROR: File UIN21.U05DA003.DATA does not exist.                                                                              
    ERROR      ERROR: Errors printed on pages 7,9,10,12,13.                                                                                 
    ERROR      ERROR: File UIN22.U05BA003.DATA does not exist.                                                                              
    ERROR      ERROR: File UIN21.U05AA003.DATA does not exist.                                                                              
    ERROR      ERROR 31-185: Format $PRD2RPT is unknown.                                                                                    
    ERROR      ERROR: File UIN21.U05AA002.DATA does not exist.                                                                              
    ERROR      ERROR: File UIN22.U05CA003.DATA does not exist.                                                                              
    ERROR      ERROR: File UIN11.U05DA003.DATA does not exist.                                                                              
    ERROR      ERROR: Variable ACT_YTD not found.                                                                                           
    ERROR      ERROR: Variable CUR_MTH not found.                                                                                           
    ERROR      ERROR: Variable MKTPRD not found.                                                                                            
    ERROR      ERROR: Variable PRE_YTD not found.                                                                                           
    ERROR      ERROR: Variable LCAT not found.                                                                                              
    ERROR      ERROR: File UIN11.U05AA003.DATA does not exist.                                                                              
    ERROR      ERROR 31-185: Format $BMP2NAM is unknown.                                                                                    
    ERROR      ERROR: File UIN12.U05BA003.DATA does not exist.                                                                              
    ERROR      ERROR: File UIN11.U05DA002.DATA does not exist.                                                                              
    ERROR      ERROR: Variable DPCT_YTD not found.                                                                                          
    ERROR      ERROR: File UIN12.U05BA002.DATA does not exist.                                                                              
    ERROR      ERROR: Variable DIFF_YTD not found.                                                                                          
    ----------------------------------------------------------------------------------------------------------------------                  
    WARNING    WARNING: The BASE Product product with which FORMAT is associated will expire within 30                                      
    WARNING    WARNING: The data set WORK.U0505AA6 may be incomplete.  When this step was stopped there                                     
    WARNING    WARNING: Variable CUR_MTH not found in data set WORK.U0505AA7.                                                               
    WARNING    WARNING: Variable CALC_YTD not found in data set WORK.U0505AA7.                                                              
    WARNING    WARNING: Variable ACT_YTD not found in data set WORK.U0505AA7.                                                               
    WARNING    WARNING: The BASE Product product with which SQL is associated will expire within 30 days.                                   
    WARNING    WARNING: The data set WORK.U0505AA2 may be incomplete.  When this step was stopped there                                     
    WARNING    WARNING: The data set WORK.U0505AA1 may be incomplete.  When this step was stopped there                                     
    WARNING    WARNING: The BASE Product product with which SUMMARY is associated will expire within 30                                     
    WARNING    WARNING: The BASE Product product with which SORT is associated will expire within 30                                        
    WARNING    WARNING: The BASE Product product with which PRINTTO is associated will expire within 30 days. Please contact your SAS       
    WARNING    WARNING: The BASE Product product with which PRINT is associated will expire within 30 days. Please contact your SAS installa
    WARNING    WARNING: The BASE Product product with which DATASTEP is associated will expire within 30                                    
    WARNING    WARNING: RUN statement ignored due to previous errors. Type QUIT; to terminate the                                           
    WARNING    WARNING: Apparent symbolic reference UPDTE not resolved.                                                                     
    WARNING    WARNING: Apparent symbolic reference UCDTE not resolved.                                                                     
    WARNING    WARNING: Variable PRE_YTD not found in data set WORK.U0505AA7.                                                               
    ----------------------------------------------------------------------------------------------------------------------                  
    NOTES      NOTE: No observations in data set WORK.U0505AA2.                                                                             
    NOTES      NOTE: No observations in data set WORK.U0505AA1.                                                                             
    NOTES      NOTE: Library UOT does not exist.                                                                                            
    NOTES      NOTE: Numeric values have been converted to character values at the places given by:                                         
    NOTES      NOTE: Library UIN6 does not exist.                                                                                           
    NOTES      NOTE: Library UIN22 does not exist.                                                                                          
    NOTES      NOTE: Library UIN21 does not exist.                                                                                          
    NOTES      NOTE: Library UIN12 does not exist.                                                                                          
    NOTES      NOTE: Library UIN11 does not exist.                                                                                          
    NOTES      NOTE: Library LIBRARY does not exist.                                                                                        
    NOTES      NOTE: The data set WORK.U0505AA7 has 0 observations and 0 variables.                                                         
    NOTES      NOTE: The data set WORK.U0505AA4 has 0 observations and 3 variables.                                                         
    NOTES      NOTE: The data set WORK.U0505AA3 has 0 observations and 2 variables.                                                         
    NOTES      NOTE: The SAS System stopped processing this step because of errors.                                                         
    NOTES      NOTE: SAS set option OBS=0 and will continue to check statements.                                                            
    ----------------------------------------------------------------------------------------------------------------------                  
    DATASETS   NOTE: The data set SD1.CARS has 428 observations and 15 variables.                                                           
    DATASETS   NOTE: The data set SD1.CLASS has 19 observations and 5 variables.                                                            
    ----------------------------------------------------------------------------------------------------------------------                  
    FILE_IO    MPRINT(U0505AA):   LIBNAME UOT "/xxxxxxxx/daily/tmp";                                                                        
    FILE_IO    MPRINT(U0505AA):   LIBNAME UIN6 "/xxxxxxxx/monthly/199607/u06" ;                                                             
    FILE_IO    MPRINT(U0505AA):   LIBNAME UIN22 "/xxxxxxxx/monthly/199606/u10";                                                             
    FILE_IO    MPRINT(U0505AA):   LIBNAME UIN21 "/xxxxxxxx/monthly/199606/u09";                                                             
    FILE_IO    MPRINT(U0505AA):   LIBNAME UIN12 "/xxxxxxxx/monthly/199607/u10";                                                             
    FILE_IO    MPRINT(U0505AA):   LIBNAME UIN11 "/xxxxxxxx/monthly/199607/u09";                                                             
    FILE_IO    MPRINT(U0505AA):   LIBNAME LIBRARY "/xxxxxxxx/yearly/199607/library";                                                        
    FILE_IO    99          libname  uot     "&uot";                                                                                         
    FILE_IO    97          libname  uin22   "&uin22";                                                                                       
    FILE_IO    96          libname  uin21   "&uin21";                                                                                       
    FILE_IO    94          libname  uin12   "&uin12";                                                                                       
    FILE_IO    93          libname  uin11   "&uin11";                                                                                       
    FILE_IO    91          libname  uin6    "&uin6" ;                                                                                       
    FILE_IO    89          libname  library "&ulibr";   /* get mkt list */                                                                  
    FILE_IO    837   libname sd1 "d:/sd1";                                                                                                  
                                                                                                                                            
    *                                                                                                                                       
     _ __  _ __ ___   ___ ___  ___ ___                                                                                                      
    | '_ \| '__/ _ \ / __/ _ \/ __/ __|                                                                                                     
    | |_) | | | (_) | (_|  __/\__ \__ \                                                                                                     
    | .__/|_|  \___/ \___\___||___/___/                                                                                                     
    |_|                                                                                                                                     
    ;                                                                                                                                       
                                                                                                                                            
                                                                                                                                            
    /*=====================================================================================*                                                
    Program Language    :  SAS V9.1.3  or later                                                                                             
    Operating System    :  Win 10 64 bit                                                                                                    
    ________________________________________________________________________________________                                                
                                                                                                                                            
    You need the Classic 1980s SAS Editor for this log check.                                                                               
                                                                                                                                            
    This will not work in the less functional EE, EG, SAS Studio, University edition....                                                    
                                                                                                                                            
    The problem is that the log summary appears immediately in a pop-up second interative editior window.                                   
    This is nice because you get an immediate summary without any mouse surfing.                                                            
                                                                                                                                            
    The summary is saved to the output location. But the interactive result                                                                 
    is save in the output location                                                                                                          
                                                                                                                                            
                                                                                                                                            
    Purpose             : Check log                                                                                                         
                                                                                                                                            
    Run Dependencies    : Requires interactive SAS connect windows or unix sessions                                                         
                                                                                                                                            
    Sample call         : %utl_logcurchk(d:/log/sample.log,d:/log/sampleChk.txt)                                                            
                                                                                                                                            
    Macro Calls                                                                                                                             
                                                                                                                                            
      Internal          : utl_logcurchk utlfkil                                                                                             
      External          : None                                                                                                              
                                                                                                                                            
    Files                                                                                                                                   
                                                                                                                                            
      Input             : d:/log/sample.log                                                                                                 
                                                                                                                                            
      Output            : d:/txt/sample.txt                                                                                                 
                                                                                                                                            
    Program Flow        :                                                                                                                   
                                                                                                                                            
         1.             Read log for time of run                                                                                            
         2.             Read log and check for error, note, warning, chop lines, perm sas datasets and fileI/O                              
         3.             Execute check                                                                                                       
         3.             Post log, lst and summary of errors and check output back to interactive session                                    
                                                                                                                                            
    Macro Assumptions   :                                                                                                                   
    Macro Parameters    :                                                                                                                   
    ========================================================================================*/                                              
                                                                                                                                            
    %macro utl_logcurchk(loginp,logout);                                                                                                    
                                                                                                                                            
        /* %let logout = d:/log/sample.txt;  */                                                                                             
        /* %let loginp = d:/log/sample.log;  */                                                                                             
                                                                                                                                            
        %utlfkil(&logout);                                                                                                                  
                                                                                                                                            
        %macro ary;                                                                                                                         
         Array Notes{328} $64 (                                                                                                             
             " 0 observations rewritten, 0 observations added and 0 observations deleted"                                                   
             " 0 lines"                                                                                                                     
             " 0 observations"                                                                                                              
             " 0 records"                                                                                                                   
             " 0 rows"                                                                                                                      
             " 0 obs"                                                                                                                       
             "%to value of"                                                                                                                 
             "traceback"                                                                                                                    
             "not currently in"                                                                                                             
             "abnormally terminated"                                                                                                        
             "access denied"                                                                                                                
             "allowed"                                                                                                                      
             "already been defined"                                                                                                         
             "ambiguous"                                                                                                                    
             "apparent invocation"                                                                                                          
             "apparent symbolic"                                                                                                            
             "appears as text"                                                                                                              
             "are not allowed"                                                                                                              
             "argument 1"                                                                                                                   
             "argument 2"                                                                                                                   
             "argument 3"                                                                                                                   
             "assumed"                                                                                                                      
             "assuming"                                                                                                                     
             "at least"                                                                                                                     
             "but appears on"                                                                                                               
             "but is not"                                                                                                                   
             "but no"                                                                                                                       
             "by-group"                                                                                                                     
             "cannot be accessed"                                                                                                           
             "cannot be deleted"                                                                                                            
             "cannot be found"                                                                                                              
             "cannot be loaded"                                                                                                             
             "cannot be"                                                                                                                    
             "cannot open"                                                                                                                  
             "cartesian"                                                                                                                    
             "central parameter"                                                                                                            
             "character in one"                                                                                                             
             "clause has been augmented"                                                                                                    
             "clause references"                                                                                                            
             "cli error"                                                                                                                    
             "closing"                                                                                                                      
             "columns were too wide"                                                                                                        
             "condition in the"                                                                                                             
             "conflicting attributes"                                                                                                       
             "contain no data in common"                                                                                                    
             "contain unequal"                                                                                                              
             "contains 1 variable"                                                                                                          
             "convert"                                                                                                                      
             "converted to"                                                                                                                 
             "converted"                                                                                                                    
             "could not be fit"                                                                                                             
             "could not be found"                                                                                                           
             "could not be loaded"                                                                                                          
             "could not be written"                                                                                                         
             "could not be"                                                                                                                 
             "could not"                                                                                                                    
             "creates a common"                                                                                                             
             "default estimation"                                                                                                           
             "default style will be used instead"                                                                                           
             "defined as both"                                                                                                              
             "did not satisfy"                                                                                                              
             "differ"                                                                                                                       
             "different data types"                                                                                                         
             "division by zero"                                                                                                             
             "denied"                                                                                                                       
             "does not exist"                                                                                                               
             "does not have enough arguments"                                                                                               
             "does not match"                                                                                                               
             "doesn't appear"                                                                                                               
             "doesn't have"                                                                                                                 
             "double-dash"                                                                                                                  
             "due to a"                                                                                                                     
             "due to errors"                                                                                                                
             "due to looping"                                                                                                               
             "dummy macro"                                                                                                                  
             "ellipsoid centered"                                                                                                           
             "end of macro"                                                                                                                 
             "end-of-record"                                                                                                                
             "ending execution"                                                                                                             
             "enter run"                                                                                                                    
             "error"                                                                                                                        
             "errorabend"                                                                                                                   
             "errorcheck=strict"                                                                                                            
             "errors noted"                                                                                                                 
             "estimated autoregression parameter"                                                                                           
             "examine fields"                                                                                                               
             "exceed"                                                                                                                       
             "exceeds 8 characters"                                                                                                         
             "execution terminated"                                                                                                         
             "execution terminating"                                                                                                        
             "expected"                                                                                                                     
             "expecting"                                                                                                                    
             "experimental release"                                                                                                         
             "export cancelled"                                                                                                             
             "expression has no"                                                                                                            
             "extraneous information"                                                                                                       
             "extraneous"                                                                                                                   
             "failed to converge"                                                                                                           
             "failed to load"                                                                                                               
             "failed to"                                                                                                                    
             "fatal"                                                                                                                        
             "firstobs option >"                                                                                                            
             "firstobs option"                                                                                                              
             "generic critical"                                                                                                             
             "groups are not created"                                                                                                       
             "hanging"                                                                                                                      
             "has 0 observations"                                                                                                           
             "has _type_"                                                                                                                   
             "has a null"                                                                                                                   
             "has already been defined"                                                                                                     
             "has already been set"                                                                                                         
             "has already been"                                                                                                             
             "has already"                                                                                                                  
             "has become more"                                                                                                              
             "has been reduced"                                                                                                             
             "has been transformed"                                                                                                         
             "has been discarded"                                                                                                           
             "has changed"                                                                                                                  
             "has different lengths"                                                                                                        
             "has exceeded"                                                                                                                 
             "has multiple"                                                                                                                 
             "has never been"                                                                                                               
             "has no condition"                                                                                                             
             "has not been dropped"                                                                                                         
             "has not been"                                                                                                                 
             "has too few"                                                                                                                  
             "have been detected"                                                                                                           
             "ignored"                                                                                                                      
             "ignoring"                                                                                                                     
             "illegal"                                                                                                                      
             "included in the"                                                                                                              
             "incomplete"                                                                                                                   
             "incorrect"                                                                                                                    
             "input data set is empty"                                                                                                      
             "input distances have been squared"                                                                                            
             "input data set is already sorted"                                                                                             
             "input empty"                                                                                                                  
             "insufficient"                                                                                                                 
             "invalid"                                                                                                                      
             "is already on the"                                                                                                            
             "is already sorted"                                                                                                            
             "is also a dataset"                                                                                                            
             "is ambiguous"                                                                                                                 
             "is before the starting"                                                                                                       
             "is included"                                                                                                                  
             "is invalid"                                                                                                                   
             "is less than or equal"                                                                                                        
             "is less than"                                                                                                                 
             "is not a valid"                                                                                                               
             "is not allowed"                                                                                                               
             "is not assigned"                                                                                                              
             "is not greater than"                                                                                                          
             "is not in effect"                                                                                                             
             "is not in"                                                                                                                    
             "is not on file"                                                                                                               
             "is not recognized"                                                                                                            
             "is not sorted"                                                                                                                
             "is not valid"                                                                                                                 
             "is obsolete"                                                                                                                  
             "is sequential"                                                                                                                
             "it is used out"                                                                                                               
             "is obsolete"                                                                                                                  
             "labels differ"                                                                                                                
             "length of numeric"                                                                                                            
             "limit set by"                                                                                                                 
             "list empty"                                                                                                                   
             "lost card"                                                                                                                    
             "mathemat"                                                                                                                     
             "mathematical operations"                                                                                                      
             "may be incomplete"                                                                                                            
             "may be longer"                                                                                                                
             "may not be as expected"                                                                                                       
             "merge statement has more than"                                                                                                
             "merge statement"                                                                                                              
             "missing close parentheses"                                                                                                    
             "missing equals sign"                                                                                                          
             "missing on every"                                                                                                             
             "missing semicolon"                                                                                                            
             "missing values"                                                                                                               
             "missing"                                                                                                                      
             "misspelled"                                                                                                                   
             "mixed engine types"                                                                                                           
             "model contains"                                                                                                               
             "more positional"                                                                                                              
             "multiple lengths"                                                                                                             
             "multiple optimal"                                                                                                             
             "multiple vertical"                                                                                                            
             "multiple"                                                                                                                     
             "must be character"                                                                                                            
             "must be entered"                                                                                                              
             "must be followed"                                                                                                             
             "must be given"                                                                                                                
             "must be invoked"                                                                                                              
             "must have appeared"                                                                                                           
             "must precede"                                                                                                                 
             "no body file"                                                                                                                 
             "no body"                                                                                                                      
             "no by"                                                                                                                        
             "no cards"                                                                                                                     
             "no data set"                                                                                                                  
             "no data sets qualify"                                                                                                         
             "no data"                                                                                                                      
             "no effect"                                                                                                                    
             "no expression"                                                                                                                
             "no file"                                                                                                                      
             "no formats found"                                                                                                             
             "no keep"                                                                                                                      
             "no libraries"                                                                                                                 
             "suppress"                                                                                                                     
             "no logical"                                                                                                                   
             "no longer exists"                                                                                                             
             "no matching"                                                                                                                  
             "no non-missing"                                                                                                               
             "no observations"                                                                                                              
             "no output destinations active"                                                                                                
             "no output produced"                                                                                                           
             "no output"                                                                                                                    
             "no rows were selected"                                                                                                        
             "no rows"                                                                                                                      
             "no shape"                                                                                                                     
             "no variables found"                                                                                                           
             "no variables specified"                                                                                                       
             "no variables"                                                                                                                 
             "none of the options"                                                                                                          
             "not a valid"                                                                                                                  
             "not acceptable"                                                                                                               
             "not adjusted"                                                                                                                 
             "not all"                                                                                                                      
             "not allow character"                                                                                                          
             "not be included"                                                                                                              
             "not be performed"                                                                                                             
             "not currently licensed"                                                                                                       
             "not found"                                                                                                                    
             "not in a valid"                                                                                                               
             "not in effect"                                                                                                                
             "not licensed"                                                                                                                 
             "not on input data set"                                                                                                        
             "not processed"                                                                                                                
             "not recognized"                                                                                                               
             "not replaced because"                                                                                                         
             "not resolved"                                                                                                                 
             "not valid for import"                                                                                                         
             "not valid"                                                                                                                    
             "not written"                                                                                                                  
             "null where"                                                                                                                   
             "numeric in one"                                                                                                               
             "obs=0"                                                                                                                        
             "observations not"                                                                                                             
             "obsolete"                                                                                                                     
             " omitted due to"                                                                                                              
             "occurred on module"                                                                                                           
             "offline"                                                                                                                      
             "one or more lines may be longer"                                                                                              
             "operand was found in"                                                                                                         
             "option value"                                                                                                                 
             "outside the axis"                                                                                                             
             "parenthesis for"                                                                                                              
             "previous errors"                                                                                                              
             "proc sql statements are executed immediately"                                                                                 
             "product not found"                                                                                                            
             "product with which"                                                                                                           
             "partial initialization"                                                                                                       
             "quoted string"                                                                                                                
             "recursion"                                                                                                                    
             "recursive"                                                                                                                    
             "reference"                                                                                                                    
             "references the data set being updated"                                                                                        
             "refers to the same"                                                                                                           
             "refers to"                                                                                                                    
             "repeat"                                                                                                                       
             "request ignored"                                                                                                              
             "required operator not found"                                                                                                  
             "requires a numeric"                                                                                                           
             "requires compatible"                                                                                                          
             "right-hand"                                                                                                                   
             "sas set option obs=0"                                                                                                         
             "sas went"                                                                                                                     
             "scale parameter was held fixed"                                                                                               
             "shifted"                                                                                                                      
             "starting variable"                                                                                                            
             "statement has been deleted"                                                                                                   
             "statement needs"                                                                                                              
             "statement syntax"                                                                                                             
             "statement transforms"                                                                                                         
             "statistics are mean corrected"                                                                                                
             "statistics requested"                                                                                                         
             "stop"                                                                                                                         
             "stopped"                                                                                                                      
             "subroutine"                                                                                                                   
             "syntax for this"                                                                                                              
             "the chi-square is small"                                                                                                      
             "too long"                                                                                                                     
             "too many array subscripts"                                                                                                    
             "too small"                                                                                                                    
             "too wide"                                                                                                                     
             "trying to use"                                                                                                                
             "unable to initialize"                                                                                                         
             "unable to"                                                                                                                    
             "unable"                                                                                                                       
             "unbalanced"                                                                                                                   
             "unclosed"                                                                                                                     
             "undeclared"                                                                                                                   
             "undetermined"                                                                                                                 
             "uninitialized"                                                                                                                
             "unknown"                                                                                                                      
             "unrecognized"                                                                                                                 
             "unref"                                                                                                                        
             "unresolved"                                                                                                                   
             "unsatisfied"                                                                                                                  
             "violation"                                                                                                                    
             "was disabled"                                                                                                                 
             "was stopped"                                                                                                                  
             "was misspelled as"                                                                                                            
             "was not created"                                                                                                              
             "was not defined"                                                                                                              
             "was not found"                                                                                                                
             "was not replaced"                                                                                                             
             "went to a new line"                                                                                                           
             "were excluded"                                                                                                                
             "will be assumed"                                                                                                              
             "will be used"                                                                                                                 
             "will not be"                                                                                                                  
             "will not load"                                                                                                                
             "will stop executing"                                                                                                          
             "within the range"                                                                                                             
             "you can only"                                                                                                                 
             "your request"                                                                                                                 
             "zero elements" );                                                                                                             
           %mend ary;                                                                                                                       
                                                                                                                                            
           proc datasets library=work kill nolist;run;quit;                                                                                 
           %sysfunc(ifc(%sysfunc(fexist(&logout)),%sysfunc(fdelete(kqzt)),%str( )));                                                        
           run;quit;                                                                                                                        
                                                                                                                                            
           filename kqzt "&logout";                                                                                                         
                                                                                                                                            
           Data Q_A(keep=question answer);                                                                                                  
            Length Question $16 Answer $255 infile $255;                                                                                    
            /*---------------------------------------------*\                                                                               
            |  Read Log and Count Errors and Warnings       |                                                                               
            \*---------------------------------------------*/                                                                               
            infile "&loginp" length=ll end=done;                                                                                            
              input;                                                                                                                        
              If _n_=1 then do;                                                                                                             
                 Question='FULL_PATH';                                                                                                      
                 Answer="&loginp";                                                                                                          
                 output;                                                                                                                    
                 Question="LOG_TIME";                                                                                                       
                 Answer=substr(compbl(_infile_),17);                                                                                        
                 Output;                                                                                                                    
                 Question="SCRUB_TIME";                                                                                                     
                 dte=datepart(datetime());                                                                                                  
                 wek=put(dte,weekdate.);                                                                                                    
                 tym=put(timepart(datetime()),time5.);                                                                                      
                 answer=catx(' ',tym,wek);                                                                                                  
                 Output;                                                                                                                    
              end;                                                                                                                          
             /*---------------------------------------------*\                                                                              
             |  Input and Output files                       |                                                                              
             \*---------------------------------------------*/                                                                              
              answer=_infile_;                                                                                                              
              infile=lowcase(left(_infile_));                                                                                               
              if index(infile,'were written to file' ) gt 0  or                                                                             
                 index(infile,'written to'           ) gt 0  or                                                                             
                 index(infile,'lines written to file') gt 0  or                                                                             
                 index(infile,'file name='           ) gt 0  or                                                                             
                 index(infile,'libname'              ) gt 0  or                                                                             
                 index(infile,'filename'             ) gt 0  or                                                                             
                 index(infile,'physical file'        ) gt 0  or                                                                             
                 index(infile,'file:'                ) gt 0  then do;question="FILE_IO";output;end;                                         
                  /*---------------------------------------------*\                                                                         
                  |  Errors Warnings Notes and Chop               |                                                                         
                  \*---------------------------------------------*/                                                                         
                 Select;                                                                                                                    
                     When (substr(left(infile),1,5) ='error'                                                                                
                           or index(infile,'error:')>0)       Do; question="%str(ERR)OR";answer=_infile_; Output; End;                      
                     When (substr(left(infile),1,4)='note')   Do;                                                                           
                          %ary;                                                                                                             
                          question="NOTES";                                                                                                 
                          Do i=1 to dim(Notes) ;                                                                                            
                            if index(strip(infile),trim(Notes{i})) > 0 then output;                                                         
                          End;                                                                                                              
                     End;                                                                                                                   
                     When (substr(left(infile),1,7)='warning')                    Do;question="WARNING";output;end;                         
                     When (index(infile,'warning')>0 or index(infile,'error')>0)  Do;question="CHOP";output;end;                            
                     Otherwise;                                                                                                             
                 end;                                                                                                                       
                  /*---------------------------------------------*\                                                                         
                  |  Examine Permanent SAS Tables                 |                                                                         
                  \*---------------------------------------------*/                                                                         
                                                                                                                                            
                 if substr(left(infile),1,4)='note' then do;                                                                                
                     question="DATASETS";                                                                                                   
                     select;                                                                                                                
                       when (substr(infile,7,5)  eq 'table' and substr(infile,13,4) ne 'work') output;                                      
                       when (substr(infile,7,12) eq 'the data set' and substr(left(substr(infile,20,5)),1,4) ne 'work') output;             
                       otherwise ;                                                                                                          
                     end;                                                                                                                   
                 end;                                                                                                                       
         run;                                                                                                                               
                                                                                                                                            
        proc format;                                                                                                                        
         invalue que2odr                                                                                                                    
         'FULL_PATH'  = -30                                                                                                                 
         'LOG_TIME'   = -20                                                                                                                 
         'SCRUB_TIME' = -10                                                                                                                 
         "%str(ERR)OR"= 4                                                                                                                   
         'WARNING'    = 5                                                                                                                   
         'NOTES'      = 6                                                                                                                   
         'DATASETS'   = 7                                                                                                                   
         'FILE_IO'    = 9                                                                                                                   
         'OPTIONS'    = 8;                                                                                                                  
        run;quit;                                                                                                                           
                                                                                                                                            
        data shl;                                                                                                                           
          length question $16 answer $255;                                                                                                  
          question='FULL_PATH'  ;answer='remove';output;                                                                                    
          question='LOG_TIME'   ;answer='remove';output;                                                                                    
          question='SCRUB_TIME' ;answer='remove';output;                                                                                    
          question="%str(ERR)OR";answer='remove';output;                                                                                    
          question='WARNING'    ;answer='remove';output;                                                                                    
          question='NOTES'      ;answer='remove';output;                                                                                    
          question='DATASETS'   ;answer='remove';output;                                                                                    
          question='FILE_IO'    ;answer='remove';output;                                                                                    
          question='OPTIONS'    ;answer='remove';output;                                                                                    
        run;                                                                                                                                
                                                                                                                                            
        proc sql;                                                                                                                           
          create                                                                                                                            
             table shlful as                                                                                                                
          select                                                                                                                            
             distinct                                                                                                                       
              coalesce(r.question,l.question) as question length=16                                                                         
             ,coalesce(r.answer,l.answer)     as answer   length=255                                                                        
             ,case when r.answer='' then 0 else 1 end as flg                                                                                
          from                                                                                                                              
              shl as l left join q_a(where=(                                                                                                
               not ( lowcase(answer) contains ("is in a format native")                    or                                               
                     lowcase(answer) contains ('note: multiple concurrent threads')        or                                               
                     lowcase(answer) contains ('refers to the same physical')              or                                               
                     lowcase(answer) contains ("data file is being copied to base file")   or                                               
                     lowcase(answer) contains ('created, with 0 rows and')                 or                                               
                     lowcase(answer) contains ('warn    =')                                                                                 
                   ))) as r                                                                                                                 
          on                                                                                                                                
              l.question=r.question                                                                                                         
        ;                                                                                                                                   
        quit;                                                                                                                               
                                                                                                                                            
        proc sql;                                                                                                                           
          create                                                                                                                            
             table typodr(where=(not (answer='remove'))) as                                                                                 
          select                                                                                                                            
            input(question,que2odr.)-8  as odr                                                                                              
            ,question                                                                                                                       
            ,put(sum(flg),4. -l) as answer                                                                                                  
          from                                                                                                                              
             shlful                                                                                                                         
          where                                                                                                                             
             question not in ('FULL_PATH' 'LOG_TIME' 'SCRUB_TIME')                                                                          
          group                                                                                                                             
             by calculated odr, question                                                                                                    
          outer union corr                                                                                                                  
          select                                                                                                                            
            input(question,que2odr.)  as odr                                                                                                
            ,question                                                                                                                       
            ,left(answer) as answer                                                                                                         
          from                                                                                                                              
             shlful                                                                                                                         
          order                                                                                                                             
             by odr, question;                                                                                                              
        quit;                                                                                                                               
                                                                                                                                            
                                                                                                                                            
        data _null_;                                                                                                                        
                                                                                                                                            
         file "&logout";                                                                                                                    
                                                                                                                                            
         retain str '----------------------------------------------------------------------------------------------------------------------'
         set typodr;                                                                                                                        
                                                                                                                                            
         by question notsorted;                                                                                                             
                                                                                                                                            
         answer=left(answer);                                                                                                               
         if _n_=1 then put str;                                                                                                             
         if odr>1 and first.question then put str;                                                                                          
         put question  @12 answer;                                                                                                          
                                                                                                                                            
        run;                                                                                                                                
                                                                                                                                            
        /* return results to interactive sas session */                                                                                     
        run;quit;                                                                                                                           
                                                                                                                                            
        dm "home;note h.h; clear ; inc '&loginp'";                                                                                          
        run;quit;                                                                                                                           
                                                                                                                                            
        dm "home;note i.i; clear ; inc '&logout'";                                                                                          
        run;quit;                                                                                                                           
                                                                                                                                            
        dm "home";                                                                                                                          
                                                                                                                                            
    %mend utl_logcurchk;                                                                                                                    
                                                                                                                                            
    %utl_logcurchk(loginp=d:/log/sample.log,logout=d:/log/sample.txt);                                                                      
                                                                                                                                            
                                                                                                                                            
