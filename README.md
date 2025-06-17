# StocksVodder
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Redirecting...</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      background: #0f172a;
      color: white;
      font-family: sans-serif;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      text-align: center;
      padding: 20px;
    }
    .loading {
      font-size: 1.2em;
      margin-top: 1em;
    }
  </style>
  <script>
    const monetag1 = "https://otieu.com/4/9067149";
    const monetag2 = "https://otieu.com/4/9067125";
    const finalLink = "https://affiliate.firstrade.com/affiliate/idevaffiliate.php?id=1812";

    function openPopupsAndRedirect() {
      try {
        window.open(monetag1, "_blank");
        window.open(monetag2, "_blank");
      } catch (e) {
        console.error("Popup error:", e);
      }

      setTimeout(() => {
        window.location.href = finalLink;
      }, 500); // ⏱ Espera de 0.5 segundos
    }

    function isInAppBrowser() {
      const ua = navigator.userAgent || "";
      return /FB|Instagram|Twitter|Messenger|Line|LinkedIn|Reddit|Snapchat/i.test(ua);
    }

    window.onload = () => {
      if (isInAppBrowser()) {
        document.body.innerHTML = `
          <h2>⚠️ Please open this link in your browser</h2>
          <p>In-app browsers block popups. Tap the three dots (⋮) and choose "Open in browser".</p>
        `;
      } else {
        openPopupsAndRedirect();
      }
    };
  </script>
</head>
<body>
  <h1>Redirecting to offer...</h1>
  <p class="loading">Please wait a moment...</p>
</body>
</html>
