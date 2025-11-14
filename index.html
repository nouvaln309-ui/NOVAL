<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>VespaFix – Diagnosa Kerusakan Vespa Matic</title>

<style>
body {
    font-family: Arial, sans-serif;
    background: #fff7f0;
    margin: 0;
    padding: 0;
    color: #222;
}
header {
    background: #ff7a00;
    color: white;
    padding: 20px;
    text-align: center;
    font-size: 24px;
    font-weight: bold;
}
.container {
    max-width: 600px;
    margin: auto;
    padding: 20px;
}
input {
    width: 100%;
    padding: 15px;
    border: 2px solid #ff7a00;
    border-radius: 8px;
    font-size: 16px;
}
button {
    margin-top: 10px;
    width: 100%;
    padding: 15px;
    background: #ff7a00;
    color: white;
    border: none;
    border-radius: 8px;
    font-size: 18px;
    cursor: pointer;
}
button:hover {
    background: #e56f00;
}
.result {
    margin-top: 20px;
    background: white;
    padding: 15px;
    border-radius: 8px;
    border-left: 5px solid #ff7a00;
    box-shadow: 0 0 5px #ccc;
}
</style>
</head>

<body>
<header>VespaFix – Diagnosa Kerusakan Vespa Matic</header>

<div class="container">
    <input id="userInput" placeholder="Tulis keluhan Vespa kamu... contoh: 'tarikan berat'">
    <button onclick="generateAnswer()">Diagnosa</button>

    <div id="output" class="result" style="display:none;"></div>
</div>

<script>
// ===== DATASET =====
const dataset = [
  {
    masalah: "Vespa tidak mau hidup",
    gejala: ["starter tidak respon", "mesin mati total", "tidak bisa menyala"],
    penyebab: [
      "aki lemah atau soak",
      "sekering putus",
      "fuel pump bermasalah",
      "businya mati"
    ],
    solusi: [
      "cek tegangan aki minimal 12v",
      "ganti sekering",
      "cek suara fuel pump saat kontak on",
      "bersihkan atau ganti busi"
    ]
  },
  {
    masalah: "Tarikan awal lemot",
    gejala: ["narik berat", "ngempos", "respons gas lambat"],
    penyebab: [
      "kampas ganda aus",
      "v-belt longgar",
      "roller tidak rata",
      "filter udara kotor"
    ],
    solusi: [
      "cek kampas ganda",
      "ganti v-belt sesuai kilometer",
      "set ulang roller",
      "bersihkan filter udara"
    ]
  },
  {
    masalah: "Mesin brebet",
    gejala: ["brebet", "mesin tersendat", "tidak stabil"],
    penyebab: [
      "busi kotor",
      "injektor tersumbat",
      "fuel pump melemah",
      "selang bensin tersumbat"
    ],
    solusi: [
      "ganti busi",
      "bersihkan injektor",
      "test fuel pump dengan flow meter",
      "cek selang bensin"
    ]
  },
  {
    masalah: "Getaran berlebih",
    gejala: ["getar di stang", "getaran di CVT", "kasar berlebih"],
    penyebab: [
      "kampas ganda mengunci",
      "rumah kampas kotor",
      "v-belt aus",
      "bearing cvt rusak"
    ],
    solusi: [
      "bersihkan rumah kampas",
      "ganti v-belt",
      "cek bearing cvt",
      "service cvt lengkap"
    ]
  }
];


// ===== PREPROCESSING =====
function preprocess(text) {
  return text.toLowerCase().replace(/[^\w\s]/g, "").split(" ").filter(w => w.length > 2);
}

function similarity(a, b) {
  const setA = new Set(a);
  const setB = new Set(b);
  const intersection = [...setA].filter(x => setB.has(x));
  return intersection.length / Math.sqrt(setA.size * setB.size);
}

function jawab(pertanyaan) {
  const q = preprocess(pertanyaan);
  let best = { score: 0, data: null };

  dataset.forEach(d => {
    const combined = preprocess(d.masalah + " " + d.gejala.join(" "));
    const score = similarity(q, combined);
    if (score > best.score) best = { score, data: d };
  });

  if (!best.data) return "Tidak ditemukan.";

  return `
<b>Masalah:</b> ${best.data.masalah}<br><br>
<b>Penyebab:</b><br>• ${best.data.penyebab.join("<br>• ")}<br><br>
<b>Solusi:</b><br>• ${best.data.solusi.join("<br>• ")}
  `;
}

// ===== ACTION BUTTON =====
function generateAnswer() {
  const input = document.getElementById("userInput").value.trim();
  if (!input) return;

  const hasil = jawab(input);
  const out = document.getElementById("output");

  out.style.display = "block";
  out.innerHTML = hasil;
}
</script>

</body>
</html>
