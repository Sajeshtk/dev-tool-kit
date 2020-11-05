Summary
-
jq is a lightweight and flexible command-line JSON processor.

https://stedolan.github.io/jq/

Use Cases
- 
Usefull in reading from the logs / text files a well-formed json string and extracting only the needed elements.

Examples
-
```
cat file_name.txt | grep -o '{.*}' | jq -c '. | {extractedAttributeName1 : .inJsonAttributeName1, extractedAttributeName2 : .inJsonAttributeName2, extractedAttributeName3 : .inJsonAttributeName3}'
```
