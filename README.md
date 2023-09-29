# VeracodeFixDemo

## For latest instructions see: 
https://veracode-my.sharepoint.com/:w:/p/cdalomba/EX7TGt30zhhDurN2tgw1mhYB8hJwVDDkSIZ77lzLYOi1qg?e=sxNhq8

# Quick Demo

# Set aliases
alias veracode="~/veracode"git
alias sast="veracode static scan"
alias cleardemo="git stash;rm SQLvulnerability.class;rm results.json"

## Compile

javac -g SQLvulnerability.java

## Run SAST

sast SQLvulnerability.class --emit-stack-dump --out results.json

## Run fix

veracode fix SQLvulnerability.java

## Recompile

javac -g SQLvulnerability.java

## Run SAST on new class file

sast SQLvulnerability.class --emit-stack-dump --out results.json

## Reset the demo (restore the source file)

cleardemo
