# Eliminating-duplicate-rows-from-a-dataset-
### ELIMINATING DUPLICATES ROWS FROM A DATASET ###

dups<-read.table("dups.txt", header = TRUE)
View(dups)

#You can see that row 3 is exactly as row 5 

# To stripp out the duplicate rows, we use the unique function 

newdata<-unique(dups)

View(newdata)

#You can see that the 5th row has been stripped out

dups[duplicated(dups) , ]
