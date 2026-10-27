<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>จกจิ้ง</title>
</head>
<body>
<h1>สินค้า</h1>
<div id="list">กำลังโหลด...</div>
<script type="module">
import { initializeApp } from "https://www.gstatic.com/firebasejs/10.12.2/firebase-app.js";
import { getFirestore, collection, getDocs } from "https://www.gstatic.com/firebasejs/10.12.2/firebase-firestore.js";

const app = initializeApp({
  // วาง firebaseConfig ที่คัดลอกไว้ตรงนี้
});
const db = getFirestore(app);

const snap = await getDocs(collection(db, "products"));
document.getElementById("list").innerHTML = snap.docs.map(d => {
  const p = d.data();
  return `<div><h3>${p.name}</h3><p>${p.price} บาท</p></div>`;
}).join("");
</script>
</body>
</html>
