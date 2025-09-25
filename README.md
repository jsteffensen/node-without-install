# node-without-install

## Download binaries

Download the binaries from https://nodejs.org/en/download

For Linux download "Linux Binaries (x64)".

For Windows download "Windows Binary (.zip)".

Extract to some folder.

In Linux right click "node" binary executable file (in /bin folder) and select "Make executable" or look in Properties -> Permissions to make it executable.

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

You can also put a shebang inside the js file that points to the binary like:

```
#!/home/jsteffensen/node-v22/bin/node
console.log('Node is awesome');
```
then you can simply run the script from the terminal with ```./myscript``` and it will go pick up the executable binary from the path in the shebang.

You can edit the npm file in the node bin folder to look like:
```
#!/home/secudesk/node-v22/bin/node
require('../lib/cli.js')(process)
```

Then npm will not rely on node being on your path and you can run npm directly in a folder like:

```
~/Desktop/my-node-project$ ../../node-v22/bin/npm init
```
