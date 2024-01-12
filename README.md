# VeracodeFixDemo

# Quick Demo

## Compile

javac -g SQLvulnerability.java

## Run SAST

veracode static scan SQLvulnerability.class

## Run fix

veracode fix SQLvulnerability.java

## Select the SQL Injection (CWE 89) finding

1

## Recompile

javac -g SQLvulnerability.java

## Run SAST on new class file

veracode static scan SQLvulnerability.class

## Reset the demo (restore the source file)

git reset --hard
