# LoopForFastqc


  For file in /DIRECTORY OF SOURCE/*.FASTQ.GZ

  do

  fastqc -f fastq -o /PATH TO OUTPUT FOLDER/ -t 4 ${file}

  done



#example in uppmax

  for file in /domus/h1/mahnaz/downloads/*.fastq.gz    #It will choose every file with .fastq.gz suffix in the mentioned directory

  do

  fastqc -f fastq -o /domus/h1/mahnaz/FaastqResults/ -t 4 ${file} #execute fastqc for all .fastq.gz files and save them with the format fastq (-f fastq). The format could be ignored. 

  done
