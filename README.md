cws-status
==========

Check the publish status of your extensions on the Google Chrome Web Store from
the command line.

No API presently exists for querying extensions’ publish status. In order to get
this information, the Chrome Web Store developer dashboard is scraped,
authenticating with the cookies from the Google Chrome browser.


## Usage

	$ cws-status \
		--url 'https://chrome.google.com/webstore/devconsole/<UUID>' \
		--cookie-path '~/Library/Application Support/Google/Chrome/Profile 1/Cookies' \
		Example
	Example extension BETA (Version 1.0)        Published to testers
	Example extension (Version 1.0)             Published - public


## Install

	$ git clone https://github.com/teddywing/cws-status.git
	$ cd cws-status
	$ python3 -m venv venv
	$ source ./venv/bin/activate
	$ pip install -r requirements.txt


## License
Copyright © 2022 Teddy Wing. Licensed under the GNU GPLv3+ (see the included
COPYING file).
