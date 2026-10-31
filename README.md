
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Selamat Ulang Tahun Ke-18 Vincent Jap!</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Canvas Confetti -->
    <script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.6.0/dist/confetti.browser.min.js"></script>
    <!-- Google Fonts: Poppins & Pacifico -->
    <link href="https://fonts.googleapis.com/css2?family=Pacifico&family=Poppins:wght@300;400;600;700;800&display=swap" rel="stylesheet">
    
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #0f172a 0%, #1e1b4b 50%, #311042 100%);
            min-height: 100vh;
            color: #f8fafc;
            overflow-x: hidden;
        }
        .font-cursive {
            font-family: 'Pacifico', cursive;
        }
        .glass-card {
            background: rgba(255, 255, 255, 0.07);
            backdrop-filter: blur(16px);
            -webkit-backdrop-filter: blur(16px);
            border: 1px solid rgba(255, 255, 255, 0.15);
            box-shadow: 0 20px 50px rgba(0, 0, 0, 0.4);
        }
        .glow-effect {
            box-shadow: 0 0 25px rgba(236, 72, 153, 0.5), 0 0 50px rgba(168, 85, 247, 0.3);
        }
        .gold-gradient-text {
            background: linear-gradient(135deg, #ffe259 0%, #ffa751 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        .animated-gradient-text {
            background: linear-gradient(270deg, #ff7eb3, #ff758c, #70a1ff, #00c6ff);
            background-size: 300% 300%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: gradientMove 6s ease infinite;
        }
        @keyframes gradientMove {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        .floating {
            animation: floating 3s ease-in-out infinite;
        }
        @keyframes floating {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }
    </style>
</head>
<body class="flex items-center justify-center p-4 md:p-8 relative">

    <!-- Ambient Background Elements -->
    <div class="fixed top-10 left-10 w-72 h-72 bg-purple-600/30 rounded-full blur-3xl pointer-events-none"></div>
    <div class="fixed bottom-10 right-10 w-80 h-80 bg-pink-600/30 rounded-full blur-3xl pointer-events-none"></div>
    
    <!-- Main Card Container -->
    <div class="glass-card w-full max-w-2xl rounded-3xl p-6 sm:p-10 text-center relative z-10 transition-all duration-500 my-auto">
        
        <!-- Header Badge -->
        <div class="inline-flex items-center gap-2 px-4 py-1.5 rounded-full bg-gradient-to-r from-pink-500/20 to-purple-500/20 border border-pink-500/30 text-pink-300 text-sm font-semibold mb-6 floating">
            <i class="fa-solid fa-cake-candles"></i> Official 18th Birthday Celebration
        </div>

        <!-- Birthday Title -->
        <h1 class="text-3xl sm:text-5xl font-extrabold tracking-tight mb-2">
            HAPPY <span class="gold-gradient-text">18TH</span> BIRTHDAY!
        </h1>
        <h2 class="text-2xl sm:text-4xl font-bold font-cursive animated-gradient-text mb-6">
            Vincent Jap 🎉
        </h2>

        <!-- Photo Container -->
        <div class="relative w-48 h-48 sm:w-60 sm:h-60 mx-auto mb-8 group">
            <div class="absolute inset-0 bg-gradient-to-tr from-yellow-400 via-pink-500 to-purple-600 rounded-full glow-effect animate-spin" style="animation-duration: 12s;"></div>
            <div class="absolute inset-1.5 bg-slate-900 rounded-full overflow-hidden border-4 border-white/20">
                <!-- User Photo Placeholder / Embed -->
                <img src="vj.png" 
                     alt="Vincent Jap" 
                     class="w-full h-full object-cover object-top transition duration-500 group-hover:scale-110"
                     onerror="this.onerror=null; this.src='https://placehold.co/600x600/1e1b4b/ffffff?text=Vincent+Jap';">
            </div>
            <!-- 18 Badge -->
            <div class="absolute -bottom-2 -right-2 bg-gradient-to-r from-amber-400 to-amber-600 text-slate-950 font-black text-xl sm:text-2xl w-14 h-14 rounded-full flex items-center justify-center shadow-lg border-2 border-white">
                18
            </div>
        </div>

        <!-- Custom Birthday Wishes Message -->
        <div class="bg-slate-900/50 rounded-2xl p-5 sm:p-6 mb-8 border border-white/10 text-slate-200 text-sm sm:text-base leading-relaxed text-left sm:text-center shadow-inner">
            <p class="mb-3">
                ✨ <strong class="text-amber-300">Selamat Memasuki Usia Dewasa, Vincent!</strong> ✨
            </p>
            <p class="mb-3">
                Selamat ulang tahun yang ke-18! Di usia yang baru ini, semoga langkahmu semakin mantap, diberikan kesehatan, kebahagiaan, dan keberhasilan dalam setiap impian serta cita-cita yang kamu perjuangkan.
            </p>
            <p class="text-slate-400 italic text-xs sm:text-sm">
                "Nikmati setiap prosesnya, kejar petualangan baru, dan jadilah versi terbaik dari dirimu sendiri!"
            </p>
        </div>

        <!-- Interactive Action Buttons -->
        <div class="flex flex-wrap items-center justify-center gap-4">
            <!-- Confetti Button -->
            <button id="confettiBtn" onclick="triggerConfetti()" class="px-6 py-3 rounded-full bg-gradient-to-r from-pink-500 to-rose-600 text-white font-semibold shadow-lg hover:from-pink-600 hover:to-rose-700 hover:scale-105 active:scale-95 transition-all duration-200 flex items-center gap-2">
                <i class="fa-solid fa-gift"></i>
                <span>Rayakan! 🎉</span>
            </button>

            <!-- Sound/Song Toggle Button -->
            <button id="musicBtn" onclick="toggleMusic()" class="px-6 py-3 rounded-full bg-gradient-to-r from-purple-500 to-indigo-600 text-white font-semibold shadow-lg hover:from-purple-600 hover:to-indigo-700 hover:scale-105 active:scale-95 transition-all duration-200 flex items-center gap-2">
                <i id="musicIcon" class="fa-solid fa-music"></i>
                <span id="musicText">Putar Musik 🎵</span>
            </button>

            <!-- Share / Copy Wish Button -->
            <button onclick="copyWishes()" class="px-6 py-3 rounded-full bg-slate-800 hover:bg-slate-700 border border-white/20 text-white font-semibold shadow-lg hover:scale-105 active:scale-95 transition-all duration-200 flex items-center gap-2">
                <i class="fa-solid fa-share-nodes"></i>
                <span>Bagikan Ucapan</span>
            </button>
        </div>

        <!-- Footer -->
        <div class="mt-8 text-xs text-slate-400 border-t border-white/10 pt-4 flex justify-between items-center px-2">
            <span>Special wishes for Vincent Jap</span>
            <span class="text-pink-400 font-semibold">18th Birthday Edition 🎈</span>
        </div>

    </div>

    <!-- Notification Toast -->
    <div id="toast" class="fixed bottom-6 bg-emerald-600 text-white px-5 py-3 rounded-xl shadow-2xl transition-all duration-300 opacity-0 transform translate-y-10 pointer-events-none z-50 flex items-center gap-2 font-medium">
        <i class="fa-solid fa-circle-check"></i>
        <span id="toastMsg">Pesan berhasil disalin!</span>
    </div>

    <!-- Audio Element (Synthesized/Web Audio API synth fallback for smooth playback) -->
    <script>
        // Trigger Confetti on Load
        window.addEventListener('load', () => {
            setTimeout(() => {
                triggerConfetti();
            }, 500);
        });

        // Confetti Fireworks Function
        function triggerConfetti() {
            var count = 200;
            var defaults = {
                origin: { y: 0.7 }
            };

            function fire(particleRatio, opts) {
                confetti(Object.assign({}, defaults, opts, {
                    particleCount: Math.floor(count * particleRatio)
                }));
            }

            fire(0.25, {
                spread: 26,
                startVelocity: 55,
            });
            fire(0.2, {
                spread: 60,
            });
            fire(0.35, {
                spread: 100,
                decay: 0.91,
                scalar: 0.8
            });
            fire(0.1, {
                spread: 120,
                startVelocity: 25,
                decay: 0.92,
                scalar: 1.2
            });
            fire(0.1, {
                spread: 120,
                startVelocity: 45,
            });
        }

        // Web Audio API Synthesizer for Happy Birthday Melody
        let isPlaying = false;
        let audioCtx = null;
        let activeNodes = [];

        function toggleMusic() {
            const musicIcon = document.getElementById('musicIcon');
            const musicText = document.getElementById('musicText');

            if (!isPlaying) {
                playHappyBirthdayMelody();
                isPlaying = true;
                musicIcon.className = 'fa-solid fa-pause';
                musicText.innerText = 'Jeda Musik ⏸️';
                showToast('🎶 Menyanyikan lagu Selamat Ulang Tahun!');
            } else {
                stopMusic();
                isPlaying = false;
                musicIcon.className = 'fa-solid fa-music';
                musicText.innerText = 'Putar Musik 🎵';
            }
        }

        function playHappyBirthdayMelody() {
            if (!audioCtx) {
                audioCtx = new (window.AudioContext || window.webkitAudioContext)();
            }

            const notes = [
                { note: 261.63, duration: 0.4 }, // C4
                { note: 261.63, duration: 0.4 }, // C4
                { note: 293.66, duration: 0.8 }, // D4
                { note: 261.63, duration: 0.8 }, // C4
                { note: 349.23, duration: 0.8 }, // F4
                { note: 329.63, duration: 1.2 }, // E4

                { note: 261.63, duration: 0.4 }, // C4
                { note: 261.63, duration: 0.4 }, // C4
                { note: 293.66, duration: 0.8 }, // D4
                { note: 261.63, duration: 0.8 }, // C4
                { note: 392.00, duration: 0.8 }, // G4
                { note: 349.23, duration: 1.2 }, // F4

                { note: 261.63, duration: 0.4 }, // C4
                { note: 261.63, duration: 0.4 }, // C4
                { note: 523.25, duration: 0.8 }, // C5
                { note: 440.00, duration: 0.8 }, // A4
                { note: 349.23, duration: 0.8 }, // F4
                { note: 329.63, duration: 0.8 }, // E4
                { note: 293.66, duration: 1.2 }, // D4

                { note: 466.16, duration: 0.4 }, // Bb4
                { note: 466.16, duration: 0.4 }, // Bb4
                { note: 440.00, duration: 0.8 }, // A4
                { note: 349.23, duration: 0.8 }, // F4
                { note: 392.00, duration: 0.8 }, // G4
                { note: 349.23, duration: 1.6 }  // F4
            ];

            let currentTime = audioCtx.currentTime + 0.1;

            notes.forEach((item) => {
                const osc = audioCtx.createOscillator();
                const gain = audioCtx.createGain();

                osc.type = 'triangle';
                osc.frequency.setValueAtTime(item.note, currentTime);

                gain.gain.setValueAtTime(0.3, currentTime);
                gain.gain.exponentialRampToValueAtTime(0.001, currentTime + item.duration - 0.05);

                osc.connect(gain);
                gain.connect(audioCtx.destination);

                osc.start(currentTime);
                osc.stop(currentTime + item.duration);

                activeNodes.push(osc);
                currentTime += item.duration;
            });

            // Loop option
            const totalDuration = notes.reduce((acc, curr) => acc + curr.duration, 0);
            setTimeout(() => {
                if (isPlaying) {
                    playHappyBirthdayMelody();
                }
            }, totalDuration * 1000);
        }

        function stopMusic() {
            if (audioCtx) {
                audioCtx.close();
                audioCtx = null;
            }
        }

        // Copy Wish Text
        function copyWishes() {
            const textToCopy = `🎉 Selamat Ulang Tahun Ke-18, Vincent Jap! 🥳\nSemoga di usia dewasa ini semakin sukses, sehat selalu, dan tercapai semua impiannya! ✨`;
            
            // Clipboard Fallback
            const dummy = document.createElement("textarea");
            document.body.appendChild(dummy);
            dummy.value = textToCopy;
            dummy.select();
            document.execCommand("copy");
            document.body.removeChild(dummy);

            showToast('Ucapan ulang tahun berhasil disalin!');
        }

        // Show Toast Notification
        function showToast(message) {
            const toast = document.getElementById('toast');
            const toastMsg = document.getElementById('toastMsg');
            toastMsg.innerText = message;
            
            toast.classList.remove('opacity-0', 'translate-y-10');
            toast.classList.add('opacity-100', 'translate-y-0');

            setTimeout(() => {
                toast.classList.remove('opacity-100', 'translate-y-0');
                toast.classList.add('opacity-0', 'translate-y-10');
            }, 3000);
        }
    </script>

