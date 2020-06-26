# Sphinx Captcha Generator

This is a fork from [Skyduy](https://github.com/skyduy/CAPTCHA_generator)'s captcha generator.


The CAPTCHA generated is like this:

![1](https://github.com/davidpierre21/sphinx-captcha/raw/master/samples/0CVSX_a405.jpg)
![2](https://github.com/davidpierre21/sphinx-captcha/raw/master/samples/0N3OG_a404.jpg)
![3](https://github.com/davidpierre21/sphinx-captcha/raw/master/samples/V7KZC_a406.jpg)

### How to use
Execute ```pipenv install``` To install the dependencies. You can run
```python captcha.py```   to generate the captchas with default settings.


for getting the arguments to execute: ```python captcha.py -h```

```
usage: captcha.py [-h] [--width WIDTH] [--height HEIGHT]
                  [--num-characters NUM_CHARACTERS] [--path PATH]
                  [--num-images NUM_IMAGES] [--debug]

Generate captchas easily

optional arguments:
  -h, --help            show this help message and exit
  --width WIDTH         Width of the generated captcha image
  --height HEIGHT       Height of the generated captcha image
  --num-characters NUM_CHARACTERS, -nc NUM_CHARACTERS
                        Number of characters per image
  --path PATH, -p PATH  Path to save the generated captcha images
  --num-images NUM_IMAGES, -n NUM_IMAGES
                        Number of captcha images to be generated
  --debug               Run in debug mode

```
---

### Warning
You may encounter some issues while trying to generate with a different number of letters,
it happens because the width of the string generated is greater than the width of the image canvas.
