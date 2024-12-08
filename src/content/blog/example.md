---
author: Nojus Balčiūnas
pubDatetime: 2024-00-00T00:00:00
modDatetime: 2024-00-01T00:00:00
title: Example
slug: example
ogImage: SITE.ogImage
featured: false
draft: false
tags:
  - example
description: Example
---

# Hello1
## Hello2
### Hello3
#### Hello4
##### Hello5
###### Hello6

> One
>> Two
>>> Three

- One
- Two
- Three

# <b>b tag</b>
# <i>i tag</i>
# <u>u tag</u>

```py
print("Hello, world!")
```

![Image](@assets/images/logo.jpg)

![something](../../assets/images/logo.jpg)

<center>
<video width="600" height="auto" controls>
  <source src="/assets/heavy-lift-quadcopter/1.mp4" type="video/mp4">
</video>
</center>

<iframe width="100%" height="600" frameborder="0" scrolling="no" marginheight="0" marginwidth="0" src="https://maps.google.com/maps?width=100%25&amp;height=600&amp;hl=en&amp;q=+(Panev%C4%97%C5%BEys)&amp;t=&amp;z=12&amp;ie=UTF8&amp;iwloc=B&amp;output=embed"><a href="https://www.gps.ie/">gps vehicle tracker</a></iframe>

<center>
    <audio controls>
      <source src="/assets/example/example.mp3" type="audio/mpeg">
    </audio>
</center>

| 1 | 2 | 3 |
|---|---|---|
| 4 | 5 | 6 |
| 7 | 8 | 9 |

[Google](https://www.google.com)

<center>
    <p>MathML Example</p>
    <div style="font-size: 1.5em; font-weight: 300; color: #ffffff;">
        <math xmlns="http://www.w3.org/1998/Math/MathML">
            <mfrac>
                <mrow>
                    <mo>-</mo>
                    <mi>b</mi>
                    <mo>±</mo>
                    <msqrt>
                        <mrow> 
                            <msup>
                                <mi>b</mi>
                                <mn>2</mn>
                            </msup>
                            <mo>-</mo>
                            <mn>4</mn>
                            <mo>&#8290;</mo>
                            <mi>a</mi>
                            <mo>&#8290;</mo>
                            <mi>c</mi> 
                        </mrow>
                    </msqrt>
                </mrow>
                <mrow>
                    <mn>2</mn>
                    <mo>&#8290;</mo>
                    <mi>a</mi>
                </mrow>
            </mfrac>
        </math>
    </div>
</center>

<center>
    <p>Animation Example</p>
    <svg width="100%" height="400" viewBox="0 0 800 400" xmlns="http://www.w3.org/2000/svg" style="display:block; width:100%; height:400px;">
        <rect width="800" height="400" fill="white" />
        <rect x="0" y="150" width="100" height="100" fill="blue">
            <animate 
                attributeName="x" 
                from="0" 
                to="700" 
                dur="2s" 
                begin="0s" 
                repeatCount="indefinite" />
        </rect>
    </svg>
</center>

<center>
    <p>Real Time Clock Example</p>
    <div id="clock" style="font-size: 1.5em; color: #ffffff;"></div>
    <script>
        function updateClock(){
            const now = new Date();
            const hours = String(now.getHours()).padStart(2, '0');
            const minutes = String(now.getMinutes()).padStart(2, '0');
            const seconds = String(now.getSeconds()).padStart(2, '0');
            document.getElementById('clock').textContent = `${hours}:${minutes}:${seconds}`;
        }
        setInterval(updateClock, 1000);
        updateClock();
    </script>
</center>
