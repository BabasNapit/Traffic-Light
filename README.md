# Traffic-Light

🚦✨ Simulasi Sistem Lalu Lintas Cerdas 4 Arah dengan PLC Omron ✨🚦

Dalam era otomasi industri dan smart city, sistem pengendalian lalu lintas menjadi salah satu aspek penting yang dapat dioptimalkan melalui teknologi. 🔧

Saya baru saja menyelesaikan simulasi lampu lalu lintas 4 ruas (4 arah) berbasis PLC Omron, di mana satu siklus berlangsung selama 60 detik.
Setiap ruas jalan mendapatkan giliran menyala (Hijau - Kuning - Merah) secara bergantian dan otomatis. ⚙️

📊 Fitur utama dari proyek ini:

🧠 Pemrograman berbasis Instruction List (IL) & Instruction List with Comment (ILC) — untuk efisiensi dan keterbacaan program.

🔍 Fungsi PLC yang digunakan:

🔹 @MOV – Memindahkan data satu kali hanya saat kondisi berubah ke ON (edge trigger), digunakan untuk perubahan nilai awal saat perpindahan state.
🔹 MOV – Memindahkan data secara kontinyu selama kondisi ON, cocok untuk update nilai waktu atau status.
🔹 <=D – Mengecek apakah waktu saat ini masih dalam durasi hijau atau kuning (kurang dari atau sama dengan batas waktu).
🔹 >=D – Mengecek kapan waktu sudah melebihi batas dan siap berpindah ke fase selanjutnya.
🔹 @-- – Mengurangi nilai counter hanya saat perubahan sinyal, efektif untuk countdown satu kali dalam tiap fase.
🔹 IL & ILC – Memudahkan debugging, dokumentasi, dan pemahaman logika dalam bentuk baris instruksi seperti bahasa rakitan.

⏱️ Setiap lampu dikendalikan secara presisi, menjamin sinkronisasi antar ruas dan efisiensi lalu lintas dalam simulasi.
