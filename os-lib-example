import os
from datetime import datetime

#--Check os useful functions
print(dir(os))

#--Get current directory
print(os.getcwd())

#--Chnage directory
os.chdir('E:\PythonProject')
print(os.getcwd())

#--List the files in curreent direcotry
print(os.listdir())

#--Make directory Single
os.mkdir("os")
print(os.listdir())


#--Make directories multileven
os.makedirs('os/os1/os2')
print(os.listdir())


#--Remove direcotry
os.rmdir('os/os1/os2')

#--Remove directories
os.removedirs('os/os1')
print(os.listdir())


#--Rename file
os.rename("test.txt","demo.txt")
print(os.listdir())


#--Information about files
print(os.stat("quickstart.py"))
#---Size of file
print(os.stat("quickstart.py").st_size)
#---Modified time of file
mod_time = os.stat("quickstart.py").st_mtime
print(datetime.fromtimestamp(mod_time))


#-- Traversing throught files and folders
for dirpath, dirnames, filenames in os.walk(os.getcwd()):
    print('Current Path:', dirpath)
    print('Directories:', dirnames)
    print('Files:', filenames)
    print()

#--Get home directory path envirment directory
print(os.environ.get("HOME"))

#-- Join method is used to join two path
OLD_PATH = os.getcwd()
NEW_PATH = os.path.join(OLD_PATH,"demo1.txt")
print(NEW_PATH)
os.mkdir(NEW_PATH)
print(os.listdir())

#--Get basename of path
print(os.path.basename(os.path.join(os.getcwd(),"demo1.txt")))

#--Get dir name of path
print(os.path.dirname(os.getcwd()))

#--Split method
print(os.path.split(os.path.join(os.getcwd(),"demo1.txt")))


#--Check path is exists or not
print(os.path.exists(os.path.join(os.getcwd(),"demo2.txt")))

#--Check is dir or not
print(os.path.isdir(os.getcwd()))

#--Check is file or not
print(os.path.isfile(os.path.join(os.getcwd(),"demo2.txt")))

#--Split path and extension
print(os.path.splitext(os.path.join(os.getcwd(),"demo2.txt")))
