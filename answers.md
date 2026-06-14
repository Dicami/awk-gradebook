Task 1
Write a one-line awk program that prints how many submissions are in the file, excluding the header line
@Dicami ➜ /workspaces/awk-gradebook (main) $ awk -F',' 'NR>1 {count++} END {print count}' Lab03-data.csv
322
I used -F',' to set the comma as the field separator. The condition NR>1 skips the header line, incrementing the 'count' variable for each subsequent data row, and finally prints the total accumulation in the END block.
Task 2