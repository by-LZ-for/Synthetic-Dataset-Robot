# Synthetic-Dataset-Navigation-Ground Robot

Link to dataset for paper ->  "Synthetic dataset for navigation tasks of autonomous systems and ground robots".

Conference -> http://itnt-conf.org/index.php

Will be available ->  20 september 2021

#!/bin/bash

#File: tree-md

tree=$(tree -tf --noreport -I '*~' --charset ascii $1 |
       sed -e 's/| \+/  /g' -e 's/[|`]-\+/ */g' -e 's:\(* \)\(\(.*/\)\([^/]\+\)\):\1[\4](\2):g')

printf "# Project tree\n\n${tree}"
