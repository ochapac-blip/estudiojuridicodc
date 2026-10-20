<!DOCTYPE html>
<html lang="es" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Estudio Jurídico DC | Abogados</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Tailwind Config for Custom Colors/Fonts -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        navy: {
                            800: '#1e293b', // slate-800
                            900: '#0f172a', // slate-900
                        },
                        gold: {
                            400: '#fbbf24', // amber-400
                            500: '#f59e0b', // amber-500
                            600: '#d97706', // amber-600
                        }
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        serif: ['Playfair Display', 'serif'],
                    }
                }
            }
        }
    </script>
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&family=Playfair+Display:wght@400;600;700&display=swap" rel="stylesheet">
    <!-- FontAwesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* Custom Styles for Hero Overlay */
        .hero-bg {
            background-image: linear-gradient(rgba(15, 23, 42, 0.8), rgba(15, 23, 42, 0.8)), url('https://images.unsplash.com/photo-1589829085413-56de8ae18c73?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
        }
    </style>
</head>
<body class="font-sans text-gray-800 bg-gray-50 flex flex-col min-h-screen">

    <!-- Navigation -->
    <nav class="fixed w-full z-50 transition-all duration-300" id="navbar">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-20">
                <!-- Logo -->
                <div class="flex-shrink-0 flex items-center">
                    <a href="#home" class="font-serif text-2xl font-bold text-white flex items-center gap-2">
                        <i class="fa-solid fa-scale-balanced text-gold-500"></i>
                        <span>Estudio Jurídico <span class="text-gold-500">DC</span></span>
                    </a>
                </div>

                <!-- Desktop Menu -->
                <div class="hidden md:flex items-center space-x-8">
                    <a href="#home" class="text-gray-300 hover:text-gold-400 transition-colors duration-200 font-medium">Inicio</a>
                    <a href="#about" class="text-gray-300 hover:text-gold-400 transition-colors duration-200 font-medium">Nosotros</a>
                    <a href="#services" class="text-gray-300 hover:text-gold-400 transition-colors duration-200 font-medium">Servicios</a>
                    <a href="#contact" class="text-gray-300 hover:text-gold-400 transition-colors duration-200 font-medium">Contacto</a>
                    <a href="#contact" class="bg-gold-500 hover:bg-gold-600 text-navy-900 px-5 py-2 rounded-sm font-semibold transition-colors duration-200 shadow-lg">Consulta Gratuita</a>
                </div>

                <!-- Mobile Menu Button -->
                <div class="md:hidden flex items-center">
                    <button id="mobile-menu-btn" class="text-gray-300 hover:text-white focus:outline-none">
                        <i class="fa-solid fa-bars text-2xl"></i>
                    </button>
                </div>
            </div>
        </div>

        <!-- Mobile Menu (Hidden by default) -->
        <div id="mobile-menu" class="hidden md:hidden bg-navy-900 border-t border-gray-700 absolute w-full shadow-xl">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                <a href="#home" class="mobile-link block px-3 py-2 rounded-md text-base font-medium text-gray-300 hover:text-gold-400 hover:bg-navy-800">Inicio</a>
                <a href="#about" class="mobile-link block px-3 py-2 rounded-md text-base font-medium text-gray-300 hover:text-gold-400 hover:bg-navy-800">Nosotros</a>
                <a href="#services" class="mobile-link block px-3 py-2 rounded-md text-base font-medium text-gray-300 hover:text-gold-400 hover:bg-navy-800">Servicios</a>
                <a href="#contact" class="mobile-link block px-3 py-2 rounded-md text-base font-medium text-gray-300 hover:text-gold-400 hover:bg-navy-800">Contacto</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero-bg h-screen flex items-center justify-center pt-20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h1 class="text-4xl sm:text-5xl md:text-6xl font-serif font-bold text-white leading-tight mb-6 animate-fade-in-up">
                Defendiendo sus derechos con <br class="hidden md:block"/>
                <span class="text-gold-500">Integridad y Excelencia</span>
            </h1>
            <p class="mt-4 text-lg sm:text-xl text-gray-300 max-w-3xl mx-auto mb-10 font-light">
                Más de 20 años de experiencia brindando asesoría legal estratégica y soluciones efectivas para empresas y particulares. Su tranquilidad es nuestra prioridad.
            </p>
            <div class="flex flex-col sm:flex-row justify-center gap-4">
                <a href="#contact" class="bg-gold-500 hover:bg-gold-600 text-navy-900 font-semibold py-3 px-8 rounded-sm text-lg transition-all shadow-lg hover:shadow-xl hover:-translate-y-1">
                    Agendar Asesoría
                </a>
                <a href="#services" class="bg-transparent border-2 border-white text-white hover:bg-white hover:text-navy-900 font-semibold py-3 px-8 rounded-sm text-lg transition-all">
                    Nuestras Áreas de Práctica
                </a>
            </div>
        </div>
    </section>

    <!-- About Us Section -->
    <section id="about" class="py-24 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex flex-col lg:flex-row items-center gap-16">
                <div class="lg:w-1/2">
                    <div class="relative">
                        <img src="https://images.unsplash.com/photo-1505664177941-44dc4c33d59e?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Oficina Legal" class="rounded-sm shadow-2xl z-10 relative">
                        <div class="absolute -bottom-6 -right-6 w-full h-full border-4 border-gold-500 rounded-sm z-0"></div>
                        <!-- Experience Badge -->
                        <div class="absolute -top-8 -left-8 bg-navy-900 text-white p-6 rounded-sm shadow-xl z-20 hidden md:block">
                            <span class="block text-4xl font-serif font-bold text-gold-500">20+</span>
                            <span class="block text-sm uppercase tracking-wider mt-1">Años de<br>Experiencia</span>
                        </div>
                    </div>
                </div>
                <div class="lg:w-1/2">
                    <div class="flex items-center gap-4 mb-4">
                        <div class="h-[2px] w-12 bg-gold-500"></div>
                        <span class="text-gold-600 font-semibold uppercase tracking-wider text-sm">Sobre Nosotros</span>
                    </div>
                    <h2 class="text-3xl md:text-4xl font-serif font-bold text-navy-900 mb-6">Comprometidos con la Justicia y el Éxito de Nuestros Clientes</h2>
                    <p class="text-gray-600 mb-6 leading-relaxed">
                        En el Estudio Jurídico DC, entendemos que enfrentar un problema legal puede ser abrumador. Por eso, nuestro equipo de abogados altamente calificados se dedica a brindar un servicio personalizado, transparente y orientado a resultados.
                    </p>
                    <p class="text-gray-600 mb-8 leading-relaxed">
                        Nos enorgullece nuestra ética de trabajo rigurosa y nuestro profundo conocimiento de la ley. Ya sea que representemos a una gran corporación o a un individuo en una disputa familiar, aplicamos la misma dedicación y agresividad táctica para proteger sus intereses.
                    </p>
                    
                    <div class="grid grid-cols-2 gap-6">
                        <div class="flex items-start gap-3">
                            <i class="fa-solid fa-check-circle text-gold-500 mt-1"></i>
                            <div>
                                <h4 class="font-bold text-navy-900">Estrategia Legal</h4>
                                <p class="text-sm text-gray-500">Soluciones a medida</p>
                            </div>
                        </div>
                        <div class="flex items-start gap-3">
                            <i class="fa-solid fa-check-circle text-gold-500 mt-1"></i>
                            <div>
                                <h4 class="font-bold text-navy-900">Confidencialidad</h4>
                                <p class="text-sm text-gray-500">Absoluta reserva</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="py-24 bg-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <div class="flex items-center justify-center gap-4 mb-4">
                    <div class="h-[2px] w-12 bg-gold-500"></div>
                    <span class="text-gold-600 font-semibold uppercase tracking-wider text-sm">Áreas de Práctica</span>
                    <div class="h-[2px] w-12 bg-gold-500"></div>
                </div>
                <h2 class="text-3xl md:text-4xl font-serif font-bold text-navy-900 mb-6">Nuestros Servicios Legales</h2>
                <p class="text-gray-600">Ofrecemos representación legal integral en diversas áreas del derecho, respaldada por años de experiencia y un profundo conocimiento jurídico.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
                <!-- Service 1: Corporate -->
                <div class="bg-white p-8 rounded-sm shadow-md hover:shadow-xl transition-shadow duration-300 border-b-4 border-transparent hover:border-gold-500 group">
                    <div class="w-14 h-14 bg-navy-50 rounded-full flex items-center justify-center mb-6 group-hover:bg-gold-50 transition-colors">
                        <i class="fa-solid fa-building text-2xl text-navy-900 group-hover:text-gold-600 transition-colors"></i>
                    </div>
                    <h3 class="text-xl font-serif font-bold text-navy-900 mb-3">Derecho Corporativo</h3>
                    <p class="text-gray-600 text-sm leading-relaxed mb-4">
                        Asesoramiento integral para empresas, desde la constitución de sociedades hasta fusiones, adquisiciones y contratos comerciales complejos.
                    </p>
                    <a href="#contact" class="text-gold-600 font-medium text-sm hover:text-navy-900 flex items-center gap-2">
                        Saber más <i class="fa-solid fa-arrow-right text-xs"></i>
                    </a>
                </div>

                <!-- Service 2: Family -->
                <div class="bg-white p-8 rounded-sm shadow-md hover:shadow-xl transition-shadow duration-300 border-b-4 border-transparent hover:border-gold-500 group">
                    <div class="w-14 h-14 bg-navy-50 rounded-full flex items-center justify-center mb-6 group-hover:bg-gold-50 transition-colors">
                        <i class="fa-solid fa-people-roof text-2xl text-navy-900 group-hover:text-gold-600 transition-colors"></i>
                    </div>
                    <h3 class="text-xl font-serif font-bold text-navy-900 mb-3">Derecho de Familia</h3>
                    <p class="text-gray-600 text-sm leading-relaxed mb-4">
                        Manejo compasivo y efectivo de divorcios, custodia de menores, pensiones alimenticias y acuerdos prenupciales.
                    </p>
                    <a href="#contact" class="text-gold-600 font-medium text-sm hover:text-navy-900 flex items-center gap-2">
                        Saber más <i class="fa-solid fa-arrow-right text-xs"></i>
                    </a>
                </div>

                <!-- Service 3: Criminal -->
                <div class="bg-white p-8 rounded-sm shadow-md hover:shadow-xl transition-shadow duration-300 border-b-4 border-transparent hover:border-gold-500 group">
                    <div class="w-14 h-14 bg-navy-50 rounded-full flex items-center justify-center mb-6 group-hover:bg-gold-50 transition-colors">
                        <i class="fa-solid fa-gavel text-2xl text-navy-900 group-hover:text-gold-600 transition-colors"></i>
                    </div>
                    <h3 class="text-xl font-serif font-bold text-navy-900 mb-3">Defensa Penal</h3>
                    <p class="text-gray-600 text-sm leading-relaxed mb-4">
                        Defensa vigorosa y estratégica ante acusaciones penales, protegiendo sus derechos constitucionales en cada etapa del proceso.
                    </p>
                    <a href="#contact" class="text-gold-600 font-medium text-sm hover:text-navy-900 flex items-center gap-2">
                        Saber más <i class="fa-solid fa-arrow-right text-xs"></i>
                    </a>
                </div>

                <!-- Service 4: Real Estate -->
                <div class="bg-white p-8 rounded-sm shadow-md hover:shadow-xl transition-shadow duration-300 border-b-4 border-transparent hover:border-gold-500 group">
                    <div class="w-14 h-14 bg-navy-50 rounded-full flex items-center justify-center mb-6 group-hover:bg-gold-50 transition-colors">
                        <i class="fa-solid fa-house-chimney text-2xl text-navy-900 group-hover:text-gold-600 transition-colors"></i>
                    </div>
                    <h3 class="text-xl font-serif font-bold text-navy-900 mb-3">Bienes Raíces</h3>
                    <p class="text-gray-600 text-sm leading-relaxed mb-4">
                        Asistencia legal en la compraventa de propiedades, disputas de arrendamiento, zonificación y desarrollo inmobiliario.
                    </p>
                    <a href="#contact" class="text-gold-600 font-medium text-sm hover:text-navy-900 flex items-center gap-2">
                        Saber más <i class="fa-solid fa-arrow-right text-xs"></i>
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Call to Action Banner -->
    <section class="bg-gold-500 py-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col md:flex-row items-center justify-between">
            <div class="text-center md:text-left mb-6 md:mb-0">
                <h2 class="text-3xl font-serif font-bold text-navy-900 mb-2">¿Necesita asistencia legal inmediata?</h2>
                <p class="text-navy-800 font-medium">Nuestro equipo está listo para evaluar su caso.</p>
            </div>
            <div>
                <a href="tel:+1234567890" class="inline-flex items-center gap-3 bg-navy-900 text-white font-bold py-4 px-8 rounded-sm hover:bg-navy-800 transition-colors shadow-lg">
                    <i class="fa-solid fa-phone text-gold-500"></i> (555) 123-4567
                </a>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-24 bg-white relative">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-16">
                <!-- Contact Info -->
                <div>
                    <div class="flex items-center gap-4 mb-4">
                        <div class="h-[2px] w-12 bg-gold-500"></div>
                        <span class="text-gold-600 font-semibold uppercase tracking-wider text-sm">Contáctenos</span>
                    </div>
                    <h2 class="text-3xl md:text-4xl font-serif font-bold text-navy-900 mb-6">Póngase en Contacto con Nosotros</h2>
                    <p class="text-gray-600 mb-10 leading-relaxed">
                        Complete el formulario a continuación o comuníquese directamente con nuestras oficinas. Ofrecemos una evaluación inicial gratuita de su caso. Todas las comunicaciones son estrictamente confidenciales.
                    </p>

                    <div class="space-y-6">
                        <div class="flex items-start gap-4">
                            <div class="w-12 h-12 bg-navy-50 rounded-full flex items-center justify-center flex-shrink-0">
                                <i class="fa-solid fa-location-dot text-gold-600 text-xl"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-navy-900 mb-1">Nuestra Oficina</h4>
                                <p class="text-gray-600 text-sm">Av. Principal 1234, Piso 5<br>Distrito Financiero, Ciudad 10001</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start gap-4">
                            <div class="w-12 h-12 bg-navy-50 rounded-full flex items-center justify-center flex-shrink-0">
                                <i class="fa-solid fa-envelope text-gold-600 text-xl"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-navy-900 mb-1">Correo Electrónico</h4>
                                <p class="text-gray-600 text-sm">contacto@estudiodc.com<br>info@estudiodc.com</p>
                            </div>
                        </div>

                        <div class="flex items-start gap-4">
                            <div class="w-12 h-12 bg-navy-50 rounded-full flex items-center justify-center flex-shrink-0">
                                <i class="fa-solid fa-phone text-gold-600 text-xl"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-navy-900 mb-1">Teléfonos</h4>
                                <p class="text-gray-600 text-sm">+1 (555) 123-4567<br>+1 (555) 987-6543</p>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Contact Form -->
                <div class="bg-navy-900 p-8 md:p-10 rounded-sm shadow-2xl">
                    <h3 class="text-2xl font-serif font-bold text-white mb-6">Solicitar Evaluación</h3>
                    <form id="contactForm" class="space-y-4">
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                            <div>
                                <label for="firstName" class="block text-sm font-medium text-gray-300 mb-1">Nombre</label>
                                <input type="text" id="firstName" class="w-full bg-navy-800 border border-gray-700 rounded-sm px-4 py-2 text-white focus:outline-none focus:border-gold-500 focus:ring-1 focus:ring-gold-500 transition-colors" placeholder="Su nombre" required>
                            </div>
                            <div>
                                <label for="lastName" class="block text-sm font-medium text-gray-300 mb-1">Apellido</label>
                                <input type="text" id="lastName" class="w-full bg-navy-800 border border-gray-700 rounded-sm px-4 py-2 text-white focus:outline-none focus:border-gold-500 focus:ring-1 focus:ring-gold-500 transition-colors" placeholder="Su apellido" required>
                            </div>
                        </div>
                        <div>
                            <label for="email" class="block text-sm font-medium text-gray-300 mb-1">Correo Electrónico</label>
                            <input type="email" id="email" class="w-full bg-navy-800 border border-gray-700 rounded-sm px-4 py-2 text-white focus:outline-none focus:border-gold-500 focus:ring-1 focus:ring-gold-500 transition-colors" placeholder="ejemplo@correo.com" required>
                        </div>
                        <div>
                            <label for="phone" class="block text-sm font-medium text-gray-300 mb-1">Teléfono</label>
                            <input type="tel" id="phone" class="w-full bg-navy-800 border border-gray-700 rounded-sm px-4 py-2 text-white focus:outline-none focus:border-gold-500 focus:ring-1 focus:ring-gold-500 transition-colors" placeholder="(555) 000-0000">
                        </div>
                        <div>
                            <label for="service" class="block text-sm font-medium text-gray-300 mb-1">Área de Interés</label>
                            <select id="service" class="w-full bg-navy-800 border border-gray-700 rounded-sm px-4 py-2 text-white focus:outline-none focus:border-gold-500 focus:ring-1 focus:ring-gold-500 transition-colors">
                                <option value="corporativo">Derecho Corporativo</option>
                                <option value="familia">Derecho de Familia</option>
                                <option value="penal">Defensa Penal</option>
                                <option value="bienes">Bienes Raíces</option>
                                <option value="otro">Otro</option>
                            </select>
                        </div>
                        <div>
                            <label for="message" class="block text-sm font-medium text-gray-300 mb-1">Mensaje</label>
                            <textarea id="message" rows="4" class="w-full bg-navy-800 border border-gray-700 rounded-sm px-4 py-2 text-white focus:outline-none focus:border-gold-500 focus:ring-1 focus:ring-gold-500 transition-colors" placeholder="Describa brevemente su situación..." required></textarea>
                        </div>
                        <button type="submit" class="w-full bg-gold-500 hover:bg-gold-600 text-navy-900 font-bold py-3 px-4 rounded-sm transition-colors mt-4">
                            Enviar Mensaje
                        </button>
                    </form>
                    <!-- Form Status Message Placeholder -->
                    <div id="formStatus" class="hidden mt-4 p-3 rounded-sm text-sm font-medium text-center"></div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-navy-900 pt-16 pb-8 border-t border-gray-800 mt-auto">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-12 mb-12">
                <div class="col-span-1 md:col-span-1">
                    <a href="#home" class="font-serif text-2xl font-bold text-white flex items-center gap-2 mb-4">
                        <i class="fa-solid fa-scale-balanced text-gold-500"></i>
                        <span>DC</span>
                    </a>
                    <p class="text-gray-400 text-sm leading-relaxed mb-6">
                        Representación legal de excelencia con integridad, dedicación y resultados comprobados a lo largo de más de dos décadas.
                    </p>
                    <div class="flex space-x-4">
                        <a href="#" class="w-8 h-8 rounded-full bg-navy-800 flex items-center justify-center text-gray-400 hover:text-white hover:bg-gold-600 transition-all"><i class="fa-brands fa-linkedin-in"></i></a>
                        <a href="#" class="w-8 h-8 rounded-full bg-navy-800 flex items-center justify-center text-gray-400 hover:text-white hover:bg-gold-600 transition-all"><i class="fa-brands fa-twitter"></i></a>
                        <a href="#" class="w-8 h-8 rounded-full bg-navy-800 flex items-center justify-center text-gray-400 hover:text-white hover:bg-gold-600 transition-all"><i class="fa-brands fa-facebook-f"></i></a>
                    </div>
                </div>
                
                <div>
                    <h4 class="text-white font-bold mb-4">Enlaces Rápidos</h4>
                    <ul class="space-y-2 text-sm text-gray-400">
                        <li><a href="#home" class="hover:text-gold-500 transition-colors">Inicio</a></li>
                        <li><a href="#about" class="hover:text-gold-500 transition-colors">Sobre Nosotros</a></li>
                        <li><a href="#services" class="hover:text-gold-500 transition-colors">Áreas de Práctica</a></li>
                        <li><a href="#contact" class="hover:text-gold-500 transition-colors">Contacto</a></li>
                    </ul>
                </div>

                <div>
                    <h4 class="text-white font-bold mb-4">Servicios</h4>
                    <ul class="space-y-2 text-sm text-gray-400">
                        <li><a href="#" class="hover:text-gold-500 transition-colors">Derecho Corporativo</a></li>
                        <li><a href="#" class="hover:text-gold-500 transition-colors">Derecho de Familia</a></li>
                        <li><a href="#" class="hover:text-gold-500 transition-colors">Defensa Penal</a></li>
                        <li><a href="#" class="hover:text-gold-500 transition-colors">Bienes Raíces</a></li>
                    </ul>
                </div>

                <div>
                    <h4 class="text-white font-bold mb-4">Horario de Atención</h4>
                    <ul class="space-y-2 text-sm text-gray-400">
                        <li class="flex justify-between"><span>Lunes - Viernes:</span> <span>9:00 AM - 6:00 PM</span></li>
                        <li class="flex justify-between"><span>Sábado:</span> <span>Con cita previa</span></li>
                        <li class="flex justify-between"><span>Domingo:</span> <span>Cerrado</span></li>
                    </ul>
                    <p class="text-xs text-gray-500 mt-4 italic">* Servicio de emergencias penales 24/7 disponible para clientes.</p>
                </div>
            </div>
            
            <div class="border-t border-gray-800 pt-8 flex flex-col md:flex-row justify-between items-center text-sm text-gray-500">
                <p>&copy; 2026 Estudio Jurídico DC. Todos los derechos reservados.</p>
                <div class="flex space-x-4 mt-4 md:mt-0">
                    <a href="#" class="hover:text-white transition-colors">Política de Privacidad</a>
                    <a href="#" class="hover:text-white transition-colors">Términos de Servicio</a>
                </div>
            </div>
        </div>
    </footer>

    <!-- JavaScript Interactions -->
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            // Navbar scroll effect
            const navbar = document.getElementById('navbar');
            window.addEventListener('scroll', () => {
                if (window.scrollY > 50) {
                    navbar.classList.add('bg-navy-900', 'shadow-lg');
                    navbar.classList.remove('bg-transparent');
                } else {
                    navbar.classList.remove('bg-navy-900', 'shadow-lg');
                    navbar.classList.add('bg-transparent');
                }
            });

            // Trigger initial scroll check
            window.dispatchEvent(new Event('scroll'));

            // Mobile menu toggle
            const btn = document.getElementById('mobile-menu-btn');
            const menu = document.getElementById('mobile-menu');
            const mobileLinks = document.querySelectorAll('.mobile-link');

            btn.addEventListener('click', () => {
                menu.classList.toggle('hidden');
                // Change icon
                const icon = btn.querySelector('i');
                if(menu.classList.contains('hidden')){
                    icon.classList.remove('fa-xmark');
                    icon.classList.add('fa-bars');
                } else {
                    icon.classList.remove('fa-bars');
                    icon.classList.add('fa-xmark');
                }
            });

            // Close mobile menu when a link is clicked
            mobileLinks.forEach(link => {
                link.addEventListener('click', () => {
                    menu.classList.add('hidden');
                    btn.querySelector('i').classList.remove('fa-xmark');
                    btn.querySelector('i').classList.add('fa-bars');
                });
            });

            // Form submission simulation
            const form = document.getElementById('contactForm');
            const formStatus = document.getElementById('formStatus');

            form.addEventListener('submit', (e) => {
                e.preventDefault();
                
                // Show simulated success message
                formStatus.classList.remove('hidden', 'bg-red-100', 'text-red-700');
                formStatus.classList.add('block', 'bg-green-100', 'text-green-800');
                formStatus.textContent = '¡Gracias! Su mensaje ha sido enviado correctamente. Nos pondremos en contacto a la brevedad.';
                
                // Reset form
                form.reset();
                
                // Hide message after 5 seconds
                setTimeout(() => {
                    formStatus.classList.add('hidden');
                    formStatus.classList.remove('block');
                }, 5000);
            });
        });
    </script>
</body>
</html>
