# Portfolio
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MD ARMAN ALI | Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');
        
        body {
            font-family: 'Poppins', sans-serif;
            scroll-behavior: smooth;
            background-color: #f8fafc;
        }
        
        .gradient-text {
            background: linear-gradient(90deg, #3b82f6, #8b5cf6);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }
        
        .card-hover {
            transition: all 0.3s ease;
        }
        
        .card-hover:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }
        
        .nav-link {
            position: relative;
        }
        
        .nav-link::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: -2px;
            left: 0;
            background-color: #3b82f6;
            transition: width 0.3s ease;
        }
        
        .nav-link:hover::after {
            width: 100%;
        }
        
        .active::after {
            width: 100%;
        }
        
        .timeline-item {
            position: relative;
            padding-left: 2rem;
        }
        
        .timeline-item::before {
            content: '';
            position: absolute;
            left: 0;
            top: 0;
            width: 2px;
            height: 100%;
            background: #3b82f6;
        }
        
        .timeline-dot {
            position: absolute;
            left: -0.5rem;
            top: 0.5rem;
            width: 1rem;
            height: 1rem;
            border-radius: 50%;
            background: #3b82f6;
            z-index: 1;
        }
        
        .skill-bar {
            height: 8px;
            border-radius: 4px;
            background: #e2e8f0;
        }
        
        .skill-progress {
            height: 100%;
            border-radius: 4px;
            background: linear-gradient(90deg, #3b82f6, #8b5cf6);
        }
        
        .project-card {
            transition: all 0.3s ease;
            perspective: 1000px;
        }
        
        .project-card:hover {
            transform: translateY(-5px);
        }
        
        .project-card-inner {
            position: relative;
            width: 100%;
            height: 100%;
            transition: transform 0.6s;
            transform-style: preserve-3d;
        }
        
        .project-card:hover .project-card-inner {
            transform: rotateY(10deg);
        }
        
        .project-card-front, .project-card-back {
            position: absolute;
            width: 100%;
            height: 100%;
            backface-visibility: hidden;
        }
        
        .project-card-back {
            transform: rotateY(180deg);
        }
        
        .contact-input {
            transition: all 0.3s ease;
        }
        
        .contact-input:focus {
            box-shadow: 0 0 0 2px rgba(59, 130, 246, 0.5);
        }
    </style>
</head>
<body class="text-gray-800">
    <!-- Navigation -->
    <nav class="fixed w-full bg-white shadow-sm z-50">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-16">
                <div class="flex items-center">

                    <a href="#home" class="text-xl font-bold gradient-text"> MD ARMAN ALI</a>
                    </div>
                <div class="hidden md:flex items-center space-x-8">
                    <a href="#home" class="nav-link active">Home</a>
                    <a href="#about" class="nav-link">About</a>
                    <a href="#skills" class="nav-link">Skills</a>
                    <a href="#experience" class="nav-link">Experience</a>
                    <a href="#projects" class="nav-link">Projects</a>
                    <a href="#contact" class="nav-link">Contact</a>
                </div>
                <div class="md:hidden flex items-center">
                    <button id="menu-toggle" class="text-gray-600 hover:text-blue-500 focus:outline-none">
                        <i class="fas fa-bars text-xl"></i>
                    </button>
                </div>
            </div>
        </div>
        
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-white shadow-lg">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                <a href="#home" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-blue-500">Home</a>
                <a href="#about" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-blue-500">About</a>
                <a href="#skills" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-blue-500">Skills</a>
                <a href="#experience" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-blue-500">Experience</a>
                <a href="#projects" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-blue-500">Projects</a>
                <a href="#contact" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-blue-500">Contact</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="pt-24 pb-16 md:pt-32 md:pb-24 bg-gradient-to-r from-blue-50 to-purple-50">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 mb-8 md:mb-0">
                    <h1 class="text-4xl md:text-5xl font-bold mb-4">Hi, I'm <span class="gradient-text">MD ARMAN ALI</span></h1>
                    <h2 class="text-2xl md:text-3xl font-semibold mb-6 text-gray-700">First Year Electrical Engineering Student</h2>
                    <p class="text-lg text-gray-600 mb-8">UI/UX Designer | Poster Design & Editing | MLSA | Ex Campus Ambassador IIT Delhi Rendezvous | Frontiers CTR Club</p>
                    <div class="flex space-x-4">
                        <a href="#contact" class="px-6 py-3 bg-gradient-to-r from-blue-500 to-purple-500 text-white rounded-lg font-medium hover:shadow-lg transition-all duration-300">Get In Touch</a>
                        <a href="#projects" class="px-6 py-3 border border-blue-500 text-blue-500 rounded-lg font-medium hover:bg-blue-50 transition-all duration-300">View My Work</a>
                    </div>
                </div>
                <div class="md:w-1/2 flex justify-center">
                    <div class="relative w-64 h-64 md:w-80 md:h-80 rounded-full overflow-hidden border-4 border-white shadow-xl">
                        <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=774&q=80" alt="MD ARMAN ALI" class="w-full h-full object-cover">
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-16 bg-white">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <h2 class="text-3xl font-bold text-center mb-12 gradient-text">About Me</h2>
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/3 mb-8 md:mb-0 flex justify-center">
                    <div class="relative w-64 h-64 rounded-lg overflow-hidden shadow-xl">
                        <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=774&q=80" alt="MD ARMAN ALI" class="w-full h-full object-cover">
                    </div>
                </div>
                <div class="md:w-2/3 md:pl-12">
                    <h3 class="text-2xl font-semibold mb-4">Who am I?</h3>
                    <p class="text-gray-600 mb-6">I'm MD ARMAN ALI, a passionate first-year Electrical Engineering student with a strong interest in UI/UX design, graphic design, and technology. I'm constantly exploring new ways to combine my technical knowledge with creative design to solve real-world problems.</p>
                    
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-8">
                        <div class="bg-gray-50 p-4 rounded-lg">
                            <h4 class="font-semibold text-blue-600 mb-2"><i class="fas fa-graduation-cap mr-2"></i>Education</h4>
                            <p class="text-gray-600">First Year Electrical Engineering</p>
                        </div>
                        <div class="bg-gray-50 p-4 rounded-lg">
                            <h4 class="font-semibold text-purple-600 mb-2"><i class="fas fa-briefcase mr-2"></i>Experience</h4>
                            <p class="text-gray-600">UI/UX Designer, Poster Designer</p>
                        </div>
                    </div>
                    
                    <div class="flex flex-wrap gap-4">
                        <div class="flex items-center bg-blue-50 px-4 py-2 rounded-full">
                            <i class="fas fa-palette text-blue-500 mr-2"></i>
                            <span class="text-sm">UI/UX Design</span>
                        </div>
                        <div class="flex items-center bg-purple-50 px-4 py-2 rounded-full">
                            <i class="fas fa-edit text-purple-500 mr-2"></i>
                            <span class="text-sm">Poster Design</span>
                        </div>
                        <div class="flex items-center bg-green-50 px-4 py-2 rounded-full">
                            <i class="fas fa-users text-green-500 mr-2"></i>
                            <span class="text-sm">MLSA</span>
                        </div>
                        <div class="flex items-center bg-yellow-50 px-4 py-2 rounded-full">
                            <i class="fas fa-university text-yellow-500 mr-2"></i>
                            <span class="text-sm">Campus Ambassador</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="py-16 bg-gray-50">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <h2 class="text-3xl font-bold text-center mb-12 gradient-text">My Skills</h2>
            
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <!-- Design Skills -->
                <div class="bg-white p-6 rounded-lg shadow-sm card-hover">
                    <h3 class="text-xl font-semibold mb-6 flex items-center">
                        <i class="fas fa-palette text-blue-500 mr-3"></i>
                        Design Skills
                    </h3>
                    <div class="space-y-4">
                        <div>
                            <div class="flex justify-between mb-1">
                                <span class="text-gray-700">UI/UX Design</span>
                                <div class="bg-gray-50 p-6 rounded-lg shadow-sm card-hover">
                        <div class="flex flex-col md:flex-row md:justify-between md:items-center mb-4">
                            <h3 class="text-xl font-semibold">Campus Ambassador - IIT Delhi Rendezvous</h3>
                            <span class="text-purple-500 font-medium">2022 - 2023</span>
                        </div>
                        <p class="text-gray-600 mb-4">Represented IIT Delhi's annual cultural fest Rendezvous at my institution.</p>
                        <ul class="list-disc pl-5 text-gray-600 space-y-1">
                            <li>Promoted events and competitions</li>
                            <li>Coordinated student participation</li>
                            <li>Managed social media campaigns</li>
                        </ul>
                    </div>
                </div>
                
                <!-- Frontiers CTR Club -->
                <div class="timeline-item">
                    <div class="timeline-dot"></div>
                    <div class="bg-gray-50 p-6 rounded-lg shadow-sm card-hover">
                        <div class="flex flex-col md:flex-row md:justify-between md:items-center mb-4">
                            <h3 class="text-xl font-semibold">Frontiers CTR Club</h3>
                            <span class="text-blue-500 font-medium">2022 - Present</span>
                        </div>
                        <p class="text-gray-600 mb-4">Active member of the Frontiers CTR Club, participating in various technical and creative activities.</p>
                        <ul class="list-disc pl-5 text-gray-600 space-y-1">
                            <li>Designed posters for club events</li>
                            <li>Contributed to UI/UX projects</li>
                            <li>Participated in technical workshops</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="py-16 bg-gray-50">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <h2 class="text-3xl font-bold text-center mb-12 gradient-text">My Projects</h2>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- UI/UX Project 1 -->
                <div class="project-card">
                    <div class="project-card-inner">
                        <div class="project-card-front bg-white p-6 rounded-lg shadow-sm h-full">
                            <div class="h-48 bg-gradient-to-r from-blue-100 to-purple-100 rounded-lg mb-4 flex items-center justify-center">
                                <i class="fas fa-mobile-alt text-5xl text-blue-500"></i>
                            </div>
                            <h3 class="text-xl font-semibold mb-2">Mobile App UI Design</h3>
                            <p class="text-gray-600 mb-4">A modern mobile application interface designed for productivity.</p>
                            <div class="flex flex-wrap gap-2">
                                <span class="text-xs bg-blue-100 text-blue-800 px-2 py-1 rounded">Figma</span>
                                <span class="text-xs bg-purple-100 text-purple-800 px-2 py-1 rounded">UI Design</span>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Poster Design Project -->
                <div class="project-card">
                    <div class="project-card-inner">
                        <div class="project-card-front bg-white p-6 rounded-lg shadow-sm h-full">
                            <div class="h-48 bg-gradient-to-r from-purple-100 to-pink-100 rounded-lg mb-4 flex items-center justify-center">
</body>
</Html>
