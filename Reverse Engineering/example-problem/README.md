# Example Problem

## Overview

Points: 500

Year: 2077

Author: someone_cool

## Description

This is an example problem description. Do stuff. I heard if you run [flag_generator.py](./attachments/flag_generator.py) it will give you the flag. `nc example.com 1337`

- [src.zip](./attachments/src.zip)

## Hints

1. Put the problem hints here.

2. If no hints, just put NA.

## Approach

First I read the problem description very carefully.

Then I got stuck.

And then because I got stuck I went to chatgpt.

![insert description of my screenshot of chatpgt being useless here](./media/chatgpt-screenshot.png)

However, chatgpt did not feel like collaborating, so I wrote my own python code. You can find the solve script below, or at [solve.py](./solve/solve.py).

```PY
import os
import sys
import time
import random

# gave me the correct flag after a couple of runs.
# trust.
print(os.urandom(36))
```

Running that python code a couple of times gave me the correct flag.

## Flag

`picoCTF{definitely_a_real_flag_2077}`

---

## Referenced materials

[include links to referenced materials, writeups, etc. here](https://google.com)
