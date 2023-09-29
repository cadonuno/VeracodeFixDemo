# VeracodeFixDemo

## For latest instructions see: 
https://veracode-my.sharepoint.com/:w:/p/cdalomba/EX7TGt30zhhDurN2tgw1mhYB8hJwVDDkSIZ77lzLYOi1qg?e=sxNhq8

# Quick Demo

# Set aliases
alias veracode="~/veracode"  
alias sast="veracode static scan"  
alias cleardemo="git stash;rm SQLvulnerability.class;rm results.json"  

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
