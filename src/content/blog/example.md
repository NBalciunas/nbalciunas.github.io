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

<h2>Kontaktinė forma</h2>
<form id="contactForm" style="color:white">
    <label for="firstName">Vardas:</label><br>
    <input type="text" id="firstName" name="firstName" style="color:black" required><br>
    <label for="lastName">Pavardė:</label><br>
    <input type="text" id="lastName" name="lastName" style="color:black" required><br>
    <label for="email">El. paštas:</label><br>
    <input type="email" id="email" name="email" style="color:black" required><br>
    <label for="phone">Telefono numeris:</label><br>
    <input type="tel" id="phone" name="phone" style="color:black" required><br>
    <label for="address">Adresas:</label><br>
    <input type="text" id="address" name="address" style="color:black" required><br><br>
    <label for="extra1">Extra 1:</label><br>
    <input type="number" id="extra1" name="extra1" style="color:black" required><br>
    <label for="extra2">Extra 2:</label><br>
    <input type="number" id="extra2" name="extra2" style="color:black" required><br>
    <label for="extra3">Extra 3:</label><br>
    <input type="number" id="extra3" name="extra3" style="color:black" required><br>
    <label for="extra4">Extra 4:</label><br>
    <input type="number" id="extra4" name="extra4" style="color:black" required><br>
    <label for="extra5">Extra 5:</label><br>
    <input type="number" id="extra5" name="extra5" style="color:black" required><br><br>
    <button type="button" style="border: 2px solid white; padding: 8px 16px; color: white; background-color: transparent;" onclick="saveForm() ">Išsaugoti</button>
</form>

<div id="result"></div>

<script>
function saveForm() {
    const form = document.getElementById('contactForm');
    const firstName = form.firstName.value;
    const lastName = form.lastName.value;
    const email = form.email.value;
    const phone = form.phone.value;
    const address = form.address.value;

    const extra1 = parseInt(form.extra1.value, 10);
    const extra2 = parseInt(form.extra2.value, 10);
    const extra3 = parseInt(form.extra3.value, 10);
    const extra4 = parseInt(form.extra4.value, 10);
    const extra5 = parseInt(form.extra5.value, 10);

    if(!validateEmail(email)){
        alert('Netinkamas el. pašto formatas');
    }

    if(!validatePhone(phone)){
        alert('Netinkamas telefono numeris');
        return;
    }

    const visitorData = {
        firstName,
        lastName,
        email,
        phone,
        address,
        extras: [extra1, extra2, extra3, extra4, extra5]
    };

    console.log(visitorData);

    let output = `
      <p>Vardas: ${visitorData.firstName}</p>
      <p>Pavardė: ${visitorData.lastName}</p>
      <p>El. paštas: ${visitorData.email}</p>
      <p>Telefonas: ${visitorData.phone}</p>
      <p>Adresas: ${visitorData.address}</p>
      <p>Extra 1: ${extra1}</p>
      <p>Extra 2: ${extra2}</p>
      <p>Extra 3: ${extra3}</p>
      <p>Extra 4: ${extra4}</p>
      <p>Extra 5: ${extra5}</p>
    `;

    const average = calculateAverage(visitorData.extras);
    let averageColorClass = 'average-green';
    if (average < 4) {
        averageColorClass = 'average-red';
    } else if (average < 7) {
        averageColorClass = 'average-orange';
    }

    output += `<p class="${averageColorClass}">${visitorData.firstName} ${visitorData.lastName} (${visitorData.email}): ${average.toFixed(2)}</p>`;
    const alertMessage = `
      Vardas: ${visitorData.firstName}
      Pavardė: ${visitorData.lastName}
      El. paštas: ${visitorData.email}
      Telefonas: ${visitorData.phone}
      Adresas: ${visitorData.address}
      Požymis 1: ${extra1}
      Požymis 2: ${extra2}
      Požymis 3: ${extra3}
      Požymis 4: ${extra4}
      Požymis 5: ${extra5}
    `;

    document.getElementById('result').innerHTML = output;
    alert(alertMessage);
}

function calculateAverage(numbers){
    const sum = numbers.reduce((total, num) => total + num, 0);
    return sum / numbers.length;
}

function validateEmail(email){
    const re = /\S+@\S+\.\S+/;
    return re.test(email);
}

function validatePhone(phone){
    const re = /^\d{9,}$/;
    return re.test(phone);
}
</script>
