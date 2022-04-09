#!/bin/bash git-repo
echo "Enter path"
read path
echo "Enter Filename"
read Filename
if [ find "$path" "$filename"];
then
     echo "file found"
else
     echo "file not found"
fi

