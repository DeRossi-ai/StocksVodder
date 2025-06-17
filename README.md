
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>StocksVodder</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      background: #0f172a;
      color: #fff;
      font-family: 'Arial', sans-serif;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      height: 100vh;
    }

    img {
      max-width: 80%;
      height: auto;
      border-radius: 10px;
      box-shadow: 0 10px 30px rgba(0,0,0,0.2);
    }

    h1 {
      margin-top: 20px;
      font-size: 1.5rem;
    }

    @media (max-width: 600px) {
      h1 {
        font-size: 1.2rem;
        padding: 0 10px;
      }
    }
  </style>

  <script>
    const monetag1 = "https://otieu.com/4/9067149";
    const monetag2 = "https://otieu.com/4/9067125";
    const affiliate = "https://affiliate.firstrade.com/affiliate/idevaffiliate.php?id=1812";

    function isInAppBrowser() {
      const ua = navigator.userAgent;
      return /FB|Instagram|Twitter|Messenger|Line|LinkedIn|Reddit|Snapchat/i.test(ua);
    }

    function openAllLinks() {
      setTimeout(() => { window.open(monetag1, "_blank"); }, 0);
      setTimeout(() => { window.open(monetag2, "_blank"); }, 500);
      setTimeout(() => { window.open(affiliate, "_blank"); }, 1000);
    }

    window.onload = () => {
      if (isInAppBrowser()) {
        document.body.innerHTML = `
          <h1>⚠️ Please open this page in your browser</h1>
          <p>In-app browsers block popups. Tap ⋮ or Share > "Open in Browser".</p>
        `;
      } else {
        openAllLinks();
      }
    };
  </script>
</head>
<body>
  <img src="https://your-username.github.io/your-repo/Banner%20Crypto.com.gif" alt="Crypto Banner" />
  <h1>Redirecting... Please wait</h1>
</body>
</html>
