<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Super Xandão - O Herói do Brasil</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Oswald:wght@400;700&display=swap');
        
        :root {
            --primary: #FF0000;
            --secondary: #FFD700;
            --dark: #0A0A0A;
        }
        
        body {
            font-family: 'Oswald', sans-serif;
            background-color: var(--dark);
            color: white;
            overflow-x: hidden;
        }
        
        .title-font {
            font-family: 'Bebas Neue', cursive;
        }
        
        .hero-bg {
            background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), 
                        url('https://images.unsplash.com/photo-1543351611-58f69d7c1781?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
        }
        
        .glow {
            text-shadow: 0 0 10px var(--primary), 0 0 20px var(--primary);
        }
        
        .card-hover {
            transition: all 0.3s ease;
        }
        
        .card-hover:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 20px rgba(255, 0, 0, 0.3);
        }
        
        .pulse {
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0% {
                box-shadow: 0 0 0 0 rgba(255, 215, 0, 0.7);
            }
            70% {
                box-shadow: 0 0 0 10px rgba(255, 215, 0, 0);
            }
            100% {
                box-shadow: 0 0 0 0 rgba(255, 215, 0, 0);
            }
        }
    </style>
</head>
<body>
    <!-- Navbar -->
    <nav class="bg-black py-4 sticky top-0 z-50 border-b border-red-600">
        <div class="container mx-auto px-4 flex justify-between items-center">
            <div class="flex items-center">
                <i class="fas fa-shield-alt text-red-600 text-2xl mr-2"></i>
                <span class="title-font text-2xl text-white">SUPER <span class="text-red-600">XANDÃO</span></span>
            </div>
            <div class="hidden md:flex space-x-8">
                <a href="#hero" class="text-white hover:text-red-500 transition">Início</a>
                <a href="#about" class="text-white hover:text-red-500 transition">Sobre</a>
                <a href="#powers" class="text-white hover:text-red-500 transition">Poderes</a>
                <a href="#missions" class="text-white hover:text-red-500 transition">Missões</a>
                <a href="#contact" class="text-white hover:text-red-500 transition">Contato</a>
            </div>
            <button class="md:hidden text-white">
                <i class="fas fa-bars text-2xl"></i>
            </button>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="hero" class="hero-bg min-h-screen flex items-center justify-center text-center py-20 px-4">
        <div class="max-w-4xl mx-auto">
            <h1 class="title-font text-6xl md:text-8xl mb-6 text-white glow">
                SUPER <span class="text-red-600">XANDÃO</span>
            </h1>
            <p class="text-xl md:text-2xl mb-10 text-gray-300 max-w-2xl mx-auto">
                O defensor máximo da justiça e protetor do Brasil contra todas as forças do mal!
            </p>
            <div class="flex flex-col sm:flex-row justify-center gap-4">
                <button class="bg-red-600 hover:bg-red-700 text-white font-bold py-3 px-8 rounded-full text-lg transition transform hover:scale-105">
                    <i class="fas fa-fist-raised mr-2"></i> JUNTE-SE À LUTA
                </button>
                <button class="bg-transparent border-2 border-white hover:bg-white hover:text-black text-white font-bold py-3 px-8 rounded-full text-lg transition transform hover:scale-105">
                    <i class="fas fa-play mr-2"></i> ASSISTA AO TRAILER
                </button>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 bg-black">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16">
                <h2 class="title-font text-4xl md:text-5xl mb-4 text-white">
                    O <span class="text-red-600">HERÓI</span> QUE O BRASIL PRECISA
                </h2>
                <div class="w-24 h-1 bg-red-600 mx-auto"></div>
            </div>
            
            <div class="flex flex-col lg:flex-row items-center gap-12">
                <div class="lg:w-1/2">
                    <div class="relative">
                        <img src="https://images.unsplash.com/photo-1589254065878-42a9da0a9701?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" 
                             alt="Super Xandão" class="rounded-lg shadow-2xl w-full">
                        <div class="absolute -bottom-6 -right-6 bg-red-600 p-4 rounded-lg shadow-lg">
                            <h3 class="title-font text-2xl text-white">+1000</h3>
                            <p class="text-white">CRIMES COMBATIDOS</p>
                        </div>
                    </div>
                </div>
                <div class="lg:w-1/2">
                    <h3 class="title-font text-3xl mb-6 text-white">
                        A <span class="text-red-600">LENDA</span> DO SUPER XANDÃO
                    </h3>
                    <p class="text-gray-400 mb-6 text-lg">
                        Nascido nas ruas do Brasil, Alexandre "Xandão" Silva recebeu seus poderes após um experimento secreto do governo para criar o super-soldado perfeito. Desde então, ele dedica sua vida a proteger os inocentes e combater o crime organizado.
                    </p>
                    <p class="text-gray-400 mb-8 text-lg">
                        Com habilidades sobre-humanas e um código de honra inquebrável, Super Xandão se tornou o símbolo máximo da justiça em nosso país, inspirando milhões com seus atos heroicos.
                    </p>
                    <div class="grid grid-cols-2 gap-4">
                        <div class="flex items-center">
                            <div class="bg-red-600 p-3 rounded-full mr-4">
                                <i class="fas fa-medal text-white"></i>
                            </div>
                            <div>
                                <h4 class="text-white font-bold">Honra</h4>
                                <p class="text-gray-400 text-sm">Código de conduta</p>
                            </div>
                        </div>
                        <div class="flex items-center">
                            <div class="bg-red-600 p-3 rounded-full mr-4">
                                <i class="fas fa-shield-alt text-white"></i>
                            </div>
                            <div>
                                <h4 class="text-white font-bold">Proteção</h4>
                                <p class="text-gray-400 text-sm">Defesa dos fracos</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Powers Section -->
    <section id="powers" class="py-20 bg-gradient-to-b from-black to-gray-900">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16">
                <h2 class="title-font text-4xl md:text-5xl mb-4 text-white">
                    PODERES <span class="text-red-600">SOBRE-HUMANOS</span>
                </h2>
                <p class="text-gray-400 max-w-2xl mx-auto text-lg">
                    Equipado com habilidades extraordinárias para combater o mal em todas as suas formas
                </p>
                <div class="w-24 h-1 bg-red-600 mx-auto mt-4"></div>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Power 1 -->
                <div class="bg-gray-800 rounded-xl p-8 card-hover">
                    <div class="bg-red-600 w-16 h-16 rounded-full flex items-center justify-center mb-6 mx-auto">
                        <i class="fas fa-bolt text-white text-2xl"></i>
                    </div>
                    <h3 class="text-2xl font-bold text-white mb-4 text-center">Super Força</h3>
                    <p class="text-gray-400 text-center">
                        Capaz de levantar até 100 toneladas, Super Xandão pode derrubar criminosos com um único golpe e parar veículos em movimento com suas próprias mãos.
                    </p>
                </div>
                
                <!-- Power 2 -->
                <div class="bg-gray-800 rounded-xl p-8 card-hover">
                    <div class="bg-red-600 w-16 h-16 rounded-full flex items-center justify-center mb-6 mx-auto">
                        <i class="fas fa-running text-white text-2xl"></i>
                    </div>
                    <h3 class="text-2xl font-bold text-white mb-4 text-center">Super Velocidade</h3>
                    <p class="text-gray-400 text-center">
                        Movendo-se mais rápido que o olho humano pode acompanhar, ele pode estar em vários lugares ao mesmo tempo, garantindo que a justiça seja feita.
                    </p>
                </div>
                
                <!-- Power 3 -->
                <div class="bg-gray-800 rounded-xl p-8 card-hover">
                    <div class="bg-red-600 w-16 h-16 rounded-full flex items-center justify-center mb-6 mx-auto">
                        <i class="fas fa-eye text-white text-2xl"></i>
                    </div>
                    <h3 class="text-2xl font-bold text-white mb-4 text-center">Visão de Raio-X</h3>
                    <p class="text-gray-400 text-center">
                        Com sua visão penetrante, Super Xandão pode ver através de paredes e objetos, localizando vítimas e desarmando armadilhas dos criminosos.
                    </p>
                </div>
                
                <!-- Power 4 -->
                <div class="bg-gray-800 rounded-xl p-8 card-hover">
                    <div class="bg-red-600 w-16 h-16 rounded-full flex items-center justify-center mb-6 mx-auto">
                        <i class="fas fa-heartbeat text-white text-2xl"></i>
                    </div>
                    <h3 class="text-2xl font-bold text-white mb-4 text-center">Regeneração Rápida</h3>
                    <p class="text-gray-400 text-center">
                        Ferimentos que matariam um homem comum são curados em questão de minutos, permitindo que ele continue lutando sem parar.
                    </p>
                </div>
                
                <!-- Power 5 -->
                <div class="bg-gray-800 rounded-xl p-8 card-hover">
                    <div class="bg-red-600 w-16 h-16 rounded-full flex items-center justify-center mb-6 mx-auto">
                        <i class="fas fa-brain text-white text-2xl"></i>
                    </div>
                    <h3 class="text-2xl font-bold text-white mb-4 text-center">Intelecto Genial</h3>
                    <p class="text-gray-400 text-center">
                        Além da força física, Super Xandão possui uma mente brilhante, capaz de resolver os crimes mais complexos e antecipar os movimentos dos vilões.
                    </p>
                </div>
                
                <!-- Power 6 -->
                <div class="bg-gray-800 rounded-xl p-8 card-hover">
                    <div class="bg-red-600 w-16 h-16 rounded-full flex items-center justify-center mb-6 mx-auto">
                        <i class="fas fa-fist-raised text-white text-2xl"></i>
                    </div>
                    <h3 class="text-2xl font-bold text-white mb-4 text-center">Soco Sônico</h3>
                    <p class="text-gray-400 text-center">
                        Seu golpe mais poderoso, capaz de criar ondas de choque que derrubam dezenas de inimigos de uma só vez e quebrar barreiras impenetráveis.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Missions Section -->
    <section id="missions" class="py-20 bg-black">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16">
                <h2 class="title-font text-4xl md:text-5xl mb-4 text-white">
                    MISSÕES <span class="text-red-600">HERÓICAS</span>
                </h2>
                <p class="text-gray-400 max-w-2xl mx-auto text-lg">
                    Algumas das batalhas mais épicas travadas pelo Super Xandão
                </p>
                <div class="w-24 h-1 bg-red-600 mx-auto mt-4"></div>
            </div>
            
            <div class="grid md:grid-cols-2 gap-8 mb-12">
                <!-- Mission 1 -->
                <div class="relative rounded-xl overflow-hidden h-96">
                    <img src="https://images.unsplash.com/photo-1540206395-68808572332f?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1526&q=80" 
                         alt="Missão 1" class="w-full h-full object-cover">
                    <div class="absolute inset-0 bg-gradient-to-t from-black to-transparent flex items-end p-6">
                        <div>
                            <span class="bg-red-600 text-white text-sm px-3 py-1 rounded-full">2019</span>
                            <h3 class="text-2xl font-bold text-white mt-2">Queda do Cartel do Rio</h3>
                            <p class="text-gray-300">Super Xandão desmantelou sozinho a maior organização criminosa do país em uma operação noturna que durou apenas 6 horas.</p>
                        </div>
                    </div>
                </div>
                
                <!-- Mission 2 -->
                <div class="relative rounded-xl overflow-hidden h-96">
                    <img src="https://images.unsplash.com/photo-1508514177221-188e1e917088?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1632&q=80" 
                         alt="Missão 2" class="w-full h-full object-cover">
                    <div class="absolute inset-0 bg-gradient-to-t from-black to-transparent flex items-end p-6">
                        <div>
                            <span class="bg-red-600 text-white text-sm px-3 py-1 rounded-full">2020</span>
                            <h3 class="text-2xl font-bold text-white mt-2">Resgate na Torre Sul</h3>
                            <p class="text-gray-300">Quando um incêndio tomou conta do edifício mais alto de São Paulo, Super Xandão resgatou 247 pessoas em menos de 15 minutos.</p>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="grid md:grid-cols-3 gap-8">
                <!-- Mission 3 -->
                <div class="relative rounded-xl overflow-hidden h-64">
                    <img src="https://images.unsplash.com/photo-1560253023-3ec5d502959f?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" 
                         alt="Missão 3" class="w-full h-full object-cover">
                    <div class="absolute inset-0 bg-gradient-to-t from-black to-transparent flex items-end p-4">
                        <div>
                            <span class="bg-red-600 text-white text-xs px-2 py-1 rounded-full">2021</span>
                            <h3 class="text-lg font-bold text-white mt-1">Destruição da Máquina do Caos</h3>
                        </div>
                    </div>
                </div>
                
                <!-- Mission 4 -->
                <div class="relative rounded-xl overflow-hidden h-64">
                    <img src="https://images.unsplash.com/photo-1505455185-d8af85ee91e9?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" 
                         alt="Missão 4" class="w-full h-full object-cover">
                    <div class="absolute inset-0 bg-gradient-to-t from-black to-transparent flex items-end p-4">
                        <div>
                            <span class="bg-red-600 text-white text-xs px-2 py-1 rounded-full">2022</span>
                            <h3 class="text-lg font-bold text-white mt-1">Batalha Contra o Exército de Clones</h3>
                        </div>
                    </div>
                </div>
                
                <!-- Mission 5 -->
                <div class="relative rounded-xl overflow-hidden h-64">
                    <img src="https://images.unsplash.com/photo-1533134242443-9486e7c787fe?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" 
                         alt="Missão 5" class="w-full h-full object-cover">
                    <div class="absolute inset-0 bg-gradient-to-t from-black to-transparent flex items-end p-4">
                        <div>
                            <span class="bg-red-600 text-white text-xs px-2 py-1 rounded-full">2023</span>
                            <h3 class="text-lg font-bold text-white mt-1">Salvamento do Trem-Bala</h3>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-gradient-to-b from-gray-900 to-black">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16">
                <h2 class="title-font text-4xl md:text-5xl mb-4 text-white">
                    DENUNCIE <span class="text-red-600">O CRIME</span>
                </h2>
                <p class="text-gray-400 max-w-2xl mx-auto text-lg">
                    Se você testemunhar atividades criminosas ou precisar de ajuda do Super Xandão, envie sua mensagem
                </p>
                <div class="w-24 h-1 bg-red-600 mx-auto mt-4"></div>
            </div>
            
            <div class="max-w-4xl mx-auto bg-gray-800 rounded-xl p-8 md:p-12 shadow-2xl">
                <form>
                    <div class="grid md:grid-cols-2 gap-6 mb-6">
                        <div>
                            <label for="name" class="block text-white mb-2">Seu Nome</label>
                            <input type="text" id="name" class="w-full bg-gray-700 border border-gray-600 rounded-lg px-4 py-3 text-white focus:outline-none focus:ring-2 focus:ring-red-600">
                        </div>
                        <div>
                            <label for="email" class="block text-white mb-2">Seu E-mail</label>
                            <input type="email" id="email" class="w-full bg-gray-700 border border-gray-600 rounded-lg px-4 py-3 text-white focus:outline-none focus:ring-2 focus:ring-red-600">
                        </div>
                    </div>
                    <div class="mb-6">
                        <label for="subject" class="block text-white mb-2">Assunto</label>
                        <input type="text" id="subject" class="w-full bg-gray-700 border border-gray-600 rounded-lg px-4 py-3 text-white focus:outline-none focus:ring-2 focus:ring-red-600">
                    </div>
                    <div class="mb-8">
                        <label for="message" class="block text-white mb-2">Sua Mensagem</label>
                        <textarea id="message" rows="5" class="w-full bg-gray-700 border border-gray-600 rounded-lg px-4 py-3 text-white focus:outline-none focus:ring-2 focus:ring-red-600"></textarea>
                    </div>
                    <button type="submit" class="w-full bg-red-600 hover:bg-red-700 text-white font-bold py-4 px-6 rounded-lg text-lg transition transform hover:scale-105">
                        <i class="fas fa-paper-plane mr-2"></i> ENVIAR MENSAGEM
                    </button>
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-black py-12 border-t border-gray-800">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row justify-between items-center">
                <div class="flex items-center mb-6 md:mb-0">
                    <i class="fas fa-shield-alt text-red-600 text-2xl mr-2"></i>
                    <span class="title-font text-2xl text-white">SUPER <span class="text-red-600">XANDÃO</span></span>
                </div>
                <div class="flex space-x-6 mb-6 md:mb-0">
                    <a href="#" class="text-gray-400 hover:text-red-600 text-xl transition">
                        <i class="fab fa-facebook-f"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-red-600 text-xl transition">
                        <i class="fab fa-twitter"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-red-600 text-xl transition">
                        <i class="fab fa-instagram"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-red-600 text-xl transition">
                        <i class="fab fa-youtube"></i>
                    </a>
                </div>
                <div class="flex flex-col items-center md:items-end">
                    <p class="text-gray-400 mb-2">Assine nossa newsletter</p>
                    <div class="flex">
                        <input type="email" placeholder="Seu e-mail" class="bg-gray-800 text-white px-4 py-2 rounded-l-lg focus:outline-none">
                        <button class="bg-red-600 hover:bg-red-700 text-white px-4 py-2 rounded-r-lg transition">
                            <i class="fas fa-paper-plane"></i>
                        </button>
                    </div>
                </div>
            </div>
            <div class="border-t border-gray-800 mt-12 pt-8 flex flex-col md:flex-row justify-between items-center">
                <p class="text-gray-500 text-sm mb-4 md:mb-0">
                    © 2023 Super Xandão. Todos os direitos reservados.
                </p>
                <div class="flex space-x-6">
                    <a href="#" class="text-gray-500 hover:text-white text-sm transition">Termos de Uso</a>
                    <a href="#" class="text-gray-500 hover:text-white text-sm transition">Política de Privacidade</a>
                    <a href="#" class="text-gray-500 hover:text-white text-sm transition">Contato</a>
                </div>
            </div>
        </div>
    </footer>

    <!-- Back to Top Button -->
    <button id="backToTop" class="fixed bottom-8 right-8 bg-red-600 text-white w-12 h-12 rounded-full flex items-center justify-center shadow-lg transition opacity-0 invisible">
        <i class="fas fa-arrow-up"></i>
    </button>

    <script>
        // Back to Top Button
        const backToTopButton = document.getElementById('backToTop');
        
        window.addEventListener('scroll', () => {
            if (window.pageYOffset > 300) {
                backToTopButton.classList.remove('opacity-0', 'invisible');
                backToTopButton.classList.add('opacity-100', 'visible');
            } else {
                backToTopButton.classList.remove('opacity-100', 'visible');
                backToTopButton.classList.add('opacity-0', 'invisible');
            }
        });
        
        backToTopButton.addEventListener('click', () => {
            window.scrollTo({
                top: 0,
                behavior: 'smooth'
            });
        });
        
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
        
        // Form submission (demo)
        const form = document.querySelector('form');
        if (form) {
            form.addEventListener('submit', (e) => {
                e.preventDefault();
                alert('Mensagem enviada com sucesso! O Super Xandão entrará em contato em breve.');
                form.reset();
            });
        }
    </script>
</body>
</html># btcorbct
