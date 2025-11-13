<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Webwerk for you - Modernes Webdesign für Anwälte & Praxen</title>
    <!-- Lädt Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Lädt die Inter-Schriftart -->
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap');
        body {
            font-family: 'Inter', sans-serif;
        }
    </style>
    <!-- Konfiguration für Tailwind (optional, aber gut für's Design) -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        'primary': '#0a2342', // Ein tiefes, seriöses Blau
                        'secondary': '#2ca58d', // Ein vertrauenswürdiges Türkis/Grün
                        'light-bg': '#f7f9fc',
                    },
                },
            },
        }
    </script>
</head>
<body class="bg-white text-gray-800">

    <!-- Header / Navigation -->
    <header class="bg-white shadow-sm sticky top-0 z-50">
        <nav class="container mx-auto px-6 py-4 flex justify-between items-center">
            <div>
                <!-- Logo / Name -->
                <a href="#" class="text-2xl font-bold text-primary">Webwerk for you</a>
            </div>
            <!-- Mobile Menu Button (einfach) -->
             <div class="md:hidden">
                <button class="text-gray-800" onclick="toggleMenu()">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path></svg>
                </button>
            </div>
            <!-- Desktop Menu -->
            <div class="hidden md:flex space-x-6">
                <a href="#leistungen" class="text-gray-600 hover:text-primary transition duration-300">Leistungen</a>
                <a href="#ueber-uns" class="text-gray-600 hover:text-primary transition duration-300">Über Uns</a>
                <a href="#kontakt" class="bg-secondary text-white px-4 py-2 rounded-lg hover:opacity-90 transition duration-300">Kostenlose Beratung</a>
            </div>
        </nav>
        <!-- Mobile Menu (versteckt) -->
        <div id="mobile-menu" class="hidden md:hidden px-6 pb-4 space-y-2">
            <a href="#leistungen" class="block text-gray-600 hover:text-primary transition duration-300">Leistungen</a>
            <a href="#ueber-uns" class="block text-gray-600 hover:text-primary transition duration-300">Über Uns</a>
            <a href="#kontakt" class="block bg-secondary text-white px-4 py-2 rounded-lg hover:opacity-90 transition duration-300">Kostenlose Beratung</a>
        </div>
    </header>

    <!-- Hero Sektion -->
    <main>
        <section class="bg-light-bg">
            <div class="container mx-auto px-6 py-20 md:py-32 text-center">
                <h1 class="text-4xl md:text-6xl font-bold text-primary mb-4">Digitale Präsenz für Ihre Kanzlei</h1>
                <p class="text-lg md:text-xl text-gray-700 max-w-3xl mx-auto mb-8">Wir erstellen moderne, seriöse und mobil-optimierte Websites für Anwälte, Notare und Praxen.</p>
                <div>
                    <a href="#kontakt" class="bg-secondary text-white text-lg px-8 py-3 rounded-lg hover:opacity-90 transition duration-300 shadow-lg">Jetzt kostenlose Erstberatung anfordern</a>
                </div>
            </div>
        </section>

        <!-- Leistungen (Services) Sektion -->
        <section id="leistungen" class="py-20">
            <div class="container mx-auto px-6">
                <h2 class="text-3xl md:text-4xl font-bold text-center text-primary mb-12">Unsere Leistungen für Ihren Erfolg</h2>
                <div class="grid md:grid-cols-3 gap-8">
                    
                    <!-- Leistung 1 -->
                    <div class="bg-white p-8 rounded-lg shadow-lg border border-gray-100">
                        <!-- Icon -->
                        <svg class="w-12 h-12 text-secondary mb-4" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.75 17L9 20l-1 1h8l-1-1-.75-3M3 13h18M5 17h14a2 2 0 002-2V5a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path></svg>
                        <h3 class="text-2xl font-bold text-primary mb-3">Professionelles Webdesign</h3>
                        <p class="text-gray-600">Seriöses, klares Design, das Vertrauen schafft und Ihre Kompetenz unterstreicht. Perfekt zugeschnitten auf Kanzleien und Praxen.</p>
                    </div>

                    <!-- Leistung 2 -->
                    <div class="bg-white p-8 rounded-lg shadow-lg border border-gray-100">
                        <!-- Icon -->
                        <svg class="w-12 h-12 text-secondary mb-4" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 18h.01M8 21h8a2 2 0 002-2V5a2 2 0 00-2-2H8a2 2 0 00-2 2v14a2 2 0 002 2z"></path></svg>
                        <h3 class="text-2xl font-bold text-primary mb-3">Responsive Design</h3>
                        <p class="text-gray-600">Perfekte Darstellung auf allen Geräten – vom Smartphone bis zum Desktop. Essentiell für Mandanten, die mobil suchen.</p>
                    </div>

                    <!-- Leistung 3 -->
                    <div class="bg-white p-8 rounded-lg shadow-lg border border-gray-100">
                        <!-- Icon -->
                        <svg class="w-12 h-12 text-secondary mb-4" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 16h-1v-4h-1m1-4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path></svg>
                        <h3 class="text-2xl font-bold text-primary mb-3">Sichtbarkeit & SEO</h3>
                        <p class="text-gray-600">Wir sorgen dafür, dass Sie bei Google gefunden werden, wenn potenzielle Mandanten nach Ihren Fachgebieten suchen.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Über Uns Sektion -->
        <section id="ueber-uns" class="bg-light-bg py-20">
            <div class="container mx-auto px-6 md:flex items-center">
                <div class="md:w-1/2 md:pr-12 mb-8 md:mb-0">
                    <h2 class="text-3xl md:text-4xl font-bold text-primary mb-4">Ihr Partner für die digitale Kanzlei</h2>
                    <p class="text-gray-700 text-lg mb-4">
                        Hallo! Ich bin [Dein Name], der Gründer von Webwerk for you. Ich habe mich darauf spezialisiert, Anwälten und Ärzten den Einstieg in die digitale Welt so einfach wie möglich zu machen.
                    </p>
                    <p class="text-gray-700 mb-4">
                        Ich verstehe die Anforderungen Ihrer Branche: Es geht um Vertrauen, Seriosität und Klarheit. Ich übersetze Ihre fachliche Kompetenz in ein modernes digitales Aushängeschild, das neue Mandanten gewinnt.
                    </p>
                    <a href="#kontakt" class="text-secondary font-bold hover:underline">Lassen Sie uns sprechen &rarr;</a>
                </div>
                <div class="md:w-1/2">
                    <!-- Platzhalter-Bild -->
                    <img src="https://placehold.co/600x400/0a2342/f7f9fc?text=Ihr+Foto+hier" alt="Porträt des Freelancers" class="rounded-lg shadow-xl w-full">
                </div>
            </div>
        </section>
        
        <!-- Kontakt Sektion -->
        <section id="kontakt" class="py-20">
            <div class="container mx-auto px-6 text-center">
                <h2 class="text-3xl md:text-4xl font-bold text-primary mb-4">Starten Sie Ihr Projekt</h2>
                <p class="text-lg text-gray-700 max-w-2xl mx-auto mb-8">
                    Bereit, Ihre Kanzlei online zu bringen? Schreiben Sie mir eine E-Mail oder rufen Sie an für eine unverbindliche und kostenlose Erstberatung.
                </p>
                <div class="bg-white p-8 md:p-12 rounded-lg shadow-xl border border-gray-100 max-w-3xl mx-auto">
                    <!-- Simple Kontakt-Info (sicherer als ein Formular am Anfang) -->
                    <p class="text-2xl font-bold text-primary">[Dein Name]</p>
                    <p class="text-xl text-gray-700 mt-2">Webdesign & Digitale Strategie</p>
                    
                    <div class="mt-6 space-y-4">
                        <p class="text-lg">
                            <span class="font-semibold">E-Mail:</span> 
                            <a href="mailto:info@deine-domain.de" class="text-secondary hover:underline">info@deine-domain.de</a>
                        </p>
                        <p class="text-lg">
                            <span class="font-semibold">Telefon:</span> 
                            <a href="tel:+49123456789" class="text-secondary hover:underline">0123 / 456 789</a>
                        </p>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="bg-primary text-gray-300 py-12">
        <div class="container mx-auto px-6 text-center">
            <p>&copy; 2025 Webwerk for you. Alle Rechte vorbehalten.</p>
            <div class="mt-4 space-x-6">
                <!-- Diese Links sind rechtlich wichtig in Deutschland! -->
                <a href="#" class="hover:text-white transition duration-300">Impressum</a>
                <a href="#" class="hover:text-white transition duration-300">Datenschutz</a>
            </div>
        </div>
    </footer>

    <!-- JavaScript für das Mobile Menu -->
    <script>
        function toggleMenu() {
            var menu = document.getElementById('mobile-menu');
            if (menu.classList.contains('hidden')) {
                menu.classList.remove('hidden');
            } else {
                menu.classList.add('hidden');
            }
        }
    </script>

</body>
</html>
