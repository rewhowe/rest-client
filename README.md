# Rest Client

Quick-and-dirty rest client for testing API.

## Install

`sudo ln -s ~/<REPO_DIRECTORY>/rest-client/rest-client /usr/local/bin/rest-client`

## Usage

example:
```
connect to? [local/dev/stg/prod] dev
 connecting to dev
use api? [cpn/ext1/ext2] cpn
 using cpn api
usage: <method> <path>[?<param>[&<param>]...]
save last response: save <filename>
> get http://api.example.jp.local/1.0/hoge/list?page=1&per=1
...
> get http://api.example.jp.local/1.0/hoge/list
? page=1
& per=1
...
> get hoge/list
...
> post hoge/info/1
* {
*   "label":"ほげ",
*   "fuga":3
*   }
...
> save hoge.txt
saved response to hoge.txt
...
```
