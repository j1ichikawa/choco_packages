# choco_packages

chocolatey installed packages

usage:

for export:
`choco export --include-version-numbers`  
`choco export

for import:
`cinst -y packages.config`

variation:

choco export  
choco export --include-version-numbers  
choco export ".\package.config"  
choco export ".\packages.config" --include-version-numbers  
choco export -o=".\package.config"  
choco export -o=".\packages.config" --include-version-numbers  
choco export --output-file-path=".\package.config"  
choco export --output-file-path=".\packages.config" --include-version-numbers  
