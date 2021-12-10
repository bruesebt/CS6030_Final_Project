Summarizer for User Reviews Feedback
Version 1.0

This program is a free software you can redistribute it under the terms of the GNU Public License
as published by the Free Software Fundation either version 2 of the License, or (at your option)
any later version.

Please extract the contents of SURF_tool.zip file in a folder of your choice

The tool uses the following open source libraries: 
- version 3.4.1 of the Stanford CoreNLP library available at the following link: http://nlp.stanford.edu/software/corenlp.shtml
- version 3.6 of the Weka library available at the following link: http://sourceforge.net/projects/weka/files/?source=navbar
- version 0.6 of the Classifier4J library available at the following link: http://http://classifier4j.sourceforge.net/

You can find the needed jar files for running the tool in the /lib folder contained in the SURF_tool.zip file

Please add these jars and SURF.jar to the java classpath and run the org.surf.Main class.

SURF is a command-line tool which automatically extracts (and classifies) 
user feedbacks from app reviews that are useful for software maintenance/evolution.
SURF generates html summaries of user reviews in which useful feedbacks for
developers are reported in the form of interactive, structured and 
condensed agendas of future change tasks.

The tool accepts in input xml files having the structure showed
in the following example:

<reviews>
   <review>
      <date>2012-01-28</date>
      <star_rating>4</star_rating>
      <user>Filigio</user>
      <app_version>1.50</app_version>
      <review_title>Walkin'by</review_title>
      <review_text>Great game to sharpen any age level's memory skills.</review_text>
   </review>
   <review>
      <date>2012-01-17</date>
      <star_rating>1</star_rating>
      <user>Teacher K-12 Gifted</user>
      <app_version>1.50</app_version>
      <review_title>Distracting ads</review_title>
      <review_text>Used to be an excellent game, but ads ruin the free version .</review_text>
   </review>
   ....
</reviews>


Here we provide a running example from command Line:

Running example for Windows systems:
java -classpath "[MYPATH]/lib/*;[MYPATH]/SURF.jar" org.surf.Main inputFile.xml outputFile.html

Running example for Unix/Linux/MacOS systems:
java -classpath "[MYPATH]/lib/*:[MYPATH]/SURF.jar" org.surf.Main inputFile.xml outputFile.html


where:
  - [MYPATH] is the path in which the contents of the zipped file has been extracted.  
  - inputFile.xml is the input file containing all the user
    reviews data the tool has to analyze
  - outputFile.html is the file which will contain the
    tool outputs.
 
