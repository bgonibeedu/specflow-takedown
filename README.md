specflow-takedown
===================

A clean and cutdown template for writing acceptance tests against API endpoints.

##Setup

Ensure you have installed the Visual Studio integration packages for Specflow as documented here <a href="http://www.specflow.org/getting-started">http://www.specflow.org/getting-started</a>.

##Usage

To run an acceptance test:

* Build solution
* Open desired feature file located within 'Features' folder
* Right click a feature or scenario title
* Click 'Run Specflow Scenarios'

Or even better use the command line to run all the tests:

* Navigate to the root of the specflow-takedown project (cd [file_location]\specflow-takedown\api-acceptance-tests)
* Execute the command line test runner by typing 'runtests.cmd' and hit [Enter]

##Auto generated documentation

Running acceptance tests via the CLI means we can generate some useful reports and documentation.

SpecRun provides a nice reporting structure for your acceptance tests. These reports can be found within the 'TestResults' folder. More information on SpecRun reporting here <a href="http://www.specflow.org/documentation/Reporting/">http://www.specflow.org/documentation/Reporting/</a>.

Pickles is a tool that will output features as human readable documentation. These files are generated within the 'Documentation' folder. More information on Pickles reporting here <a href="http://docs.picklesdoc.com/en/latest/StartSimple/">http://docs.picklesdoc.com/en/latest/StartSimple/</a>

It is recommended that any generated reports should be displayed as artifacts within your automated build process.

##Troubleshooting

The acceptance tests make a GET request to various endpoints within <a href="http://jsonplaceholder.typicode.com">jsonplaceholder.typicode.com<a/>. In case of request timeouts please check your connection to <a href="http://jsonplaceholder.typicode.com">jsonplaceholder.typicode.com<a/>. 

##Credits	

Shout outs to <a href="http://www.specflow.org/">Specflow<a/>, <a href="http://www.specrun.com/">SpecRun<a/>, <a href="https://github.com/shouldly/shouldly">Shouldly<a/> and <a href="https://github.com/hhariri/EasyHttp">EasyHttp<a/>.
