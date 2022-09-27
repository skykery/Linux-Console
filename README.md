# Linux-Console
Tips &amp; Tricks

#replace all the blank lines // -i = alias for backup
`sed -i=backup '/^\s*$/d' filename`

# sort by 6nd key from a string as `s:s:s:s:s:key:... /n` and the 7nd key as secondary factor
`sort -t\: -k6,6n -k7,7n oldfile > newfile` 


#replace \n with |
`sed -i=backup ':a;N;$!ba;s/\n/|/g' filename` 
