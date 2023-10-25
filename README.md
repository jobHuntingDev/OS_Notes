# Notes on the os module

## Installing

The os module comes with python so you just import it.

```python
import os

# Show all attributes and methods
python(dir(os))
```

## Using the module:

**Print current directory:**

```python 
import os

current_dir = os.getcwd()

print(current_dir)
```

**Change directory:**

```python
import os

# Changing current directory
os.chdir('/Users/coreyschafer/Desktop/')

print(os.getcwd())
```

**List items in directory**

```python 
import os

# List current directory
print(os.listdir())

# Change directory
os.chdir('/Users/Username/Documents/')

# List current directory
print(os.listdir())
```

**Make folder:**

```python
import os

# Make simple directory
os.mkdir('OS-DEMO-2')

# Make parent and children
os.makedirs('OS-DEMO-3/Sub-Dir-1')

os.listdir()

# Delete a folder
os.rmdir('OS-DEMO-2')

# Delete a folder recurservly
os.removedirs('OS-Demo-3/Sub-Dir-1')
```

**Rename file**

```python
import os

os.rename('test.txt', 'demo.txt')
```

**Print info on file**

```python
import os

print(os.stat('demo.txt')

# Refer to documentation on what each stat is
```

**Print all directories and what's in them:**

```python
import os

for dirpath, dirnames, filenames in os.walk('/Users/coreyschafer/Desktop/'):
    print('Current Path:', dirpath)
    print('Directories:', dirnames)
    print('Files', filenames) 
```

**Print out environment variables:**

```python
import os

# print all my environment variables
print(os.environ)

# print a specific envirnment variables
print(os.environ.get('HOME'))
```

**Working with paths**

```python
import 

# joining two paths
file_path = os.path.join(frist_path, second_path)

# Print out path methods
print(dir(os.path))
```
