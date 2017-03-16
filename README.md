A Python I wrote script that goes over all files in a directory (recursively) and extracts the API for the project.
The goal is to easily find things like undocumented or poorly written APIs and find vulnerabilities in them.
It works only Java Spring applications.


Right now it only extracts the endpoint address, method, params and some more attributes in the @RequestMapping annotation.
In the future I’m planning to add some brains to it so it can help identify problems easier.

Usage:

python RequestMapper.py -p "root of project" -o "output file"

example:
python RequestMapper.py -p "C:\Pentests\UAA\" -o "C:\UAA.txt"

