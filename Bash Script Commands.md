### Bash Script Commands

____

Get number of arguments & argument contents:

```bash
num = $#
arg1 = ${1}
arg2 = ${2} #...
```

Limit program running time:

```bash
timeout 20s [command]
```

Get program running time: 

```bash
start_time="$(date -u +%s)"
end_time="$(date -u +%s)"
elapsed="$(($end_time - $start_time))" #(gives time in sec)
```

Sleep for x second

```bash
sleep x
```

Write text to file

```bash
echo "text" > file.txt #(overwrite)
echo "text" >> file.txt #(append)
```

Declare an array

```bash
array=(50 100 500 1000 5000)
${array[i]}
for content in ${array[@]}; do
done # @: loops through all elements contained in array
```

