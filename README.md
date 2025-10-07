<!DOCTYPE html>
<html>
<head>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Roboto:wght@300;400;700&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
            color: #ffffff;
            font-family: 'Roboto', sans-serif;
            min-height: 100vh;
            overflow-x: hidden;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
        }
        
        /* Header Styles */
        .header {
            text-align: center;
            padding: 4rem 0;
            position: relative;
        }
        
        .glow-text {
            font-family: 'Orbitron', sans-serif;
            font-size: 3.5rem;
            font-weight: 900;
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4, #45b7d1, #96ceb4);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-size: 300% 300%;
            animation: gradient 3s ease infinite;
            margin-bottom: 1rem;
        }
        
        @keyframes gradient {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        
        .subtitle {
            font-size: 1.5rem;
            color: #b8b8b8;
            margin-bottom: 2rem;
        }
        
        .location {
            display: inline-flex;
            align-items: center;
            background: rgba(255, 255, 255, 0.1);
            padding: 0.5rem 1rem;
            border-radius: 25px;
            backdrop-filter: blur(10px);
        }
        
        /* About Section */
        .section {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 2rem;
            margin: 2rem 0;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .section-title {
            font-family: 'Orbitron', sans-serif;
            font-size: 2rem;
            margin-bottom: 1.5rem;
            color: #4ecdc4;
        }
        
        /* Code Block */
        .code-block {
            background: #1e1e1e;
            border-radius: 15px;
            padding: 1.5rem;
            margin: 1rem 0;
            border-left: 4px solid #4ecdc4;
            font-family: 'Courier New', monospace;
        }
        
        .keyword { color: #569cd6; }
        .function { color: #dcdcaa; }
        .string { color: #ce9178; }
        .comment { color: #6a9955; }
        .variable { color: #9cdcfe; }
        
        /* Tech Stack */
        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
            margin-top: 1.5rem;
        }
        
        .tech-category h3 {
            color: #ff6b6b;
            margin-bottom: 1rem;
            font-family: 'Orbitron', sans-serif;
        }
        
        .tech-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
        }
        
        .tech-tag {
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
            padding: 0.5rem 1rem;
            border-radius: 20px;
            font-size: 0.9rem;
            font-weight: bold;
        }
        
        /* Stats */
        .stats-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }
        
        .stat-card {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 15px;
            padding: 1.5rem;
            text-align: center;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        
        /* Contact */
        .contact-links {
            display: flex;
            justify-content: center;
            gap: 2rem;
            margin-top: 2rem;
        }
        
        .contact-btn {
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            padding: 1rem 2rem;
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
            border-radius: 50px;
            text-decoration: none;
            color: white;
            font-weight: bold;
            transition: transform 0.3s ease;
        }
        
        .contact-btn:hover {
            transform: translateY(-5px);
        }
        
        /* Floating Elements */
        .floating {
            animation: float 6s ease-in-out infinite;
        }
        
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
            100% { transform: translateY(0px); }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header -->
        <header class="header floating">
            <h1 class="glow-text">💫 Yashitha Malan</h1>
            <p class="subtitle">Full Stack Developer | AI & Software Engineer | Tech Innovator</p>
            <div class="location">
                <span>📍 Sri Lanka 🇱🇰</span>
            </div>
        </header>

        <!-- About Section -->
        <section class="section">
            <h2 class="section-title">🚀 About Me</h2>
            <div class="code-block">
                <span class="keyword">class</span> <span class="function">YashithaMalan</span> {<br>
                &nbsp;&nbsp;<span class="keyword">constructor</span>() {<br>
                &nbsp;&nbsp;&nbsp;&nbsp;<span class="variable">this</span>.<span class="function">name</span> = <span class="string">"Yashitha Malan"</span>;<br>
                &nbsp;&nbsp;&nbsp;&nbsp;<span class="variable">this</span>.<span class="function">title</span> = <span class="string">"Full Stack & AI Engineer"</span>;<br>
                &nbsp;&nbsp;&nbsp;&nbsp;<span class="variable">this</span>.<span class="function">education</span> = <span class="string">"Bachelor of Information Technology"</span>;<br>
                &nbsp;&nbsp;&nbsp;&nbsp;<span class="variable">this</span>.<span class="function">focus</span> = <span class="string">"Advanced AI and Software Engineering"</span>;<br>
                &nbsp;&nbsp;}<br>
                &nbsp;&nbsp;<span class="function">currentMission</span>() {<br>
                &nbsp;&nbsp;&nbsp;&nbsp;<span class="keyword">return</span> <span class="string">"Building the future with code and artificial intelligence"</span>;<br>
                &nbsp;&nbsp;}<br>
                }
            </div>
        </section>

        <!-- Tech Stack -->
        <section class="section">
            <h2 class="section-title">🛠️ Tech Arsenal</h2>
            <div class="tech-grid">
                <div class="tech-category">
                    <h3>💻 Languages</h3>
                    <div class="tech-tags">
                        <span class="tech-tag">C</span>
                        <span class="tech-tag">Python</span>
                        <span class="tech-tag">JavaScript</span>
                        <span class="tech-tag">Dart</span>
                    </div>
                </div>
                <div class="tech-category">
                    <h3>🎯 Frameworks</h3>
                    <div class="tech-tags">
                        <span class="tech-tag">Django</span>
                        <span class="tech-tag">Flask</span>
                        <span class="tech-tag">Node.js</span>
                        <span class="tech-tag">Flutter</span>
                    </div>
                </div>
                <div class="tech-category">
                    <h3>🗄️ Databases & Tools</h3>
                    <div class="tech-tags">
                        <span class="tech-tag">MySQL</span>
                        <span class="tech-tag">Git</span>
                        <span class="tech-tag">GitHub</span>
                    </div>
                </div>
            </div>
        </section>

        <!-- GitHub Stats -->
        <section class="section">
            <h2 class="section-title">📊 GitHub Analytics</h2>
            <div class="stats-container">
                <div class="stat-card">
                    <h3>Profile Views</h3>
                    <img src="https://komarev.com/ghpvc/?username=yashithamalan&label=Profile+Views&color=blue&style=for-the-badge" alt="Profile Views">
                </div>
                <div class="stat-card">
                    <h3>GitHub Stats</h3>
                    <img src="https://github-readme-stats.vercel.app/api?username=yashithamalan&show_icons=true&theme=radical&hide_border=true" alt="GitHub Stats" style="width: 100%;">
                </div>
                <div class="stat-card">
                    <h3>Top Languages</h3>
                    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=yashithamalan&layout=compact&theme=radical&hide_border=true" alt="Top Languages" style="width: 100%;">
                </div>
            </div>
        </section>

        <!-- Contact -->
        <section class="section">
            <h2 class="section-title">📬 Let's Connect</h2>
            <div style="text-align: center;">
                <p style="margin-bottom: 2rem; font-size: 1.2rem;">Ready to bring your ideas to life? Let's create something amazing together! ✨</p>
                <div class="contact-links">
                    <a href="mailto:yashithamalan@gmail.com" class="contact-btn">
                        📧 Email Me
                    </a>
                    <a href="https://facebook.com/yashithamalan" class="contact-btn">
                        📱 Facebook
                    </a>
                </div>
            </div>
        </section>

        <!-- Footer -->
        <footer style="text-align: center; margin-top: 4rem; padding: 2rem; color: #888;">
            <p>🚀 Built with passion and code | 💫 Yashitha Malan © 2024</p>
        </footer>
    </div>

    <script>
        // Add floating animation to multiple elements
        document.addEventListener('DOMContentLoaded', function() {
            const elements = document.querySelectorAll('.section');
            elements.forEach((element, index) => {
                element.style.animationDelay = `${index * 0.2}s`;
                element.classList.add('floating');
            });
        });
    </script>
</body>
</html>