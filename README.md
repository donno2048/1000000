# 1000000:

This is the script used to create this repo:
```bash
mkdir 1000000
cd 1000000/
git init
python3 ../1000000.py | git fast-import
git remote add origin https://github.com/donno2048/1000000.git
git push origin master
```
Where this is the content of _1000000.py_:
```py
print('blob\nmark :1\ndata 1\na\nreset refs/heads/master\ncommit refs/heads/master\nmark :2\nauthor donno2048 <just4now666666@gmail.com> 0 +0000\ncommitter donno2048 <just4now666666@gmail.com> 0 +0000\ndata 1\n\nM 100644 :1 a\n')
for i in range(2, 1000001):print(f'commit refs/heads/master\nmark :{i + 1}\nauthor donno2048 <just4now666666@gmail.com> 0 +0000\ncommitter donno2048 <just4now666666@gmail.com> 0 +0000\ndata 1\n\nfrom :{i}\n')
```
