<br>![images](https://github.com/MichaelMa666/Build-node.js-express-environment/blob/master/images/logo.png)<br>
#Node.js with Express structure
<br>
<a>node -v 4.4.3</a>
##Linux
download node-v4.4.3-linux-x64.tar.xz from Google searching.<br>
<br>upload the package to the directory: **/user/local/**<br>
<br>`cd /usr/local/`<br>
<br>Decompression this package: `tar –xvf node-v4.4.3-linux-x64.tar.xz`<br>
<br>![images](https://github.com/MichaelMa666/Build-node.js-express-environment/blob/master/images/install.png)<br>
<br>Add the node path to environment variables:<br>
<br>`ln -s /usr/local/node-v4.4.3-linux-x64/bin/node /usr/local/bin/node`<br>
<br>`ln -s /usr/local/node-v4.4.3-linux-x64/bin/npm /usr/local/bin/npm`<br>
<br>Then you can test it: `node –v` and `npm –v`<br>
<br>If it shows the version, it means you make it.<br>
<br>![images](https://github.com/MichaelMa666/Build-node.js-express-environment/blob/master/images/install2.png)<br>
##Windows
<br>It is easy to download <a href='http://nodejs.cn/download/'>node.exe</a> or <a href='http://nodejs.cn/download/'>node-v4.4.4-x64.msi</a><br>
<br>Then next and next and install<br>
###Proxy Configuration
<br>![images](https://github.com/MichaelMa666/Build-node.js-express-environment/blob/master/images/proxy_config.PNG)<br>
<br>Open cmd<br>
<br>`npm config set proxy http://serverIP:port`<br>
<br>You can also try<br>
<br>`npm config set https-proxy http://serverIP:port`<br>
<br>If authorization required.<br>
<br>`npm config set proxy http://username:password@serverIP:port`<br>
<br>Or `npm config set https-proxy http://username:password@serverIP:port`<br>
<br>If your proxy dosen't support https, you would modify the address where the package stored.<br>
<br>Do like this: `npm config set registry http://registry.npmjs.org`<strong>(This command fixed my problem!)</strong><br>
