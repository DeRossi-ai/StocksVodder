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

    #popupWarning {
      display: none;
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      background: #fff3cd;
      color: #856404;
      border: 1px solid #ffeeba;
      padding: 20px;
      font-size: 16px;
      font-family: Arial, sans-serif;
      z-index: 9999;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
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

    function checkPopupBlocker() {
      const test = window.open('', '', 'width=100,height=100');
      if (!test || test.closed || typeof test.closed === "undefined") {
        document.getElementById("popupWarning").style.display = "block";
        return true;
      } else {
        test.close();
        return false;
      }
    }

    function openAllLinks() {
      setTimeout(() => window.open(monetag1, "_blank"), 0);
      setTimeout(() => window.open(monetag2, "_blank"), 500);
      setTimeout(() => window.open(affiliate, "_blank"), 1000);
    }

    window.onload = () => {
      if (isInAppBrowser()) {
        document.body.innerHTML = `
          <h1>⚠️ Please open this page in your browser</h1>
          <p>In-app browsers block popups. Tap ⋮ or Share > "Open in Browser".</p>
        `;
      } else {
        const blocked = checkPopupBlocker();
        if (!blocked) openAllLinks();
      }
    };
  </script>
</head>
<body>
  <div id="popupWarning">
    <strong>⚠️ Important Notice:</strong>  
    It seems that your browser has blocked pop-up windows.  
    We use <strong>non-intrusive ads</strong> to keep our content free and accessible.<br><br>
    👉 Please enable pop-ups or open this page in a standard browser to continue.
  </div>

  <img src="https://your-username.github.io/your-repo/Banner%20Crypto.com.gif" alt="Crypto Banner" />
  <h1>Redirecting... Please wait</h1>
</body>
</html>
