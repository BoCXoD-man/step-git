#! /bin/bash

counter() # takes one argument

{

  local let "c1+=$1"

  let "c2+=${c1}*2"

}

for i in `seq 1 10`

do

  counter ${i}

done

echo "counters are $c1 and $c2" 
