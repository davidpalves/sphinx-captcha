# Sphinx Captcha Generator

The CAPTCHA generated is like this:

![1](https://github.com/davidpierre21/sphinx-captcha/raw/master/samples/0CVSX_a405.jpg)
![2](https://github.com/davidpierre21/sphinx-captcha/raw/master/samples/0N3OG_a404.jpg)
![3](https://github.com/davidpierre21/sphinx-captcha/raw/master/samples/V7KZC_a406.jpg)

### How to use
Change the batch_create_img function parameter on the main section of the code to choose how many captcha images you want to generate. You can run
```python captcha.py```   to generate the captchas.

### example:
```python
from captcha import Captcha


characters_set = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'K', 'M',
                  'N', 'P', 'R', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z',
                  '0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
characters_per_img = 5
min_width, min_height = 150, 40
c = Captcha(min_width, min_height, characters_set, characters_per_img, debug=True)
c.batch_create_img(5)
```
---

### Warning
You may encounter some issues while trying to generate with a different number of letters,
it happens because the width of the string generated is greater than the width of the image canvas. 
