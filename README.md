twitter_crawler
===============

Code to crawl followers and friends of a list of users

1. Obtain API keys
	1. Register at (http://dev.twitter.com)
	2. Go to (http://dev.twitter.com/apps), click on create a new application
	3. Enter a unique name, description, website and click on _create your Twitter Application_
	4. You'll be redirected to the application page, else go to the page. Click on settings section
	5. In the Application Type, change the access for Read only to Read and Write, and click on "Update this twiter application's settings"
	6. Go to the details section. In Your Access Token, click on _Create my Access Token_. Might take a few minutes to generate an access token
	7. Copy the Consumer key and Consumer Key under the OAuth Settings and Access Token and Access Token Secret to the keys.ini file, to the *C_KEY1*, *C_SECRET1*, *T_KEY1* and *T_SECRET1* respectively
	8. Repeat the procedure for filling the details for the remaining variables in _keys.ini_

2. Go to the folder _python-oauth2-master_ from terminal, run the command: <code>sudo python setup.py install</code>

3. For crawling through the proxy server, update the proxy settings in _proxy.ini_ file

4. Run the command, <code>python crawl.py</code> for non-proxy environment and <code>python crawl_through_proxy.py</code> for proxy environment
