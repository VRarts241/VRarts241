

<!DOCTYPE html><html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>VR Arts</title>
<style>
  body {
    font-family: Arial, sans-serif;
    margin: 0;
    background: #f2f2f2;
    padding: 20px;
  }
  .container {
    max-width: 450px;
    margin: auto;
    background: white;
    padding: 20px;
    border-radius: 12px;
    box-shadow: 0 0 10px rgba(0,0,0,0.2);
  }
  h2 {
    text-align: center;
  }
  select, input {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
    border-radius: 8px;
    border: 1px solid #aaa;
  }
  button {
    width: 100%;
    padding: 12px;
    background: #000;
    color: white;
    font-size: 16px;
    border: none;
    border-radius: 8px;
    cursor: pointer;
  }
  button:hover {
    background: #333;
  }
</style>
</head>
<body>
<div class="container">
  <h2>@VRarts241</h2><label>Choose Art Type</label> <select id="artType"> <option value="Anime Sketch - 400 Rs">Anime Sketch - 400 Rs</option> <option value="Single Person Sketch - 400 Rs">Single Person Sketch - 400 Rs</option> <option value="Two Person Sketch - 500 Rs">Two Person Sketch - 500 Rs</option> <option value="Three or More Sketch - 600 Rs">Three or More Sketch - 600 Rs</option> <option value="Single Person Painting - 600 Rs">Single Person Painting - 600 Rs</option> <option value="Two Person Painting - 800 Rs">Two Person Painting - 800 Rs</option> <option value="Others">Others</option> </select>

<label>Upload Reference Photo (optional)</label> <input type="file" id="photo" accept="image/*" />

<label>Your Phone Number</label> <input type="tel" id="phone" placeholder="Enter phone number" />

<button onclick="sendMessage()">Done</button>

</div><script>
function sendMessage() {
  let art = document.getElementById('artType').value;
  let phone = document.getElementById('phone').value;

  if (!phone) {
    alert("Please enter your phone number");
    return;
  }

  // WhatsApp message format
  let message = `New Art Request:%0AArt Type: ${art}%0APhone: ${phone}`;

  // Send to your number
  window.location.href = `https://wa.me/8957022089?text=${message}`;
}
</script></body>
</html>
<!--
**VRarts241/VRarts241** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
