<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Selamat Ulang Tahun, Muhammad Alfan!</title>
     <img src="apan2.jpg" alt="Muhammad Alfan Ersianov Firdaus Sukandar" class="profile-photo">
    <style>
        /* Latar belakang gradient */
        body {
            background: linear-gradient(135deg, #ffefba, #ffffff);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 0;
            font-family: 'Comic Sans MS', cursive, sans-serif;
            overflow: hidden;
        }

        /* Container untuk halaman */
        .birthday-container {
            background-color: #fff;
            padding: 40px;
            border-radius: 15px;
            text-align: center;
            box-shadow: 0px 8px 15px rgba(0, 0, 0, 0.3);
            position: relative;
            overflow: hidden;
        }

        /* Gaya untuk kue ulang tahun */
        .cake {
            width: 200px;
            margin: 0 auto;
            position: relative;
        }

        .cake img {
            width: 100%;
            border-radius: 15px;
        }

        /* Balon animasi */
        .balloon {
            position: absolute;
            bottom: -100px; /* Awalnya di luar tampilan */
            animation: fly 6s linear infinite;
            width: 80px;
        }

        @keyframes fly {
            0% {
                bottom: -100px; /* Mulai dari bawah */
                opacity: 1;
            }
            50% {
                opacity: 1;
                transform: translateY(-200px); /* Naik */
            }
            100% {
                bottom: -100px; /* Kembali di luar tampilan */
                opacity: 0; /* Memudar */
            }
        }

        /* Gaya tombol dan pesan */
        .btn-surprise {
            margin-top: 20px;
            font-size: 1.2rem;
        }

        .hidden-message {
            display: none;
            margin-top: 20px;
            animation: fadeIn 2s forwards;
        }

        @keyframes fadeIn {
            0% {
                opacity: 0;
            }
            100% {
                opacity: 1;
            }
        }

        /* Lilin yang berkedip */
        .candle-flame {
            position: absolute;
            top: -30px;
            left: 50%;
            transform: translateX(-50%);
            width: 20px;
            height: 40px;
            background-color: orange;
            border-radius: 50%;
            animation: flicker 0.5s alternate infinite;
        }

        @keyframes flicker {
            0% {
                opacity: 1;
                transform: scale(1);
            }
            50% {
                opacity: 0.8;
                transform: scale(1.2);
            }
            100% {
                opacity: 1;
                transform: scale(1);
            }
        }
    </style>
</head>
<body>
    <div class="birthday-container">
        <!-- Kue ulang tahun -->
        <div class="cake">
            <div class="candle-flame"></div>
            <img src="https://i.imgur.com/4N6OTmD.png" alt="Kue Ulang Tahun">
        </div>

        <!-- Pesan Ucapan -->
        <h1 class="fw-bold mt-4">Selamat Ulang Tahun, Alfan!</h1>
        <h3 class="fw-light">Semoga semua impianmu terwujud 🎂</h3>

        <!-- Tombol Kejutan -->
        <button id="surpriseButton" class="btn btn-primary btn-surprise">Open Your Surprise!!</button>

        <!-- Pesan kejutan tersembunyi -->
        <div id="surpriseMessage" class="hidden-message">
            <h2>🎉 Kejutan Spesial untuk Alfan! 🎉</h2>
            <p>Semoga hari-harimu selalu dipenuhi dengan tawa, cinta, dan kebahagiaan! 🎈</p>
        </div>

        <!-- Balon animasi -->
        <div class="balloons">
            <img src="https://i.imgur.com/KJXmDnF.png" alt="Balon" class="balloon" style="left: 10%;">
            <img src="https://i.imgur.com/KJXmDnF.png" alt="Balon" class="balloon" style="left: 40%;">
            <img src="https://i.imgur.com/KJXmDnF.png" alt="Balon" class="balloon" style="left: 70%;">
        </div>
    </div>

    <script>
        // Menampilkan pesan kejutan saat tombol diklik
        document.getElementById('surpriseButton').addEventListener('click', function() {
            var surpriseMessage = document.getElementById('surpriseMessage');
            surpriseMessage.style.display = 'block'; // Menampilkan pesan kejutan
        });
    </script>
</body>
</html>
