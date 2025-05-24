# portofolio

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Wahyu Andika - IT Professional Portfolio</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap');

        /* Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background: #f4f4f4;
            color: #333;
            line-height: 1.6;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            overflow-x: hidden;
        }

        header {
            background-color: #007acc;
            padding: 2rem 1.5rem;
            text-align: center;
            color: white;
            animation: fadeIn 1s ease-in;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        header h1 {
            font-size: 3rem;
            font-weight: 700;
            margin-bottom: 0.5rem;
        }

        header p {
            font-weight: 300;
            font-size: 1.2rem;
        }

        main {
            flex-grow: 1;
            max-width: 900px;
            margin: 2rem auto;
            padding: 0 1rem;
        }

        section {
            margin-bottom: 3rem;
            background-color: white;
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            opacity: 0;
            transform: translateY(20px);
            animation: slideIn 0.5s forwards;
        }

        @keyframes slideIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        section h2 {
            font-weight: 700;
            font-size: 2rem;
            margin-bottom: 1rem;
            color: #007acc;
        }

        .projects-list {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 1.5rem;
        }

        .project-card {
            background: #e9ecef;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            opacity: 0;
            transform: translateY(20px);
            animation: fadeInUp 0.5s forwards;
        }

        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.2);
        }

        .project-image {
            width: 100%;
            height: 160px;
            object-fit: cover;
        }

        .project-info {
            padding: 1rem;
        }

        .project-info h3 {
            color: #007acc;
            margin-bottom: 0.5rem;
        }

        .skills-list {
            display: flex;
            flex-wrap: wrap;
            gap: 1rem;
        }

        .skill {
            background: #007acc;
            color: white;
            font-weight: 600;
            padding: 0.5rem 1rem;
            border-radius: 20px;
            transition: background 0.3s ease;
        }

        .skill:hover {
            background: #005fa3;
        }

        .contact {
            text-align: center;
        }

        .contact p {
            margin-bottom: 1rem;
            font-size: 1.1rem;
        }

        .contact a {
            color: #007acc;
            text-decoration: none;
            font-weight: 700;
            transition: color 0.3s ease;
        }

        .contact a:hover {
            color: #005fa3;
        }

        footer {
            text-align: center;
            padding: 1rem 0;
            background: #007acc;
            color: white;
            font-weight: 500;
            font-size: 0.9rem;
        }

        /* Responsive for Laptop */
        @media (max-width: 1024px) {
            header h1 {
                font-size: 2.5rem;
            }

            section h2 {
                font-size: 1.8rem;
            }
        }

        /* Responsive for Mobile */
        @media (max-width: 480px) {
            header h1 {
                font-size: 2rem;
            }

            section h2 {
                font-size: 1.5rem;
            }

            .projects-list {
                grid-template-columns: 1fr;
            }

            header {
                padding: 1.5rem 1rem;
            }

            main {
                margin: 1rem auto;
                padding: 0 1rem;
            }

            section {
                padding: 1.5rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Wahyu Andika</h1>
        <p>IT Professional | Web Developer</p>
        <p>Universitas Pelita Bangsa</p>
    </header>
    <main>
        <section class="about" id="about">
            <h2>Tentang Saya</h2>
            <p>Halo! Saya Wahyu, seorang profesional IT yang bersemangat dalam mengembangkan aplikasi web dan perangkat lunak. Saya memiliki minat yang besar dalam pemrograman, desain, dan teknologi. Dengan pengetahuan yang saya peroleh selama studi, saya berusaha untuk menciptakan solusi yang inovatif dan efisien.</p>
        </section>
        <section class="projects" id="projects">
            <h2>Projects</h2>
            <div class="projects-list">
                <div class="project-card">
                    <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=400&q=80" alt="Project One" class="project-image" />
                    <div class="project-info">
                        <h3>Website Portofolio</h3>
                        <p>Sebuah website portofolio pribadi yang responsif dibangun dengan HTML, CSS, dan JavaScript untuk menampilkan karya dan keterampilan saya.</p>
                    </div>
                </div>
                <div class="project-card">
                    <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?auto=format&fit=crop&w=400&q=80" alt="Project Two" class="project-image" />
                    <div class="project-info">
                        <h3>Aplikasi E-commerce</h3>
                        <p>Sebuah aplikasi web e-commerce yang dibangun dengan Node.js dan MongoDB, dilengkapi dengan autentikasi pengguna dan sistem pembayaran.</p>
                    </div>
                </div>
                <div class="project-card">
                    <img src="https://images.unsplash.com/photo-1486312338219-ce68d2c6f44d?auto=format&fit=crop&w=400&q=80" alt="Project Three" class="project-image" />
                    <div class="project-info">
                        <h3>Aplikasi Manajemen Tugas</h3>
                        <p>Sebuah aplikasi produktivitas yang dibangun dengan Vue.js dan Firebase untuk membantu pengguna mengatur tugas harian mereka dengan efektif.</p>
                    </div>
                </div>
            </div>
        </section>
        <section class="skills" id="skills">
            <h2>Skills</h2>
            <div class="skills-list">
                <span class="skill">JavaScript</span>
                <span class="skill">React</span>
                <span class="skill">Node.js</span>
                <span class="skill">HTML5</span>
                <span class="skill">CSS3</span>
                <span class="skill">Vue.js</span>
                <span class="skill">MongoDB</span>
                <span class="skill">Git</span>
                <span class="skill">Figma</span>
            </div>
        </section>
        <section class="contact" id="contact">
            <h2>Contact Me</h2>
            <p>Silakan hubungi saya jika Anda ingin berkolaborasi atau sekadar menyapa!</p>
            <p>Email: <a href="mailto:wahyuandika0426@gmail.com" target="_blank" rel="noopener">wahyuandika0426@gmail.com</a></p>
            <p>Telepon: <a href="tel:+6289657613057" target="_blank" rel="noopener">+6289657613057</a></p>
            <p>LinkedIn: <a href="https://www.linkedin.com/in/wahyuandika" target="_blank" rel="noopener">linkedin.com/in/wahyuandika</a></p>
        </section>
    </main>
    <footer>
        &copy; 2025 Wahyu Andika. All rights reserved.
    </footer>
</body>
</html>
