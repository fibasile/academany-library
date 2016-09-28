## Academany library

Dependencies
- Node.js 4.5.0
- npm install gitbook-cli
- install Calibre from binary at calibre-ebook.org
- add this to .profile

	export PATH=$PATH:/opt/calibre/bin:/root/node-v4.5.0-linux-x64/bin
	export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/opt/calibre/lib

## How to

**Add a new book**:

- clone the repo into a subfolder
- edit deployer.json 
- add the webhook to github http://docs.academany.org:8080/incoming/webhook-deployer
- stop webhook-deployer (killall -9 node)
- start webhook-deployer (webhook-deployer -l logfile -d &)

