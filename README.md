# Basic-JMeter-Performance-Testing
Basic performance testing learning using JMeter tool

Basics steps:

Run JMeter (in GUI mode by default)
  Run jmeter.bat script in the bin, through command line


Run project and Create HTML report
	jmeter -n -t "<bin>/<relativePath>/ResreqRequests.jmx" -l ./<relativePath>/Reports/log_result.csv -e -o ./<relativePath>/Reports -JThreads=50
	
	Note: You need to run your script from bin folder and find your jmx project. If you don't specify your reports path, a new folder will be created
	
	-e, --reportatendofloadtests
        generate report dashboard after load test
	-t, --testfile <argument>
	-l, --logfile <argument>
	-n, --nongui
	-o, --reportoutputfolder <argument>
        output folder for report dashboard
