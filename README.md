# awktools

1.Formatting a epoch timestamp to date format in a file in linux systems
  awk -F'\t' '{OFS="\t";$1=strftime("%Y-%m-%d",$1);print}' file1 > file2
  In case of mac
  brew install gawk
  gawk -F'\t' '{OFS="\t";$1=strftime("%Y-%m-%d",$1);print}' file1 > file2 
