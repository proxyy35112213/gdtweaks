# gdtweaks
# Re-create the zip file with the previous website content
import zipfile

file_path = "/mnt/data/gdtweaks_website_final.zip"

# Create the zip file containing the website files
with zipfile.ZipFile(file_path, 'w') as z:
    z.writestr("index.html", """
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>GD Tweaks</title>
  <style>
    body {\n      background-color: black;\n      color: white;\n      font-family: 'Burbank Big Condensed', sans-serif;\n      text-align: center;\n      margin: 0;\n      padding: 0;\n    }\n\n    h1 {\n      font-size: 50px;\n      margin-top: 50px;\n    }\n\n    .button {\n      background-color: limegreen;\n      color: black;\n      padding: 15px 30px;\n      text-decoration: none;\n      font-size: 20px;\n      border-radius: 8px;\n      display: inline-block;\n      margin-top: 20px;\n    }\n\n    .social-icons {\n      display: flex;\n      justify-content: space-between;\n      position: fixed;\n      bottom: 20px;\n      width: 100%;\n      padding: 0 50px;\n      box-sizing: border-box;\n    }\n\n    .social-icons a img {\n      width: 40px;\n    }\n\n    .container {\n      max-width: 800px;\n      margin: 0 auto;\n    }\n  </style>\n</head>\n<body>\n\n  <div class=\"container\">\n    <h1>GD TWEAKS</h1>\n    <img src=\"https://cdn.discordapp.com/attachments/1312409265192833024/1330956225596358807/GD.gif\" alt=\"Logo GD\" width=\"200\">\n    \n    <p>¿QUIERES +FPS 📈 REDUCIR DELAY y MEJORAR los BAJONES de FPS?<br>\n      GD TWEAKS ES TU SOLUCIÓN ✅\n    </p>\n\n    <a href=\"#\" class=\"button\">MÁS INFORMACIÓN 👀</a>\n\n    <div class=\"social-icons\">\n      <a href=\"https://www.tiktok.com/@prooxxyfn?_t=ZN-8tVdZzgFtIM&_r=1\" target=\"_blank\">\n        <img src=\"https://upload.wikimedia.org/wikipedia/commons/6/6f/TikTok_Logo.svg\" alt=\"TikTok\">\n      </a>\n      <a href=\"https://discord.gg/8KfXfjKPVC\" target=\"_blank\">\n        <img src=\"https://upload.wikimedia.org/wikipedia/en/9/98/Discord_logo.svg\" alt=\"Discord\">\n      </a>\n    </div>\n  </div>\n\n  <script>\n    // Redirigir \"Reseñas\" al enlace de Discord\n    document.querySelector('.button').addEventListener('click', function() {\n      window.location.href = \"https://discord.gg/8KfXfjKPVC\";\n    });\n  </script>\n\n</body>\n</html>
""")

file_path
