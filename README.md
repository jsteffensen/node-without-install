# node-without-install

## Download binaries

Download the binaries from https://nodejs.org/en/download

For Linux download "Linux Binaries (x64)".

For Windows download "Windows Binary (.zip)".

Extract to some folder.

In Linux right click "node" binary executable file (in /bin folder) and select "Make executable".

## Running Node and NPM

Open Terminal in:
/&lt;some folder&gt;/node-v20.11.1-linux-x64/bin/

Since you have not installed Node the ```npm``` command is not on your path.
You can still make Node run the NPM script by using the following command:

To init project (generate a package.json file) run:
```./node npm init```


To install node packages:
```./node npm install```

To run:
```./node index```
