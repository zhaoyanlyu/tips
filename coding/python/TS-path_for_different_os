# Trouble Shooting: Path Format for Different OS

## Problem statement

We often need use to read path of files in the OS. However, depending on which OS you are using, the format could be different. In particular, the Windows system is especially confusing.

When right licking on the file while holding shift key, we can copy the path of file as a string, which looks like:
```
C:\Users\Folder\File.txt
```

This is very much like the path in Linux/Unix/MacOS system (Linux-like OS):

```
\User\Folder\File.txt
```

Right, in the Linux-like systems, the different hard disks are monted under the root path.

However, when we use pyhon **os** package, things will be different. For example, by

```python
os.path.join(pathA, pathB)
```

For Linus-like OS, the return path will looks like:

```
/pathA/pathB
```

However, under Windows OS, the direction of slash will be inversed, and probably doubled:

```
C:\\pathA\\pathB
```

So you can predict that if we split the paths that been processed by the python **os** package using

```python
String.split('\\')
```

or

```python
String.split('/')
```

will cause some trouble trouble.

## Solution

Use the **pathlib** package to split the paths. e.g.

```Python
from pathlib import PurePath

path_parts = PurePath(full_path).parts
```

Under Windows OS, you will get a tuple like:

```
('C:\\', 'Users', 'Paths', 'File.txt')
```

## One more thing

The **pathlib** has more functions, referring to the [official docs](https://docs.python.org/3.4/library/pathlib.html).
