<!DOCTYPE html>
<html lang="th">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>จกจิ๊ง</title>
</head>
<body>
  <h1>สินค้า</h1>
  <div id="list">กำลังโหลด...</div>

  <script type="module">
    import { initializeApp } from "https://www.gstatic.com/firebasejs/10.x.x/firebase-app.js";
    import { getFirestore, collection, getDocs } from "https://www.gstatic.com/firebasejs/10.x.x/firebase-firestore.js";

    // เอาค่า Firebase Config ที่ก๊อปปี้มา มาวางตรงนี้
    const firebaseConfig = {
      apiKey: "AIzaSyA16VXbSopR3NTBMD-SU-RCgJV5zLPkkBU",
      authDomain: "jokjing-shop.firebaseapp.com",
      projectId: "jokjing-shop",
      storageBucket: "jokjing-shop.firebasestorage.app",
      messagingSenderId: "559683140548",
      appId: "1:559683140548:web:f540aa77108c5a171cc291"
    };

    const app = initializeApp(firebaseConfig);
    // โค้ดส่วนอื่นๆ สำหรับดึงสินค้ามาแสดง...
  </script>
</body>
</html>
