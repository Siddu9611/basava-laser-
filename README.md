# basava-laser-
laser cuttinh
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Basava Laser Industrie</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
    }
    .orange-section {
      background-color: orange;
      color: #fff;
      padding: 40px 20px;
    }
    .orange-section h1 {
      font-size: 3em;
      margin: 0;
      font-weight: bold;
    }
    .orange-section h2 {
      font-size: 2em;
      margin: 10px 0 20px;
    }
    .section-content {
      background-color: #fff;
      color: #333;
      padding: 20px;
      border-radius: 10px;
      margin: 20px auto;
      max-width: 800px;
    }
    .section-content.alt {
      background-color: #f0f0f0;
    }
    .highlight-link {
      text-align: center;
      margin-top: 30px;
    }
    .highlight-link a {
      font-size: 1.5em;
      color: red;
      font-weight: bold;
      text-decoration: none;
    }
    .black-section {
      background-color: #000;
      color: white;
      padding: 30px 20px;
    }
    .black-section h2 {
      color: yellow;
      text-align: center;
      font-size: 2em;
    }
    form {
      background-color: #fff;
      color: #000;
      padding: 20px;
      margin: 20px auto;
      max-width: 800px;
      border-radius: 10px;
    }
    label {
      display: block;
      margin: 10px 0 5px;
      font-weight: bold;
    }
    input, select, textarea {
      width: 100%;
      padding: 8px;
      margin-bottom: 10px;
      border-radius: 5px;
      border: 1px solid #ccc;
    }
    button {
      background-color: #ff6600;
      color: white;
      padding: 12px 20px;
      border: none;
      border-radius: 5px;
      font-size: 1em;
      cursor: pointer;
    }
  </style>
</head>
<body>

  <!-- ORANGE INTRO SECTION -->
  <div class="orange-section">
    <h1>BASAVA</h1>
    <h2>LASER INDUSTRIE</h2>
    <p><em>Plot No. 69, 1st Main Road, Auto Complex, Shimoga</em></p>
  </div>

  <!-- ABOUT & TYPES OF WORK -->
  <div class="section-content">
    <h3>About Our Company</h3>
    <p>We have a knack for quality design and output. Our quality vector designs encompass laser cutting systems. We are passionate about providing quality detailed designs for significant categories.</p>

    <h3>"TYPES OF WORK"</h3>
    <ul>
      <li>We can make any design from photos into cutting files</li>
      <li>Jolly cuttings (gate designs and exterior roof designs)</li>
      <li>Brass sheet cutting (Cuttings and markings)</li>
      <li>SS sheet cuttings (For interior design and partition)</li>
      <li>MS sheet cuttings (Elevation designs, gates, windows, skylights)</li>
    </ul>
  </div>

  <!-- INDUSTRIAL CUTTINGS -->
  <div class="section-content alt">
    <p style="color:blue; font-weight:bold;">
      We also do all types of industrial components cutting and bunkers, elevators for rice mill industries.
    </p>
    <ul>
      <li>Body frame cutting in MS sheet (0–18mm)</li>
      <li>Body frame cutting in SS sheet (0–8mm)</li>
      <li>Chassis frame cuttings</li>
      <li>Areca nut dehusker conveyor cuttings</li>
      <li>Spring steel blades cuttings</li>
      <li>Areca nut peeling machine parts cuttings</li>
    </ul>

    <div class="highlight-link">
      <a href="#order">Click to Order Now</a>
    </div>
  </div>

  <!-- ORDER FORM SECTION -->
  <div class="black-section" id="order">
    <h2>WELCOME TO BASAVA LASER INDUSTRIES</h2>
  </div>

  <form id="orderForm">
    <label>Width Size</label>
    <select name="widthUnit">
      <option>Inch</option>
      <option>MM</option>
      <option>Feet</option>
    </select>
    <input type="text" name="width" required>

    <label>Height Size</label>
    <select name="heightUnit">
      <option>Inch</option>
      <option>MM</option>
      <option>Feet</option>
    </select>
    <input type="text" name="height" required>

    <label>Metal Type</label>
    <select name="metal">
      <option>MS</option>
      <option>SS</option>
      <option>GI</option>
      <option>Other</option>
    </select>

    <label>Thickness (mm or gauge)</label>
    <input type="text" name="thickness" required>

    <label>Upload Drawing Images</label>
    <input type="file" name="images" multiple>

    <label>Phone Number</label>
    <input type="tel" name="phone" required>

    <label>Address</label>
    <textarea name="address" required></textarea>

    <label>Email ID (Optional)</label>
    <input type="email" name="email">

    <label>Frame Border Size (inch/mm/feet)</label>
    <input type="text" name="borderSize">

    <button type="submit">Submit Order</button>
  </form>

  <script>
    document.getElementById("orderForm").addEventListener("submit", function(event) {
      event.preventDefault();
      const form = event.target;
      const data = {
        width: form.width.value + " " + form.widthUnit.value,
        height: form.height.value + " " + form.heightUnit.value,
        metal: form.metal.value,
        thickness: form.thickness.value,
        phone: form.phone.value,
        address: form.address.value,
        email: form.email.value,
        borderSize: form.borderSize.value
      };

      const message = `New Order Details:
Width: ${data.width}
Height: ${data.height}
Metal Type: ${data.metal}
Thickness: ${data.thickness}
Phone: ${data.phone}
Address: ${data.address}
Email: ${data.email}
Frame Border Size: ${data.borderSize}`;

      // Send to Email
      window.location.href = mailto:siddeshjb4@gmail.com?subject=New Order&body=${encodeURIComponent(message)};

      // Send to WhatsApp
      window.open(https://wa.me/919611438319?text=${encodeURIComponent(message)}, '_blank');
    });
  </script>
</body>
</html>
