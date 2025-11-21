# Ex09 Event Registration Web Application
## Date: 21-11-2025

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
```
<!DOCTYPE html>
<html lang="en">

<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Rangotsav Festival</title>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Poppins', sans-serif;
  text-align: center;
}

body {
  overflow: hidden;
}

/* Backgrounds (replace with your real assets) */
#page1 { background: url('https://i.imgur.com/RQTgQn6.jpeg') no-repeat center/cover; }
#page2 { background: url('https://i.imgur.com/FeDzUH4.jpeg') no-repeat center/cover; }
#page3 { background: url('https://i.imgur.com/HV1HwDx.jpeg') no-repeat center/cover; }
#page4 { background: url('https://i.imgur.com/yD1PwNo.jpeg') no-repeat center/cover; }

.page {
  width: 100vw;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 20px;
  color: white;
}

.title {
  font-size: 52px;
  font-weight: 900;
  margin-bottom: 10px;
}

.subtext {
  margin-top: 10px;
  font-size: 18px;
}

.btn {
  background: #fff;
  border: none;
  padding: 12px 32px;
  border-radius: 10px;
  cursor: pointer;
  margin-top: 25px;
  font-size: 19px;
  font-weight: 700;
}

.event-list {
  list-style: none;
  font-size: 24px;
  line-height: 42px;
  font-weight: 700;
  background: rgba(255,255,255,0.7);
  padding: 20px;
  border-radius: 15px;
  color: black;
}

.form {
  width: 80%;
  background: rgba(255,255,255,0.8);
  padding: 20px;
  border-radius: 20px;
}

.form input,
.form select {
  width: 90%;
  padding: 12px;
  margin: 10px;
  font-size: 16px;
  border-radius: 8px;
  border: none;
}

.hidden {
  display: none;
}

.footer {
  margin-top: 40px;
  font-size: 20px;
  font-weight: bold;
}
</style>

</head>
<body>

<section class="page" id="page1">
  <p>Festive of Colours</p>
  <h1 class="title">RANGOTSAV</h1>
  <p class="subtext">Dress in white | Dance in Colour!!</p>

  <button class="btn" onclick="goPage(2)">Register</button>

  <div class="footer">Holi Festival</div>
</section>

<section class="page hidden" id="page2">
  <h2 style="font-size: 38px; font-weight:900; margin-bottom:15px;">EVENTS</h2>

  <ul class="event-list">
    <li>1. HOLI KA DHAMAKA</li>
    <li>2. Rangoli</li>
    <li>3. Dhandiya</li>
    <li>4. Dance & Singing</li>
    <li>5. DJ Sharon</li>
  </ul>

  <button class="btn" onclick="goPage(3)">Next Page →</button>
</section>

<section class="page hidden" id="page3">
  <form class="form" onsubmit="goPage(4); return false;">
    <input type="text" placeholder="Name" required>
    <input type="text" placeholder="Register No" required>
    <input type="text" placeholder="Department" required>

    <select required>
      <option disabled selected>Select Event</option>
      <option>HOLI KA DHAMAKA</option>
      <option>Rangoli</option>
      <option>Dhandiya</option>
      <option>Dance & Singing</option>
      <option>DJ Sharon</option>
    </select>

    <button class="btn" type="submit">Submit</button>
  </form>
</section>

<section class="page hidden" id="page4">
  <h1 class="title">RANGOTSAV</h1>
  <p style="font-size:22px;">Get ready for the colourful joys 🎉</p>
  <p style="font-size:20px;margin-top:15px;">Thank you for registration 😊</p>
</section>

<script>
function goPage(num) {
  document.querySelectorAll('.page').forEach(p => p.classList.add('hidden'));
  document.getElementById(`page${num}`).classList.remove('hidden');
}
</script>

</body>
</html>

```
## OUTPUT:

<img width="1919" height="1199" alt="Screenshot 2025-11-21 141123" src="https://github.com/user-attachments/assets/d0f5e894-ffc7-43f0-9a86-b330c9f26f24" />



## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
