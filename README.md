# plugin-put-aside
Prod is the latest version
https://cdn.jsdelivr.net/npm/switlish-plugin-put-aside/xxx.js

To create a new version, it is not done in github. Github is only for storing.

How to push a new version ?
1/ git clone https://github.com/switlishswitee/plugin-put-aside.git
2/ vim package.json -> version : X.X.X
3/ npm publish
It will throw an error if you try to override a previous version
4/ git add .
5/ git commit -m "X.X.X"
6/ git push origin master

What latest is pointing at if I push 1.0.7 then 1.0.6 ?
It will point to 1.0.6 because it is the last one pushed
