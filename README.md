.tag:hover {
            background-color: #2563EB;
            color: white;
        }
        
        .admin-menu {
            position: fixed;
            top: 20px;
            right: 20px;
            z-index: 1000;
        }
        
        .admin-dropdown {
            display: none;
            position: absolute;
            right: 0;
            background-color: white;
            min-width: 160px;
            box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
            z-index: 1;
            border-radius: 4px;
            overflow: hidden;
        }
        
        .admin-dropdown a {
            color: #1E3A8A;
            padding: 12px 16px;
            text-decoration: none;
            display: block;
            transition: background-color 0.3s;
        }
        
        .admin-dropdown a:hover {
            background-color: #EFF6FF;
        }
        
        .show {
            display: block;
        }
    </style>
</head>
<body class="bg-gray-50 font-body">
    <!-- Admin Menu -->
    <div class="admin-menu">
        <button onclick="toggleAdminMenu()" class="bg-primary text-white w-10 h-10 rounded-full flex items-center justify-center hover:bg-secondary transition duration-300">
            <i class="fas fa-ellipsis-v"></i>
        </button>
        <div id="adminDropdown" class="admin-dropdown">
            <a href="#"><i class="fas fa-plus mr-2"></i> Novo Artigo</a>
            <a href="#"><i class="fas fa-list mr-2"></i> Gerenciar Artigos</a>
            <a href="#"><i class="fas fa-cog mr-2"></i> Configurações</a>
            <a href="#"><i class="fas fa-sign-out-alt mr-2"></i> Sair</a>
        </div>
    </div>

    <!-- Header -->
    <header class="bg-primary text-white shadow-lg">
        <div class="container mx-auto px-6 py-4">
            <div class="flex items-center justify-between">
                <div class="flex items-center space-x-4">
                    <i class="fas fa-balance-scale text-3xl"></i>
                    <div>
                        <h1 class="text-2xl font-bold font-sans">LOPES & PIMENTEL</h1>
                        <p class="text-light text-sm">Advogados Associados | CNPJ 53.181.246/0001-73</p>
                    </div>
                </div>
                <nav class="hidden md:flex space-x-8">
                    <a href="#" class="hover:text-accent font-semibold">Início</a>
                    <a href="#" class="hover:text-accent font-semibold">Artigos</a>
                    <a href="#" class="hover:text-accent font-semibold">Publicações</a>
                    <a href="#" class="hover:text-accent font-semibold">Sobre</a>
                    <a href="#" class="hover:text-accent font-semibold">Contato</a>
                </nav>
                <button class="md:hidden focus:outline-none">
                    <i class="fas fa-bars text-2xl"></i>
                </button>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="bg-gradient-to-r from-primary to-secondary text-white py-20">
        <div class="container mx-auto px-6 text-center">
            <h2 class="text-4xl md:text-5xl font-bold mb-6 font-sans">Excelência Jurídica com Rigor Científico</h2>
            <p class="text-xl mb-8 max-w-3xl mx-auto">Soluções jurídicas personalizadas e artigos acadêmicos para clientes e profissionais do Direito.</p>
            <div class="flex flex-col sm:flex-row justify-center gap-4">
                <a href="#articles" class="bg-white text-primary font-bold py-3 px-8 rounded-lg hover:bg-light transition duration-300">
                    Explorar Artigos
                </a>
                <a href="#contact" class="bg-transparent border-2 border-white text-white font-bold py-3 px-8 rounded-lg hover:bg-white hover:text-primary transition duration-300">
                    Fale com o Advogado
                </a>
            </div>
        </div>
    </section>

    <!-- Featured Article -->
    <section class="py-16 bg-white">
        <div class="container mx-auto px-6">
            <div class="bg-light rounded-xl p-8 shadow-lg">
                <div class="flex flex-col lg:flex-row gap-8">
                    <div class="lg:w-1/3">
                        <img src="https://images.unsplash.com/photo-1589829545856-d10d557cf95f?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Direito" class="w-full h-64 object-cover rounded-lg shadow-md">
                    </div>
                    <div class="lg:w-2/3">
                        <span class="inline-block bg-accent text-white text-xs px-3 py-1 rounded-full mb-3">Destaque</span>
                        <h3 class="text-3xl font-bold text-dark mb-4 font-sans">A Evolução do Direito Digital no Brasil: Desafios e Perspectivas</h3>
                        <p class="text-gray-700 mb-4">Este artigo analisa criticamente o desenvolvimento do marco regulatório do direito digital no Brasil, abordando os principais desafios legislativos e jurisprudenciais enfrentados na proteção de dados pessoais, crimes cibernéticos e comércio eletrônico.</p>
                        <div class="flex flex-wrap gap-2 mb-6">
                            <span class="tag bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Direito Digital</span>
                            <span class="tag bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">LGPD</span>
                            <span class="tag bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Tecnologia</span>
                        </div>
                        <div class="flex items-center justify-between">
                            <div class="flex items-center">
                                <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=100&q=80" alt="João Felipe Pimentel" class="w-10 h-10 rounded-full mr-3">
                                <div>
                                    <p class="font-semibold text-dark">João Felipe Pimentel</p>
                                    <p class="text-sm text-gray-500">Publicado em 15/08/2023</p>
                                </div>
                            </div>
                            <a href="#" class="bg-primary text-white px-6 py-2 rounded-lg hover:bg-secondary transition duration-300">Ler Artigo</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Articles Section -->
    <section id="articles" class="py-16 bg-gray-50">
        <div class="container mx-auto px-6">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold text-dark mb-4 font-sans">Artigos Científicos Recentes</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">Publicações acadêmicas e análises jurídicas aprofundadas sobre diversos ramos do Direito.</p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Article 1 -->
                <div class="article-card bg-white rounded-xl overflow-hidden shadow-md transition duration-300">
                    <img src="https://images.unsplash.com/photo-1450101499163-c8848c66ca85?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Direito Tributário" class="w-full h-48 object-cover">
                    <div class="p-6">
                        <div class="flex flex-wrap gap-2 mb-3">
                            <span class="tag bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Tributário</span>
                            <span class="tag bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Economia</span>
                        </div>
                        <h3 class="text-xl font-bold text-dark mb-3 font-sans">Reforma Tributária: Impactos nas Empresas Brasileiras</h3>
                        <p class="text-gray-600 mb-4">Análise dos principais pontos da proposta de reforma tributária e seus possíveis efeitos no ambiente de negócios nacional.</p>
                        <div class="flex items-center justify-between">
                            <span class="text-sm text-gray-500">10/08/2023</span>
                            <a href="#" class="text-primary font-semibold hover:underline">Ler mais →</a>
                        </div>
                    </div>
                </div>
                
                <!-- Article 2 -->
                <div class="article-card bg-white rounded-xl overflow-hidden shadow-md transition duration-300">
                    <img src="https://images.unsplash.com/photo-1589391886645-d51941baf7fb?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Direito Ambiental" class="w-full h-48 object-cover">
                    <div class="p-6">
                        <div class="flex flex-wrap gap-2 mb-3">
                            <span class="tag bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Ambiental</span>
                            <span class="tag bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Sustentabilidade</span>
                        </div>
                        <h3 class="text-xl font-bold text-dark mb-3 font-sans">Licenciamento Ambiental e Desenvolvimento Sustentável</h3>
                        <p class="text-gray-600 mb-4">Estudo sobre os novos paradigmas do licenciamento ambiental brasileiro frente aos desafios do desenvolvimento sustentável.</p>
                        <div class="flex items-center justify-between">
                            <span class="text-sm text-gray-500">03/08/2023</span>
                            <a href="#" class="text-primary font-semibold hover:underline">Ler mais →</a>
                        </div>
                    </div>
                </div>
                
                <!-- Article 3 -->
                <div class="article-card bg-white rounded-xl overflow-hidden shadow-md transition duration-300">
                    <img src="https://images.unsplash.com/photo-1589829545856-d10d557cf95f?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Direito Trabalhista" class="w-full h-48 object-cover">
                    <div class="p-6">
                        <div class="flex flex-wrap gap-2 mb-3">
                            <span class="tag bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Trabalhista</span>
                            <span class="tag bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Terceirização</span>
                        </div>
                        <h3 class="text-xl font-bold text-dark mb-3 font-sans">Terceirização e Precarização: Limites Jurídicos</h3>
                        <p class="text-gray-600 mb-4">Análise crítica da jurisprudência do TST sobre os limites da terceirização e seus impactos nas relações de trabalho.</p>
                        <div class="flex items-center justify-between">
                            <span class="text-sm text-gray-500">27/07/2023</span>
                            <a href="#" class="text-primary font-semibold hover:underline">Ler mais →</a>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-12">
                <a href="#" class="inline-block bg-primary text-white font-bold py-3 px-8 rounded-lg hover:bg-secondary transition duration-300">
                    Ver Todos os Artigos
                </a>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section class="py-16 bg-white">
        <div class="container mx-auto px-6">
            <div class="flex flex-col lg:flex-row items-center gap-12">
                <div class="lg:w-1/2">
                    <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=800&q=80" alt="João Felipe Pimentel" class="w-full rounded-xl shadow-lg">
                </div>
                <div class="lg:w-1/2">
                    <h2 class="text-3xl font-bold text-dark mb-6 font-sans">Sobre João Felipe Pimentel</h2>
                    <p class="text-gray-700 mb-4">Sócio-fundador do escritório LOPES & PIMENTEL Advogados Associados, Mestre em Direito pela Universidade Federal, com especialização em Direito Civil e Processual Civil. Atua há mais de 15 anos na advocacia consultiva e contenciosa, com vasta experiência em casos complexos.</p>
                    <p class="text-gray-700 mb-6">Autor de diversos artigos científicos publicados em revistas especializadas e palestrante em eventos jurídicos nacionais e internacionais. Comprometido com a produção acadêmica de qualidade e sua aplicação prática na advocacia.</p>
                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-4 mb-8">
                        <div class="flex items-center">
                            <i class="fas fa-graduation-cap text-primary mr-3 text-xl"></i>
                            <span class="text-gray-700">Mestre em Direito</span>
                        </div>
                        <div class="flex items-center">
                            <i class="fas fa-briefcase text-primary mr-3 text-xl"></i>
                            <span class="text-gray-700">15+ anos de experiência</span>
                        </div>
                        <div class="flex items-center">
                            <i class="fas fa-book text-primary mr-3 text-xl"></i>
                            <span class="text-gray-700">20+ artigos publicados</span>
                        </div>
                        <div class="flex items-center">
                            <i class="fas fa-medal text-primary mr-3 text-xl"></i>
                            <span class="text-gray-700">Prêmios acadêmicos</span>
                        </div>
                    </div>
                    <a href="#" class="inline-block bg-primary text-white font-bold py-3 px-8 rounded-lg hover:bg-secondary transition duration-300">
                        Saiba Mais
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-16 bg-light">
        <div class="container mx-auto px-6">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold text-dark mb-4 font-sans">Entre em Contato</h2>
                <p class="text-gray-700 max-w-2xl mx-auto">Para consultorias jurídicas especializadas ou dúvidas sobre os artigos publicados.</p>
            </div>
            
            <div class="bg-white rounded-xl shadow-lg p-8 max-w-4xl mx-auto">
                <div class="flex flex-col md:flex-row gap-8">
                    <div class="md:w-1/2">
                        <h3 class="text-xl font-bold text-dark mb-6 font-sans">Informações de Contato</h3>
                        <div class="space-y-4">
                            <div class="flex items-start">
                                <i class="fas fa-envelope text-primary mt-1 mr-4"></i>
                                <div>
                                    <h4 class="font-semibold text-gray-800">Email</h4>
                                    <p class="text-gray-600">joaofelipelopes.adv@gmail.com</p>
                                </div>
                            </div>
                            <div class="flex items-start">
                                <i class="fas fa-phone-alt text-primary mt-1 mr-4"></i>
                                <div>
                                    <h4 class="font-semibold text-gray-800">Telefone</h4>
                                    <p class="text-gray-600">(71) 98199-8223</p>
                                </div>
                            </div>
                            <div class="flex items-start">
                                <i class="fas fa-map-marker-alt text-primary mt-1 mr-4"></i>
                                <div>
                                    <h4 class="font-semibold text-gray-800">Escritório</h4>
                                    <p class="text-gray-600">Av. Principal, 1234 - Sala 501<br>Centro - Salvador/BA</p>
                                </div>
                            </div>
                        </div>
                        
                        <div class="mt-8">
                            <h3 class="text-xl font-bold text-dark mb-4 font-sans">Redes Sociais</h3>
                            <div class="flex space-x-4">
                                <a href="#" class="bg-gray-100 text-gray-700 w-10 h-10 rounded-full flex items-center justify-center hover:bg-primary hover:text-white transition duration-300">
                                    <i class="fab fa-linkedin-in"></i>
                                </a>
                                <a href="#" class="bg-gray-100 text-gray-700 w-10 h-10 rounded-full flex items-center justify-center hover:bg-blue-500 hover:text-white transition duration-300">
                                    <i class="fab fa-twitter"></i>
                                </a>
                                <a href="#" class="bg-gray-100 text-gray-700 w-10 h-10 rounded-full flex items-center justify-center hover:bg-blue-800 hover:text-white transition duration-300">
                                    <i class="fab fa-facebook-f"></i>
                                </a>
                                <a href="#" class="bg-gray-100 text-gray-700 w-10 h-10 rounded-full flex items-center justify-center hover:bg-pink-600 hover:text-white transition duration-300">
                                    <i class="fab fa-instagram"></i>
                                </a>
                            </div>
                        </div>
                    </div>
                    
                    <div class="md:w-1/2">
                        <h3 class="text-xl font-bold text-dark mb-6 font-sans">Envie uma Mensagem</h3>
                        <form class="space-y-4">
                            <div>
                                <label for="name" class="block text-gray-700 font-medium mb-2">Nome</label>
                                <input type="text" id="name" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent">
                            </div>
                            <div>
                                <label for="email" class="block text-gray-700 font-medium mb-2">Email</label>
                                <input type="email" id="email" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent">
                            </div>
                            <div>
                                <label for="subject" class="block text-gray-700 font-medium mb-2">Assunto</label>
                                <input type="text" id="subject" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent">
                            </div>
                            <div>
                                <label for="message" class="block text-gray-700 font-medium mb-2">Mensagem</label>
                                <textarea id="message" rows="4" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent"></textarea>
                            </div>
                            <button type="submit" class="w-full bg-primary text-white font-bold py-3 px-6 rounded-lg hover:bg-secondary transition duration-300">
                                Enviar Mensagem
                            </button>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- WhatsApp Float Button -->
    <a href="https://wa.me/5571981998223?text=Olá%20João%20Felipe%20Pimentel,%20gostaria%20de%20mais%20informações%20sobre%20seus%20serviços%20jurídicos" class="whatsapp-float" target="_blank">
        <i class="fab fa-whatsapp"></i>
    </a>

    <!-- Footer -->
    <footer class="bg-dark text-white py-12">
        <div class="container mx-auto px-6">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <div>
                    <h3 class="text-xl font-bold mb-4 font-sans">LOPES & PIMENTEL</h3>
                    <p class="text-gray-400">Advogados Associados | CNPJ 53.181.246/0001-73</p>
                    <p class="text-gray-400 mt-2">Excelência jurídica com rigor científico para profissionais e estudantes de Direito.</p>
                </div>
                <div>
                    <h4 class="font-bold mb-4 text-lg">Links Rápidos</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Início</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Artigos</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Publicações</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Sobre</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Contato</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="font-bold mb-4 text-lg">Categorias</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Direito Civil</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Direito Penal</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Direito Tributário</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Direito Trabalhista</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Direito Ambiental</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="font-bold mb-4 text-lg">Newsletter</h4>
                    <p class="text-gray-400 mb-4">Assine para receber novos artigos e atualizações.</p>
                    <form class="flex">
                        <input type="email" placeholder="Seu email" class="px-4 py-2 w-full rounded-l-lg focus:outline-none text-dark">
                        <button type="submit" class="bg-primary px-4 py-2 rounded-r-lg hover:bg-secondary transition duration-300">
                            <i class="fas fa-paper-plane"></i>
                        </button>
                    </form>
                </div>
            </div>
            <div class="border-t border-gray-800 mt-8 pt-8 text-center text-gray-400">
                <p>&copy; 2023 LOPES & PIMENTEL Advogados Associados. Todos os direitos reservados.</p>
            </div>
        </div>
    </footer>

    <script>
        // WhatsApp button click event
        document.querySelector('.whatsapp-float').addEventListener('click', function() {
            // You can add analytics here if needed
            console.log('WhatsApp button clicked');
        });
        
        // Mobile menu toggle functionality would go here
        // This is a basic implementation for demonstration
        document.querySelector('button.md\\:hidden').addEventListener('click', function() {
            const nav = document.querySelector('nav.md\\:flex');
            if (nav.style.display === 'flex') {
                nav.style.display = 'none';
            } else {
                nav.style.display = 'flex';
                nav.classList.add('flex-col', 'absolute', 'top-16', 'right-0', 'bg-primary', 'w-full', 'p-4', 'space-y-4', 'space-x-0', 'z-50');
            }
        });
        
        // Admin menu toggle
        function toggleAdminMenu() {
            document.getElementById('adminDropdown').classList.toggle('show');
        }
        
        // Close the dropdown if clicked outside
        window.onclick = function(event) {
            if (!event.target.matches('.admin-menu button')) {
                var dropdowns = document.getElementsByClassName("admin-dropdown");
                for (var i = 0; i < dropdowns.length; i++) {
                    var openDropdown = dropdowns[i];
                    if (openDropdown.classList.contains('show')) {
                        openDropdown.classList.remove('show');
                    }
                }
            }
        }
    </script>
</body>
</html>
