BASH
====


Tips
----

```bash
# import a file
. locallib.sh
source locallib.sh

#set
set -e #exit on error
set -u #exit when a variable is unset
set -x #print out every command it runs before running it
help set

#http://stackoverflow.com/questions/59895/getting-the-source-directory-of-a-bash-script-from-within
DIR="$( cd "$( dirname "${BASH_SOURCE[0]}" )" && pwd )"

#https://stackoverflow.com/questions/5947742/how-to-change-the-output-color-of-echo-in-linux
for (( i = 30; i <= 37; i++ )); 
do echo -e "\e[0;"$i"m  Hi stackoverflow\e[0m"; 
done
```

Links
-----

* http://jvns.ca/blog/2017/03/26/bash-quirks/ (https://twitter.com/b0rk/status/846203979403083776)
