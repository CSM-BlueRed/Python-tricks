# Python-tricks
A lot of Python tricks that can you save you hours

<hr>

## Underscored ints

```python
number = 10000000
print(number, type(number))

# use this instead:

number = 10_000_000
print(number, type(number))
```
output

```
10000000 <class 'int'>
```

<hr>

## Condition and var assignment

```python
a, b = 1, 2
result = a + b
if result == 3:
    print('ok')

# use this instead:

a, b = 1, 2
if result:= a + b == 3:
    print('ok')
```
output

```
ok
```

## Dict datas update

```python
datas = {
    'content-type': 'application/json',
    'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/102.0.0.0 Safari/537.36'
    'code': 12093
}
datas['token'] = 'hgUYffTRFOyouIUTyterYHOIhuyUYîpojiuorT8OUIhioyR4YUTfomih4IOHRTF'
data['encoding'] = 'utf-8'

print(datas['token'])

# use this instead:

datas = {
    'content-type': 'application/json',
    'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/102.0.0.0 Safari/537.36'
    'code': 12093
}
datas.update({
    'token': 'hgUYffTRFOyouIUTyterYHOIhuyUYîpojiuorT8OUIhioyR4YUTfomih4IOHRTF',
    'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/102.0.0.0 Safari/537.36'
})

print(datas['token'])

```
output

```
hgUYffTRFOyouIUTyterYHOIhuyUYîpojiuorT8OUIhioyR4YUTfomih4IOHRTF
```
