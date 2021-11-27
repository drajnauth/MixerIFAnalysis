# MixerIFAnalysis
This program analyzes inputs and outputs from a mixer to identify frequencies that could fold back into the passband. The program assumes that an RF frequency is fed into a mixer along with an LO frequency which generates an IF output frequency.  The IF frequency may either be the sum RF+LO or the difference of RF-LO. 
				
Its a work in progress and any 'constructive' feed back regarding its accuracy would be appreciated. I wouldvery much like to make this program accurate as possible. 

Software (c) VE3OOI. All rights reserved and provided 'as is', without warranty or support of any kind;

The program is written in Java and developed using Eclipse. The program requires Java version 8 to be installed (https://www.java.com/en/download/manual.jsp).  You need to understand how to run a Java program using the Java VM.   


Usage:

java -jar FilterAnalyzer.jar

Written by Dave Rajnauth (VE3OOI) and licensed under Creative Commons. No commercial use permitted.  Provided 'as is', without warranty or support of any kind;
