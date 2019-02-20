# plugin-put-aside
Prod is the latest version
https://cdn.jsdelivr.net/npm/switlish-plugin-put-aside/xxx.js

To create a new version, it is not done in github. Github is only for storing.

How to push a new version ?
1/ git clone https://github.com/switlishswitee/plugin-put-aside.git
2/ vim package.json -> version : X.X.X
2.5/ + modif version in (homol_)switlish_widget.min.js to have fix version to avoid crop code with latest
3/ npm publish
It will throw an error if you try to override a previous version
4/ git add .
5/ git commit -m "X.X.X"
6/ git push origin master

What latest is pointing at if I push 1.0.7 then 1.0.6 ?
It will point to 1.0.6 because it is the last one pushed

Latest can take up to 24h to update

jsDelivr has an easy to use API to purge files from the cache and force the files to update. This is useful when you release a new version and want to force the update of all version aliased users.
To avoid abuse, access to purge is given after an email request (for now - dak@prospectone.io).

Soon an purge caching will be available.

source: https://github.com/jsdelivr/jsdelivr/issues/18063
source: https://github.com/jsdelivr/jsdelivr#purge-cache
source 20180619 - https://github.com/jsdelivr/www.jsdelivr.com/issues/179

Not to do:
Do not fuse switlish_widget with switlish_tracking because extension only use switlish_widget