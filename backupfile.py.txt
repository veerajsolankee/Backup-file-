import os
import shutil
source=input("enter the folder name to be backup ")
destination=input("enter the folder for which you want to copy ")
source=source+'/'
destination=destination+'/'
list=os.listdir(source)
for file in list:
    shutil.copy((source+file),destination)