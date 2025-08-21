<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>KOTAK ASPIRASI HME FTIK UNISMU</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Poppins', sans-serif;
      margin: 0;
      background: #f3f4f6;
      color: #1e293b;
    }
    header {
      background: #1e3a8a;
      color: white;
      padding: 1rem;
      text-align: center;
      font-size: 1.5rem;
      font-weight: 600;
      box-shadow: 0 2px 8px rgba(0,0,0,0.2);
    }
    .container {
      max-width: 800px;
      margin: 2rem auto;
      padding: 1rem;
    }
    .card {
      background: white;
      border-radius: 1rem;
      padding: 2rem;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
      margin-bottom: 2rem;
    }
    label {
      display: block;
      margin-bottom: .5rem;
      font-weight: 600;
    }
    input, select, textarea {
      width: 100%;
      padding: .75rem;
      margin-bottom: 1.5rem;
      border: 1px solid #cbd5e1;
      border-radius: .5rem;
      font-size: 1rem;
    }
    textarea {
      resize: vertical;
    }
    button {
      background: #1e3a8a;
      color: white;
      border: none;
      padding: .75rem 1.5rem;
      border-radius: .5rem;
      cursor: pointer;
      font-size: 1rem;
      font-weight: 600;
      transition: all 0.2s;
    }
    button:hover {
      background: #facc15;
      color: #1e3a8a;
    }
    .admin-section {
      display: none;
    }
    table {
      width: 100%;
      border-collapse: collapse;
    }
    th, td {
      padding: .75rem;
      text-align: left;
      border-bottom: 1px solid #e5e7eb;
    }
    th {
      background: #1e3a8a;
      color: white;
    }
    .status {
      padding: .25rem .75rem;
      border-radius: 1rem;
      font-size: .875rem;
      font-weight: 600;
    }
    .baru { background: #fee2e2; color: #b91c1c; }
    .diproses { background: #fef9c3; color: #92400e; }
    .selesai { background: #dcfce7; color: #166534; }
    .login-admin {
      text-align: center;
      margin-bottom: 2rem;
    }
  </style>
</head>
<body>
  <header>KOTAK ASPIRASI HME FTIK UNISMU</header>
  <div class="container">

    <!-- Form Anggota -->
    <div class="card">
      <h2>Form Aspirasi Anggota</h2>
      <form id="aspirasiForm">
        <label for="nama">Nama</label>
        <input type="text" id="nama" required>

        <label for="nim">NIM</label>
        <input type="text" id="nim" required>

        <label for="angkatan">Angkatan</label>
        <input type="text" id="angkatan" required>

        <label for="kategori">Pilihan</label>
        <select id="kategori" required>
          <option value="Himpunan">Himpunan</option>
          <option value="Kampus">Kampus</option>
        </select>

        <label for="pesan">Kritik & Saran</label>
        <textarea id="pesan" rows="4" required></textarea>

        <label for="email">Email</label>
        <input type="email" id="email" required>

        <button type="submit">Kirim Aspirasi</button>
      </form>
    </div>

    <!-- Login Admin -->
    <div class="login-admin">
      <button onclick="showAdminLogin()">Login Admin</button>
    </div>

    <div class="card admin-section" id="adminLoginCard">
      <h2>Login Admin</h2>
      <input type="password" id="adminPin" placeholder="Masukkan PIN">
      <button onclick="loginAdmin()">Login</button>
    </div>

    <!-- Panel Admin -->
    <div class="card admin-section" id="adminPanel">
      <h2>Daftar Aspirasi</h2>
      <table id="aspirasiTable">
        <thead>
          <tr>
            <th>Nama</th>
            <th>NIM</th>
            <th>Angkatan</th>
            <th>Pilihan</th>
            <th>Kritik & Saran</th>
            <th>Email</th>
            <th>Status</th>
            <th>Aksi</th>
          </tr>
        </thead>
        <tbody></tbody>
      </table>
    </div>

  </div>

  <script>
    const form = document.getElementById('aspirasiForm');
    const tableBody = document.querySelector('#aspirasiTable tbody');
    const adminLoginCard = document.getElementById('adminLoginCard');
    const adminPanel = document.getElementById('adminPanel');
    const adminPIN = "654321";

    let aspirasiList = JSON.parse(localStorage.getItem('aspirasiList')) || [];

    function saveData() {
      localStorage.setItem('aspirasiList', JSON.stringify(aspirasiList));
    }

    function renderTable() {
      tableBody.innerHTML = '';
      aspirasiList.forEach((asp, index) => {
        let row = `<tr>
          <td>${asp.nama}</td>
          <td>${asp.nim}</td>
          <td>${asp.angkatan}</td>
          <td>${asp.kategori}</td>
          <td>${asp.pesan}</td>
          <td>${asp.email}</td>
          <td><span class="status ${asp.status.toLowerCase()}">${asp.status}</span></td>
          <td>
            <button onclick="ubahStatus(${index}, 'Baru')">Baru</button>
            <button onclick="ubahStatus(${index}, 'Diproses')">Diproses</button>
            <button onclick="ubahStatus(${index}, 'Selesai')">Selesai</button>
            <button onclick="hapusAspirasi(${index})">Hapus</button>
          </td>
        </tr>`;
        tableBody.innerHTML += row;
      });
    }

    form.addEventListener('submit', (e) => {
      e.preventDefault();
      const data = {
        nama: document.getElementById('nama').value,
        nim: document.getElementById('nim').value,
        angkatan: document.getElementById('angkatan').value,
        kategori: document.getElementById('kategori').value,
        pesan: document.getElementById('pesan').value,
        email: document.getElementById('email').value,
        status: 'Baru'
      };
      aspirasiList.push(data);
      saveData();
      form.reset();
      alert('Aspirasi berhasil dikirim!');
    });

    function showAdminLogin() {
      adminLoginCard.style.display = 'block';
    }

    function loginAdmin() {
      const pin = document.getElementById('adminPin').value;
      if(pin === adminPIN) {
        adminLoginCard.style.display = 'none';
        adminPanel.style.display = 'block';
        renderTable();
      } else {
        alert('PIN salah!');
      }
    }

    function ubahStatus(index, status) {
      aspirasiList[index].status = status;
      saveData();
      renderTable();
    }

    function hapusAspirasi(index) {
      aspirasiList.splice(index, 1);
      saveData();
      renderTable();
    }
  </script>
</body>
</html>
