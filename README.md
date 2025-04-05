<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Name | Professional Portfolio</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                    colors: {
                        primary: {
                            50: '#f0f9ff',
                            100: '#e0f2fe',
                            200: '#bae6fd',
                            300: '#7dd3fc',
                            400: '#38bdf8',
                            500: '#0ea5e9',
                            600: '#0284c7',
                            700: '#0369a1',
                            800: '#075985',
                            900: '#0c4a6e',
                        }
                    }
                }
            }
        }
    </script>
    <!-- Font Awesome CDN -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        html {
            scroll-behavior: smooth;
        }
        .gradient-text {
            background: linear-gradient(90deg, #0ea5e9, #3b82f6);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }
        .section-title:after {
            content: '';
            display: block;
            width: 60px;
            height: 3px;
            background: linear-gradient(90deg, #0ea5e9, #3b82f6);
            margin: 15px auto 0;
        }
    </style>
</head>
<body class="font-sans bg-gray-50 text-gray-800">
    <!-- Navigation -->
    <nav class="fixed w-full bg-white/90 backdrop-blur-md shadow-sm z-50">
        <div class="max-w-7xl mx-auto px-6">
            <div class="flex justify-between h-20 items-center">
                <a href="#home" class="text-2xl font-bold gradient-text">YN</a>
                <div class="hidden md:flex items-center space-x-8">
                    <a href="#home" class="text-gray-700 hover:text-primary-600 font-medium transition duration-300">Home</a>
                    <a href="#about" class="text-gray-700 hover:text-primary-600 font-medium transition duration-300">About</a>
                    <a href="#services" class="text-gray-700 hover:text-primary-600 font-medium transition duration-300">Services</a>
                    <a href="#portfolio" class="text-gray-700 hover:text-primary-600 font-medium transition duration-300">Portfolio</a>
                    <a href="#testimonials" class="text-gray-700 hover:text-primary-600 font-medium transition duration-300">Testimonials</a>
                    <a href="#contact" class="text-gray-700 hover:text-primary-600 font-medium transition duration-300">Contact</a>
                </div>
                <div class="md:hidden flex items-center">
                    <button id="menu-btn" class="text-gray-700">
                        <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                        </svg>
                    </button>
                </div>
            </div>
        </div>
        <!-- Mobile menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-white/95 backdrop-blur-md pb-4 px-6 shadow-lg">
            <a href="#home" class="block py-3 text-gray-700 hover:text-primary-600 transition duration-300 border-b border-gray-100">Home</a>
            <a href="#about" class="block py-3 text-gray-700 hover:text-primary-600 transition duration-300 border-b border-gray-100">About</a>
            <a href="#services" class="block py-3 text-gray-700 hover:text-primary-600 transition duration-300 border-b border-gray-100">Services</a>
            <a href="#portfolio" class="block py-3 text-gray-700 hover:text-primary-600 transition duration-300 border-b border-gray-100">Portfolio</a>
            <a href="#testimonials" class="block py-3 text-gray-700 hover:text-primary-600 transition duration-300 border-b border-gray-100">Testimonials</a>
            <a href="#contact" class="block py-3 text-gray-700 hover:text-primary-600 transition duration-300">Contact</a>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="min-h-screen flex items-center pt-20">
        <div class="max-w-7xl mx-auto px-6 py-20">
            <div class="grid md:grid-cols-2 gap-12 items-center">
                <div class="order-2 md:order-1">
                    <h1 class="text-4xl md:text-5xl lg:text-6xl font-bold mb-6 leading-tight">
                        Hi, I'm <span class="gradient-text">Your Name</span>
                    </h1>
                    <h2 class="text-2xl md:text-3xl text-gray-600 mb-8 font-medium">
                        Professional <span class="text-primary-600">Job Title</span>
                    </h2>
                    <p class="text-gray-600 mb-8 max-w-lg">
                        I create exceptional digital experiences that help businesses grow and succeed in today's competitive landscape. 
                        With a focus on quality and innovation, I deliver solutions that make an impact.
                    </p>
                    <div class="flex flex-wrap gap-4">
                        <a href="#contact" class="bg-gradient-to-r from-primary-600 to-primary-500 text-white font-medium py-3 px-8 rounded-lg hover:shadow-lg transition duration-300">
                            Get In Touch
                        </a>
                        <a href="#portfolio" class="border border-gray-300 text-gray-700 font-medium py-3 px-8 rounded-lg hover:bg-gray-100 transition duration-300">
                            View My Work
                        </a>
                    </div>
                </div>
                <div class="order-1 md:order-2 relative">
                    <div class="w-full h-80 md:h-96 bg-gradient-to-br from-primary-100 to-primary-50 rounded-2xl overflow-hidden shadow-xl">
                        <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=774&q=80" 
                             alt="Your Name" 
                             class="w-full h-full object-cover object-top">
                    </div>
                    <div class="absolute -bottom-4 -right-4 bg-white p-4 rounded-lg shadow-lg border border-gray-100">
                        <div class="flex items-center">
                            <div class="bg-green-500 w-3 h-3 rounded-full mr-2"></div>
                            <span class="text-sm font-medium">Available for work</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold text-gray-800 mb-4 section-title">About Me</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">Get to know me better - my journey, skills, and what drives me in my professional work.</p>
            </div>
            <div class="grid md:grid-cols-2 gap-12 items-center">
                <div>
                    <h3 class="text-2xl font-semibold text-gray-800 mb-6">Who I Am</h3>
                    <p class="text-gray-600 mb-6">
                        I'm a passionate professional with X years of experience in [your field]. My journey began [brief background story], 
                        and since then I've dedicated myself to mastering my craft and delivering exceptional results for clients and employers alike.
                    </p>
                    <p class="text-gray-600 mb-6">
                        What sets me apart is my commitment to [unique value proposition]. I believe in [core professional philosophy] 
                        and approach every project with [key professional traits].
                    </p>
                    <p class="text-gray-600 mb-8">
                        When I'm not working, you can find me [personal interests/hobbies]. These activities help me maintain creativity 
                        and bring fresh perspectives to my professional work.
                    </p>
                    <div class="flex space-x-4">
                        <a href="#" class="bg-primary-600 hover:bg-primary-700 text-white font-medium py-2 px-6 rounded-lg transition duration-300 flex items-center">
                            <i class="fas fa-file-alt mr-2"></i> Download CV
                        </a>
                        <a href="#" class="border border-gray-300 text-gray-700 font-medium py-2 px-6 rounded-lg hover:bg-gray-100 transition duration-300 flex items-center">
                            <i class="fab fa-linkedin-in mr-2"></i> LinkedIn
                        </a>
                    </div>
                </div>
                <div>
                    <div class="bg-gray-50 p-8 rounded-xl">
                        <h4 class="text-xl font-semibold text-gray-800 mb-6">My Skills</h4>
                        <div class="space-y-6">
                            <div>
                                <div class="flex justify-between mb-2">
                                    <span class="font-medium text-gray-700">Skill 1</span>
                                    <span class="text-gray-500">90%</span>
                                </div>
                                <div class="w-full bg-gray-200 rounded-full h-2">
                                    <div class="bg-primary-600 h-2 rounded-full" style="width: 90%"></div>
                                </div>
                            </div>
                            <div>
                                <div class="flex justify-between mb-2">
                                    <span class="font-medium text-gray-700">Skill 2</span>
                                    <span class="text-gray-500">85%</span>
                                </div>
                                <div class="w-full bg-gray-200 rounded-full h-2">
                                    <div class="bg-primary-600 h-2 rounded-full" style="width: 85%"></div>
                                </div>
                            </div>
                            <div>
                                <div class="flex justify-between mb-2">
                                    <span class="font-medium text-gray-700">Skill 3</span>
                                    <span class="text-gray-500">80%</span>
                                </div>
                                <div class="w-full bg-gray-200 rounded-full h-2">
                                    <div class="bg-primary-600 h-2 rounded-full" style="width: 80%"></div>
                                </div>
                            </div>
                            <div>
                                <div class="flex justify-between mb-2">
                                    <span class="font-medium text-gray-700">Skill 4</span>
                                    <span class="text-gray-500">75%</span>
                                </div>
                                <div class="w-full bg-gray-200 rounded-full h-2">
                                    <div class="bg-primary-600 h-2 rounded-full" style="width: 75%"></div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="py-20 bg-gray-50">
        <div class="max-w-7xl mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold text-gray-800 mb-4 section-title">My Services</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">Professional services tailored to meet your specific needs and business objectives.</p>
            </div>
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition duration-300">
                    <div class="text-primary-600 text-4xl mb-6">
                        <i class="fas fa-laptop-code"></i>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-4">Service 1</h3>
                    <p class="text-gray-600 mb-6">
                        Comprehensive description of your first service offering and how it benefits clients.
                    </p>
                    <a href="#" class="text-primary-600 hover:text-primary-700 font-medium flex items-center">
                        Learn more <i class="fas fa-arrow-right ml-2"></i>
                    </a>
                </div>
                <div class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition duration-300">
                    <div class="text-primary-600 text-4xl mb-6">
                        <i class="fas fa-mobile-alt"></i>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-4">Service 2</h3>
                    <p class="text-gray-600 mb-6">
                        Detailed explanation of your second service and the unique value it provides to customers.
                    </p>
                    <a href="#" class="text-primary-600 hover:text-primary-700 font-medium flex items-center">
                        Learn more <i class="fas fa-arrow-right ml-2"></i>
                    </a>
                </div>
                <div class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition duration-300">
                    <div class="text-primary-600 text-4xl mb-6">
                        <i class="fas fa-chart-line"></i>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-4">Service 3</h3>
                    <p class="text-gray-600 mb-6">
                        Thorough description of your third service offering and how it solves specific client problems.
                    </p>
                    <a href="#" class="text-primary-600 hover:text-primary-700 font-medium flex items-center">
                        Learn more <i class="fas fa-arrow-right ml-2"></i>
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Portfolio Section -->
    <section id="portfolio" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold text-gray-800 mb-4 section-title">My Portfolio</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">A selection of my recent work showcasing my skills and expertise.</p>
            </div>
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Project 1 -->
                <div class="bg-white rounded-xl overflow-hidden shadow-lg hover:shadow-xl transition duration-300 group">
                    <div class="h-60 bg-gray-100 relative overflow-hidden">
                        <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" 
                             alt="Project 1" 
                             class="w-full h-full object-cover group-hover:scale-105 transition duration-500">
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-gray-800 mb-2">Project Title 1</h3>
                        <p class="text-gray-600 mb-4">Brief description of the project and your role in it.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-primary-100 text-primary-800 text-xs px-3 py-1 rounded-full">Technology 1</span>
                            <span class="bg-primary-100 text-primary-800 text-xs px-3 py-1 rounded-full">Technology 2</span>
                        </div>
                        <div class="flex justify-between items-center">
                            <a href="#" class="text-primary-600 hover:text-primary-800 font-medium flex items-center">
                                View Project <i class="fas fa-arrow-right ml-2"></i>
                            </a>
                            <a href="#" class="text-gray-500 hover:text-gray-700">
                                <i class="fab fa-github"></i>
                            </a>
                        </div>
                    </div>
                </div>
                <!-- Project 2 -->
                <div class="bg-white rounded-xl overflow-hidden shadow-lg hover:shadow-xl transition duration-300 group">
                    <div class="h-60 bg-gray-100 relative overflow-hidden">
                        <img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1415&q=80" 
                             alt="Project 2" 
                             class="w-full h-full object-cover group-hover:scale-105 transition duration-500">
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-gray-800 mb-2">Project Title 2</h3>
                        <p class="text-gray-600 mb-4">Brief description of the project and your role in it.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-primary-100 text-primary-800 text-xs px-3 py-1 rounded-full">Technology 1</span>
                            <span class="bg-primary-100 text-primary-800 text-xs px-3 py-1 rounded-full">Technology 2</span>
                        </div>
                        <div class="flex justify-between items-center">
                            <a href="#" class="text-primary-600 hover:text-primary-800 font-medium flex items-center">
                                View Project <i class="fas fa-arrow-right ml-2"></i>
                            </a>
                            <a href="#" class="text-gray-500 hover:text-gray-700">
                                <i class="fab fa-github"></i>
                            </a>
                        </div>
                    </div>
                </div>
                <!-- Project 3 -->
                <div class="bg-white rounded-xl overflow-hidden shadow-lg hover:shadow-xl transition duration-300 group">
                    <div class="h-60 bg-gray-100 relative overflow-hidden">
                        <img src="https://images.unsplash.com/photo-1559028012-481c04fa702d?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1636&q=80" 
                             alt="Project 3" 
                             class="w-full h-full object-cover group-hover:scale-105 transition duration-500">
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-gray-800 mb-2">Project Title 3</h3>
                        <p class="text-gray-600 mb-4">Brief description of the project and your role in it.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-primary-100 text-primary-800 text-xs px-3 py-1 rounded-full">Technology 1</span>
                            <span class="bg-primary-100 text-primary-800 text-xs px-3 py-1 rounded-full">Technology 2</span>
                        </div>
                        <div class="flex justify-between items-center">
                            <a href="#" class="text-primary-600 hover:text-primary-800 font-medium flex items-center">
                                View Project <i class="fas fa-arrow-right ml-2"></i>
                            </a>
                            <a href="#" class="text-gray-500 hover:text-gray-700">
                                <i class="fab fa-github"></i>
                            </a>
                        </div>
                    </div>
                </div>
            </div>
            <div class="text-center mt-12">
                <a href="#" class="inline-flex items-center px-6 py-3 border border-gray-300 text-gray-700 font-medium rounded-lg hover:bg-gray-100 transition duration-300">
                    <i class="fab fa-github mr-2"></i> View All Projects
                </a>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section id="testimonials" class="py-20 bg-gray-50">
        <div class="max-w-7xl mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold text-gray-800 mb-4 section-title">Client Testimonials</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">What my clients and colleagues say about working with me.</p>
            </div>
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Testimonial 1 -->
                <div class="bg-white p-8 rounded-xl shadow-sm">
                    <div class="flex items-center mb-6">
                        <div class="w-12 h-12 rounded-full overflow-hidden mr-4">
                            <img src="https://randomuser.me/api/portraits/women/43.jpg" alt="Client 1" class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-semibold text-gray-800">Client Name 1</h4>
                            <p class="text-gray-600 text-sm">Position, Company</p>
                        </div>
                    </div>
                    <p class="text-gray-600 italic mb-6">
                        "Working with [Your Name] was an absolute pleasure. Their attention to detail and professional approach resulted in exceptional outcomes for our project."
                    </p>
                    <div class="text-yellow-400">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                </div>
                <!-- Testimonial 2 -->
                <div class="bg-white p-8 rounded-xl shadow-sm">
                    <div class="flex items-center mb-6">
                        <div class="w-12 h-12 rounded-full overflow-hidden mr-4">
                            <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="Client 2" class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-semibold text-gray-800">Client Name 2</h4>
                            <p class="text-gray-600 text-sm">Position, Company</p>
                        </div>
                    </div>
                    <p class="text-gray-600 italic mb-6">
                        "[Your Name] delivered beyond our expectations. Their expertise and communication throughout the project were outstanding."
                    </p>
                    <div class="text-yellow-400">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                </div>
                <!-- Testimonial 3 -->
                <div class="bg-white p-8 rounded-xl shadow-sm">
                    <div class="flex items-center mb-6">
                        <div class="w-12 h-12 rounded-full overflow-hidden mr-4">
                            <img src="https://randomuser.me/api/portraits/women/65.jpg" alt="Client 3" class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-semibold text-gray-800">Client Name 3</h4>
                            <p class="text-gray-600 text-sm">Position, Company</p>
                        </div>
                    </div>
                    <p class="text-gray-600 italic mb-6">
                        "I highly recommend [Your Name] for anyone looking for professional, high-quality work delivered on time and within budget."
                    </p>
                    <div class="text-yellow-400">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star-half-alt"></i>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold text-gray-800 mb-4 section-title">Get In Touch</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">Have a project in mind or want to discuss potential opportunities? I'd love to hear from you.</p>
            </div>
            <div class="grid md:grid-cols-2 gap-12">
                <div>
                    <h3 class="text-2xl font-semibold text-gray-800 mb-6">Contact Information</h3>
                    <div class="space-y-6">
                        <div class="flex items-start">
                            <div class="text-primary-600 mr-4 mt-1">
                                <i class="fas fa-envelope text-xl"></i>
                            </div>
                            <div>
                                <h4 class="text-lg font-semibold text-gray-800 mb-1">Email</h4>
                                <p class="text-gray-600">your.email@example.com</p>
                            </div>
                        </div>
                        <div class="flex items-start">
                            <div class="text-primary-600 mr-4 mt-1">
                                <i class="fas fa-phone-alt text-xl"></i>
                            </div>
                            <div>
                                <h4 class="text-lg font-semibold text-gray-800 mb-1">Phone</h4>
                                <p class="text-gray-600">+1 (555) 123-4567</p>
                            </div>
                        </div>
                        <div class="flex items-start">
                            <div class="text-primary-600 mr-4 mt-1">
                                <i class="fab fa-whatsapp text-xl"></i>
                            </div>
                            <div>
                                <h4 class="text-lg font-semibold text-gray-800 mb-1">WhatsApp</h4>
                                <a href="https://wa.me/15551234567" class="text-gray-600 hover:text-green-600 transition duration-300">+1 (555) 123-4567</a>
                            </div>
                        </div>
                        <div class="flex items-start">
                            <div class="text-primary-600 mr-4 mt-1">
                                <i class="fas fa-map-marker-alt text-xl"></i>
                            </div>
                            <div>
                                <h4 class="text-lg font-semibold text-gray-800 mb-1">Location</h4>
                                <p class="text-gray-600">Your City, Country</p>
                            </div>
                        </div>
                    </div>
                    <div class="mt-10">
                        <h4 class="text-lg font-semibold text-gray-800 mb-4">Follow Me</h4>
                        <div class="flex space-x-4">
                            <a href="#" class="bg-gray-800 text-white w-10 h-10 rounded-full flex items-center justify-center hover:bg-gray-900 transition duration-300">
                                <i class="fab fa-github"></i>
                            </a>
                            <a href="#" class="bg-blue-700 text-white w-10 h-10 rounded-full flex items-center justify-center hover:bg-blue-800 transition duration-300">
                                <i class="fab fa-linkedin-in"></i>
                            </a>
                            <a href="#" class="bg-blue-400 text-white w-10 h-10 rounded-full flex items-center justify-center hover:bg-blue-500 transition duration-300">
                                <i class="fab fa-twitter"></i>
                            </a>
                            <a href="#" class="bg-pink-600 text-white w-10 h-10 rounded-full flex items-center justify-center hover:bg-pink-700 transition duration-300">
                                <i class="fab fa-dribbble"></i>
                            </a>
                        </div>
                    </div>
                </div>
                <div>
                    <h3 class="text-2xl font-semibold text-gray-800 mb-6">Send Me a Message</h3>
                    <form class="space-y-6">
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                            <div>
                                <label for="name" class="block text-gray-700 mb-2">Your Name *</label>
                                <input type="text" id="name" required class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary-500 focus:border-primary-500 outline-none transition duration-300">
                            </div>
                            <div>
                                <label for="email" class="block text-gray-700 mb-2">Email Address *</label>
                                <input type="email" id="email" required class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary-500 focus:border-primary-500 outline-none transition duration-300">
                            </div>
                        </div>
                        <div>
                            <label for="subject" class="block text-gray-700 mb-2">Subject *</label>
                            <input type="text" id="subject" required class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary-500 focus:border-primary-500 outline-none transition duration-300">
                        </div>
                        <div>
                            <label for="message" class="block text-gray-700 mb-2">Your Message *</label>
                            <textarea id="message" rows="5" required class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary-500 focus:border-primary-500 outline-none transition duration-300"></textarea>
                        </div>
                        <button type="submit" class="bg-gradient-to-r from-primary-600 to-primary-500 text-white font-medium py-3 px-6 rounded-lg hover:shadow-lg transition duration-300 w-full">
                            Send Message
                        </button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12">
        <div class="max-w-7xl mx-auto px-6">
            <div class="grid md:grid-cols-4 gap-8">
                <div>
                    <h3 class="text-xl font-bold mb-4 gradient-text">Your Name</h3>
                    <p class="text-gray-400">Creating professional digital solutions that drive results and exceed expectations.</p>
                </div>
                <div>
                    <h4 class="text-lg font-semibold mb-4">Quick Links</h4>
                    <ul class="space-y-2">
                        <li><a href="#home" class="text-gray-400 hover:text-white transition duration-300">Home</a></li>
                        <li><a href="#about" class="text-gray-400 hover:text-white transition duration-300">About</a></li>
                        <li><a href="#services" class="text-gray-400 hover:text-white transition duration-300">Services</a></li>
                        <li><a href="#portfolio" class="text-gray-400 hover:text-white transition duration-300">Portfolio</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="text-lg font-semibold mb-4">Services</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Service 1</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Service 2</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Service 3</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Consulting</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="text-lg font-semibold mb-4">Newsletter</h4>
                    <p class="text-gray-400 mb-4">Subscribe to my newsletter for the latest updates and insights.</p>
                    <form class="flex">
                        <input type="email" placeholder="Your email" class="px-4 py-2 w-full rounded-l-lg focus:outline-none text-gray-800">
                        <button type="submit" class="bg-primary-600 hover:bg-primary-700 px-4 py-2 rounded-r-lg transition duration-300">
                            <i class="fas fa-paper-plane"></i>
                        </button>
                    </form>
                </div>
            </div>
            <div class="border-t border-gray-800 mt-10 pt-6 flex flex-col md:flex-row justify-between items-center">
                <p class="text-gray-400 text-sm">© 2023 Your Name. All rights reserved.</p>
                <div class="flex space-x-6 mt-4 md:mt-0">
                    <a href="#" class="text-gray-400 hover:text-white transition duration-300 text-sm">Privacy Policy</a>
                    <a href="#" class="text-gray-400 hover:text-white transition duration-300 text-sm">Terms of Service</a>
                </div>
            </div>
        </div>
    </footer>

    <!-- Floating WhatsApp Button -->
    <a href="https://wa.me/15551234567" 
       class="fixed bottom-6 right-6 bg-green-500 text-white w-14 h-14 rounded-full flex items-center justify-center shadow-lg hover:bg-green-600 transition duration-300 z-50"
       target="_blank">
        <i class="fab fa-whatsapp text-2xl"></i>
    </a>

    <!-- Back to Top Button -->
    <button id="back-to-top" class="fixed bottom-24 right-6 bg-primary-600 text-white w-12 h-12 rounded-full shadow-lg flex items-center justify-center opacity-0 invisible transition-all duration-300 hover:shadow-xl">
        <i class="fas fa-arrow-up"></i>
    </button>

    <!-- JavaScript -->
    <script>
        // Mobile menu toggle
        const menuBtn = document.getElementById('menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        
        menuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if (targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                    
                    // Close mobile menu if open
                    if (!mobileMenu.classList.contains('hidden')) {
                        mobileMenu.classList.add('hidden');
                    }
                }
            });
        });

        // Back to top button
        const backToTopBtn = document.getElementById('back-to-top');
        
        window.addEventListener('scroll', () => {
            if (window.pageYOffset > 300) {
                backToTopBtn.classList.remove('opacity-0', 'invisible');
                backToTopBtn.classList.add('opacity-100', 'visible');
            } else {
                backToTopBtn.classList.remove('opacity-100', 'visible');
                backToTopBtn.classList.add('opacity-0', 'invisible');
            }
        });
        
        backToTopBtn.addEventListener('click', () => {
            window.scrollTo({
                top: 0,
                behavior: 'smooth'
            });
        });

        // Form submission (prevent default)
        const form = document.querySelector('form');
        if (form) {
            form.addEventListener('submit', (e) => {
                e.preventDefault();
                alert('Thank you for your message! This is a demo form and no data will be sent.');
                form.reset();
            });
        }
    </script>
</body>
</html>
