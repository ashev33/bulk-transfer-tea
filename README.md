
```markdown
# Bulk Transfer TEA Token

Skrip ini digunakan untuk mentransfer token TEA secara massal ke banyak alamat di jaringan **Tea Sepolia** menggunakan **JSON-RPC**. Anda bisa menginput jumlah penerima dan jumlah token yang dikirimkan, serta mengatur jumlah token secara acak dalam rentang tertentu.

## ✨ Fitur

- Menggunakan **RPC Tea Sepolia** untuk transaksi token.
- Mengimpor **wallet dari private key**.
- **Mengirim token ke banyak alamat acak** dalam satu eksekusi.
- Jumlah token yang dikirim **diatur secara random** antara **500 juta - 1,5 miliar**.
- Log transaksi yang jelas untuk setiap pengiriman.

---

## ⚡ Persyaratan

Sebelum menggunakan skrip ini, pastikan Anda memiliki:

1. **Node.js** dan **npm** (Unduh di: [Node.js Official Site](https://nodejs.org/)).
2. **Private Key** dari wallet yang memiliki saldo TEA token.
3. **RPC URL** dari jaringan **Tea Sepolia** (gunakan layanan seperti [Alchemy](https://www.alchemy.com/)).
4. **Smart Contract Address** dari token TEA yang akan dikirim.

---

## 🚀 Instalasi dan Penggunaan

### 1️⃣ Clone Repository

Clone repository ini ke komputer Anda:

```bash
git clone https://github.com/ashev33/bulk-transfer-tea.git
cd bulk-transfer-tea
```

### 2️⃣ Instalasi Dependensi

Jalankan perintah berikut untuk menginstal dependensi:

```bash
npm install ethers
```

### 3️⃣ Konfigurasi Skrip

Sebelum menjalankan skrip, lakukan beberapa konfigurasi:

1. **Masukkan Private Key**  
   Anda perlu memasukkan private key wallet yang akan digunakan untuk mentransfer token dalam file konfigurasi.

2. **Gunakan RPC URL yang benar**  
   Pastikan Anda menggunakan **RPC URL dari Tea Sepolia** yang bisa diperoleh dari Alchemy atau penyedia lain.

3. **Smart Contract Address**  
   Pastikan alamat smart contract token TEA yang digunakan benar.

---

### 4️⃣ Menjalankan Skrip

Untuk menjalankan skrip, gunakan perintah:

```bash
node transfer.js
```

Kemudian, skrip akan meminta input:

- **Jumlah penerima**: Masukkan jumlah alamat yang ingin menerima token.
- **Jumlah token yang akan dikirim**: Skrip akan secara otomatis memilih jumlah acak antara **500 juta - 1,5 miliar TEA**.

Setelah itu, skrip akan mulai melakukan transfer dan mencetak hasil transaksi:

```bash
1. Transaction successfully (0x123abc...456def)
2. Transaction successfully (0x789ghi...012jkl)
...
500. Transaction successfully (0xaaa111...bbb222)
```

Jika terjadi error, periksa apakah saldo cukup dan apakah RPC serta smart contract address sudah benar.

---
