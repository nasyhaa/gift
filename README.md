<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Selamat Ulang Tahun, Muhammad Alfan!</title>
    <!-- Link ke CDN Bootstrap -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        /* Background dengan gradient pastel */
        body {
            background: linear-gradient(135deg, #ffecd2, #fcb69f);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 0;
            font-family: 'Helvetica Neue', sans-serif;
        }

        /* Container untuk keseluruhan kartu ulang tahun */
        .birthday-container {
            background: linear-gradient(135deg, #84fab0, #8fd3f4);
            padding: 40px;
            border-radius: 20px;
            box-shadow: 0 8px 30px rgba(0, 0, 0, 0.2);
            max-width: 600px;
            text-align: center;
            animation: fadeIn 2s ease-in-out;
        }

        /* Gaya untuk foto profil dengan animasi */
        .profile-photo {
            width: 200px;
            height: 200px;
            object-fit: cover;
            margin-bottom: 20px;
            border: 5px solid #fff;
            border-radius: 50%;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            animation: bounce 2s infinite;
        }

        /* Animasi bounce untuk gambar */
        @keyframes bounce {
            0%, 100% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-10px);
            }
        }

        /* Animasi fade-in untuk container */
        @keyframes fadeIn {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }

        /* Tombol dengan gaya modern */
        .btn-surprise {
            background-color: #ff8a65;
            color: white;
            font-size: 18px;
            padding: 10px 20px;
            border: none;
            border-radius: 30px;
            box-shadow: 0 4px 15px rgba(255, 138, 101, 0.4);
            transition: background-color 0.3s ease, transform 0.3s ease;
        }

        .btn-surprise:hover {
            background-color: #ff7043;
            transform: scale(1.05);
        }

        /* Pesan kejutan tersembunyi dengan animasi */
        .hidden {
            display: none;
        }

        #surpriseMessage {
            background-color: #fff3e0;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
            margin-top: 20px;
            animation: fadeIn 1.5s ease-in-out;
        }

        /* Gaya teks untuk ucapan */
        h1 {
            font-size: 36px;
            color: #ffffff;
            font-weight: 700;
            text-shadow: 2px 2px 8px rgba(0, 0, 0, 0.1);
        }

        h2 {
            font-size: 28px;
            color: #ffffff;
            font-weight: 300;
        }

        p {
            font-size: 18px;
            color: #333;
        }
    </style>
</head>
<body>
    <div class="birthday-container">
        <!-- Foto Ulang Tahun -->
        <div class="photo-section" <imgsrc="img/apan 2.jpg" alt="Foto Muhammad Alfan" class="profile-photo">
        </div>
        
        <!-- Nama dan Pesan Ucapan -->
        <div class="message-section mt-4">
            <h2 class="fw-normal">Hari ini, 13 Oktober 2024</h2>
            <h1 class="fw-bold">Selamat Ulang Tahun!</h1>
            <h2 class="fw-light">Muhammad Alfan Ersianov Firdaus Sukandar</h2>
        </div>
        
        <!-- Tombol Kejutan -->
        <button id="surpriseButton" class="btn-surprise mt-4">Open Your Surprise!!</button>
        
        <!-- Pesan Kejutan Tersembunyi -->
        <div id="surpriseMessage" class="hidden mt-4">
            <h3>🎉 Your Gift From Apann! 🎉</h3>
            <p>Terima kasih banyak telah datang di kehidupan nasa ini yaaa. Semoga ulang tahun apann hari ini selalu dipenuhi dengan tawa dan kebahagiaan, pokoknya doa terbaik dari nasa buatt apann terus lewatin semuanyaabarengg barengg yaaa. I Lovee uu acumm sayangg! 😘</p>
        </div>
    </div>

    <script>
        // Menangani event klik pada tombol
        document.getElementById('surpriseButton').addEventListener('click', function() {
            var surpriseMessage = document.getElementById('surpriseMessage');
            surpriseMessage.classList.toggle('hidden'); // Menampilkan atau menyembunyikan pesan kejutan
            this.textContent = surpriseMessage.classList.contains('hidden') ? 'Open Your Surprise!!' : 'Close Your Surprise'; // Mengubah teks tombol
        });
    </script>
</body>
</html>
