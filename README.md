# VeracodeFixDemo

# Quick Demo

## Compile

javac -g SQLvulnerability.java

## Run SAST

sast SQLvulnerability.class --results-file results.json

## Run fix

veracode fix SQLvulnerability.java

## Select the SQL Injection (CWE 89) finding

1000

## Recompile

javac -g SQLvulnerability.java

## Run SAST on new class file

sast SQLvulnerability.class --results-file results.json

## Reset the demo (restore the source file)

cleardemo
