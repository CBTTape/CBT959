# CBT959
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)
This is still a work in progress. GitHub repos will be deleted and created during this period...
~~~~~~~~~~~~~~~~

//***FILE 959 is from Richard W. Pinion and contains a program      *   FILE 959
//*           to release excess space from a list of datasets (by   *   FILE 959
//*           name), without affecting the last-access date.        *   FILE 959
//*           This program uses the PARTREL macro from SYS1.MACLIB. *   FILE 959
//*                                                                 *   FILE 959
//*           email:  RPINION@firsthorizon.com                      *   FILE 959
//*                                                                 *   FILE 959
//*           The UCB lookup in this program uses the ULUT          *   FILE 959
//*           (UCB Lookup Table) method, from CBT File 873, that    *   FILE 959
//*           was pioneered by Gilbert Saint-flour.  Please see     *   FILE 959
//*           member $ULUNOTE for some background on this subject,  *   FILE 959
//*           which is not documented by IBM.  The easy-to-use      *   FILE 959
//*           UCB Lookup Table macros were written by Sam Golob.    *   FILE 959
//*                                                                 *   FILE 959
//*       PARTREL  - RELEASES EXCESS SPACE FROM DATASETS, EITHER    *   FILE 959
//*                  CATALOGED, OR UNCATALOGED (WITH VOLSER).       *   FILE 959
//*                                                                 *   FILE 959
//*       Further documentation:                                    *   FILE 959
//*                                                                 *   FILE 959
//*       The PARTREL program takes input in the //INDD DD name     *   FILE 959
//*       with the dataset name starting in column1, and optionally *   FILE 959
//*       the volser of the dataset, which is necessary if the      *   FILE 959
//*       dataset is uncataloged, starting (for 6 characters)       *   FILE 959
//*       in column 45.                                             *   FILE 959
//*                                                                 *   FILE 959
//*       Model JCL for the //INDD DD card is as follows:           *   FILE 959
//*       Please  make sure that the "ruler" comment card does not  *   FILE 959
//*       immediately follow the //INDD DD card, or a //SYSIN DD *  *   FILE 959
//*       card will be generated, nullifying the //INDD DD * card.  *   FILE 959
//*                                                                 *   FILE 959
//*       //PARTR01  EXEC PGM=PARTREL                               *   FILE 959
//*       //STEPLIB   DD  DSN=SYS1.CBT.LINKLIB,DISP=SHR             *   FILE 959
//*       //SYSPRINT  DD  SYSOUT=*                                  *   FILE 959
//*       //*-+----1----+----2----+----3----+----4----volser        *   FILE 959
//*       //INDD      DD  *                                         *   FILE 959
//*       IBMUSER.TEST.PARTREL.PDS2                   VPWRKD        *   FILE 959
//*       IBMUSER.TEST.PARTREL.PDS                                  *   FILE 959
//*       /*                                                        *   FILE 959
//*       //                                                        *   FILE 959
//*                                                                 *   FILE 959
~~~~~~~~~~~~~~~~

