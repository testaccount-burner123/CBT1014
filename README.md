# CBT1014
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. GitHub repos will be deleted and created during this period...

```
//***FILE1014 is a very interesting piece of code (a REXX exec)     *   FILE1014
//*           written by (the late) Ken Tomiak.  And it has been    *   FILE1014
//*           included here, not only as an honor and a tribute     *   FILE1014
//*           to him, but also because it is useful.  This REXX     *   FILE1014
//*           exec (called CONDCODE) follows job execution and      *   FILE1014
//*           supplies statistics somewhat similar to an IEFACTRT   *   FILE1014
//*           exit, about the results of the job.                   *   FILE1014
//*                                                                 *   FILE1014
//*   Example Usage:                                                *   FILE1014
//*                                                                 *   FILE1014
//*   //*         put this at the end of your job                   *   FILE1014
//*   //CONDCODE EXEC PGM=IKJEFT01                                  *   FILE1014
//*   //SYSPROC  DD   DISP=SHR,DSN=SYS1.U.CLIST   <-- change        *   FILE1014
//*   //SYSTSPRT DD   SYSOUT=*                                      *   FILE1014
//*   //SYSTSIN  DD   *                                             *   FILE1014
//*   CONDCODE                                                      *   FILE1014
//*   /*                                                            *   FILE1014
//*                                                                 *   FILE1014
//*               Sample SYSTSPRT Output for a job                  *   FILE1014
//*   READY                                                         *   FILE1014
//*   CONDCODE                                                      *   FILE1014
//*   JOB=IBMUSERM(JOB00857) JCTACODE=00000000 FAIL=00 STAT=00      *   FILE1014
//*                          LASTABEND=0 HIGHESTCOND=0000           *   FILE1014
//*   Step.ProcStep                  Program    Code                *   FILE1014
//*   S01.TAPEMAP                    TAPEMAP       0                *   FILE1014
//*   S02.TAPEMAP                    TAPEMAP       0                *   FILE1014
//*   S03.TAPEMAP                    TAPEMAP       0                *   FILE1014
//*   READY                                                         *   FILE1014
//*   END                                                           *   FILE1014
//*                                                                 *   FILE1014
//*               Sample TSO Output if run as an EXEC               *   FILE1014
//*                     under your TSO session                      *   FILE1014
//*                                                                 *   FILE1014
//*   JOB=IBMUSER (TSU00849) JCTACODE=00000000 FAIL=00 STAT=00      *   FILE1014
//*                          LASTABEND=0 HIGHESTCOND=000            *   FILE1014
//*   Step.ProcStep                  Program    Code                *   FILE1014
//*   ISPFPROC.ISPFPROC              ADFMDF03  Active               *   FILE1014
//*   ADF041A ENTER A NULL LINE TO RETURN TO FULL SCREEN PROGRAM    *   FILE1014
//*                                                                 *   FILE1014
```
