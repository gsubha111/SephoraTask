# SephoraTask

dependency_table() : Function can used to parse the sql scripts and to get the each query dependent tables
please look at the image for reference.

Here i am assigning the sequence number in order to run the scripts in sequence.

For this , first i am considering all the scripts which only using raw.<table_names> and i am assigning the sequence number to them.

Second, i am considing the scripts which using at lease one tmp.<table_name> and i am assigning the number by considering the first list

Ex: in in first list max sequence 5
then for second list starting sequence nymber will be 6

run_sql_in_sequence(): Function can be used to run the scripts in sequence order.

run_sql_in_parallel() : Function can be used to run the scripts in Parallel.
Ex: Scripts which are not dependeing on the /tmp foldercan run parallel
