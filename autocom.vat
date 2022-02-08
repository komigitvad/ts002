 @ECHO OFF
cls
SET comment=Saved on %date%-%time%
IF "%~1"=="" GOTO COMMIT
SET username=%1
SET comment=%comment% by %username%
 
:COMMIT
ECHO %comment%
 
cd C:\_vad\ts4
git checkout dev
git add .
 
git commit -m "%comment%"
git push