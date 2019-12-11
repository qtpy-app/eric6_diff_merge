# eric6_diff_merge
python diff merge module copy from eric6.

### install:
`pip install eric6_diff_merge`

### useage:
```python
from eric6_diff_merge import Eric6Diff

def main():

    diff = Eric6Diff("./speedtext1.txt",
                     "./speedtext2.txt",
                     output="./result.txt")

    diff.on_diff()

if __name__ == "__main__":
    main()
```
### input :
speedtext1.txt
```python

== Capital-Saratoga ==
aaa
bbb
ccc
ddd



```
speedtext2.txt
```python
== Capital-Saratoga ==
abc
bbb
ccc


```

### output : result.txt
```
--- ./speedtext1.txt	Thu Dec 12 03:08:59 2019
+++ ./speedtext2.txt	Thu Dec 12 03:08:59 2019
@@ -1,7 +1,5 @@
 == Capital-Saratoga ==
-aaa
+abc
 bbb
 ccc
-ddd
 
-

```
#### the same module:
If you found the same module, please inform me in issue, thanks!
