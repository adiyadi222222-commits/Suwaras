<!DOCTYPE html>
<html lang="id" class="dark">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Portfolio Premium Bebbb</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    // Dark/Light mode toggle
    function toggleTheme() {
      document.documentElement.classList.toggle('dark');
      localStorage.setItem('theme', document.documentElement.classList.contains('dark') ? 'dark' : 'light');
    }
    // Load theme dari localStorage
    if (localStorage.getItem('theme') === 'light') {
      document.documentElement.classList.remove('dark');
    }
  </script>
</head>
<body class="bg-gray-50 dark:bg-gray-900 text-gray-800 dark:text-gray-100 font-sans transition-colors duration-500">

  <!-- Navbar -->
  <nav class="fixed w-full bg-white/70 dark:bg-gray-800/70 backdrop-blur-md shadow-md z-50">
    <div class="container mx-auto flex justify-between items-center p-4">
      <h1 class="text-2xl font-bold text-pink-500">Bebbb</h1>
      <div class="space-x-6">
        <a href="#about" class="hover:text-pink-500">Tentang</a>
        <a href="#projects" class="hover:text-pink-500">Project</a>
        <a href="#contact" class="hover:text-pink-500">Kontak</a>
        <button onclick="toggleTheme()" class="px-3 py-1 rounded-lg bg-gray-200 dark:bg-gray-700 hover:bg-pink-500 hover:text-white transition">
          🌙/☀️
        </button>
      </div>
    </div>
  </nav>

  <!-- Hero Section -->
  <section class="h-screen flex flex-col justify-center items-center text-center px-4">
    <h2 class="text-5xl md:text-6xl font-extrabold mb-4 animate-bounce">
      Halo, aku <span class="text-pink-500">Bebbb</span> 👋
    </h2>
    <p class="text-lg md:text-xl text-gray-600 dark:text-gray-300 max-w-2xl">
      Web developer gratisan, open source lover, dan penikmat ngulik hal-hal baru 🚀
    </p>
    <a href="#projects" class="mt-8 px-8 py-3 bg-pink-500 text-white rounded-full shadow-lg hover:scale-110 transform transition">
      ✨ Lihat Project
    </a>
  </section>

  <!-- About -->
  <section id="about" class="py-20 container mx-auto px-6 text-center">
    <h3 class="text-3xl font-bold mb-6">Tentang Aku</h3>
    <p class="max-w-3xl mx-auto text-gray-700 dark:text-gray-300 leading-relaxed">
      Aku suka berbagi dan belajar dari dunia open source. Dari script kecil sampai project gede, 
      semua aku simpen di GitHub biar bermanfaat buat kaum gretongan 💎. 
      Web ini aku buat biar orang lain bisa lihat karya-karyaku dengan tampilan elegan premium 😍.
    </p>
  </section>

  <!-- Projects -->
  <section id="projects" class="py-20 bg-gray-100 dark:bg-gray-800">
    <div class="container mx-auto px-6">
      <h3 class="text-3xl font-bold mb-10 text-center">Project Keren</h3>
      <div class="grid md:grid-cols-3 gap-10">
        
        <!-- Card -->
        <div class="bg-white dark:bg-gray-700 rounded-2xl p-6 shadow-lg hover:shadow-2xl transform hover:-translate-y-2 transition">
          <h4 class="text-xl font-bold mb-2 text-pink-500">🌐 Website Gratis</h4>
          <p class="text-gray-600 dark:text-gray-300">Portfolio & blog pribadi yang di-host di GitHub Pages.</p>
        </div>

        <div class="bg-white dark:bg-gray-700 rounded-2xl p-6 shadow-lg hover:shadow-2xl transform hover:-translate-y-2 transition">
          <h4 class="text-xl font-bold mb-2 text-pink-500">🤖 Bot Telegram</h4>
          <p class="text-gray-600 dark:text-gray-300">Bot untuk reply otomatis & hunting info gratisan.</p>
        </div>

        <div class="bg-white dark:bg-gray-700 rounded-2xl p-6 shadow-lg hover:shadow-2xl transform hover:-translate-y-2 transition">
          <h4 class="text-xl font-bold mb-2 text-pink-500">📊 Data Scraper</h4>
          <p class="text-gray-600 dark:text-gray-300">Script buat ambil data dari web publik secara otomatis.</p>
        </div>

      </div>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact" class="py-20 container mx-auto px-6 text-center">
    <h3 class="text-3xl font-bold mb-6">Kontak Aku</h3>
    <p class="text-gray-600 dark:text-gray-300 mb-8">Kalau mau collab, silakan hubungi aku lewat:</p>
    <div class="space-x-4">
      <a href="mailto:emailbebbb@example.com" class="px-6 py-3 bg-pink-500 text-white rounded-full shadow hover:scale-110 transition">Email</a>
      <a href="https://github.com/username" target="_blank" class="px-6 py-3 bg-gray-300 dark:bg-gray-600 rounded-full hover:bg-pink-500 hover:text-white shadow transition">GitHub</a>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-white dark:bg-gray-800 py-6 text-center text-gray-500 dark:text-gray-400">
    © 2025 Bebbb. Dibuat dengan 💖 & GitHub Pages.
  </footer>

</body>
</html>
