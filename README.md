_____________________________
<h1>INICIO</h1
____________________________

<!DOCTYPE html>
<html lang="es">

<!--
    Archivo: Bienvenida/Inicio.html
    Descripción: Página de inicio de la plataforma "Ubicampus".
    Propósito: Presentación principal y acceso rápido a recursos institucionales.
    Este archivo utiliza TailwindCSS, Google Fonts y Phosphor Icons.

    Contiene las siguientes secciones:
    - Encabezado fijo (HEADER)
    - Sección principal (HERO)
    - Sección informativa "Sobre Ubicampus"
    - Pie de página (FOOTER)
-->

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ubicampus</title>
    
    <!-- Carga de TailwindCSS desde CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Fuentes personalizadas desde Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600&family=Merriweather:ital,wght@0,300;0,400;0,700;1,300&display=swap" rel="stylesheet">
    
    <!-- Iconos de Phosphor Icons -->
    <script src="https://unpkg.com/@phosphor-icons/web"></script>

    <!-- Configuración personalizada de TailwindCSS -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    // Colores personalizados para identidad de Ubicampus
                    colors: {
                        'ub-blue': '#002855',
                        'ub-dark': '#021730',
                    },
                    // Familias de fuentes globales
                    fontFamily: {
                        serif: ['Merriweather', 'serif'],
                        sans: ['Inter', 'sans-serif'],
                    }
                }
            }
        }
    </script>
</head>

<body class="bg-white font-sans text-gray-900 overflow-x-hidden">

    <!-- ================================================ -->
    <!-- CABECERA (HEADER) -->
    <!-- Barra superior fija con logo, enlaces y menú -->
    <!-- ================================================ -->
    <header class="fixed top-0 left-0 w-full z-50 flex justify-between items-start">
        
        <!-- Grupo Izquierdo: Logo + Enlaces -->
        <div class="flex flex-col md:flex-row md:items-center bg-white/95 backdrop-blur-md p-4 pr-8 rounded-br-xl shadow-sm md:shadow-none md:bg-transparent transition-all duration-300">
            
            <!-- Logo: Regresa a Inicio -->
            <a href="Inicio.html" class="flex items-center gap-3 mr-8 group">
                
                <!-- Caja del logo (UPEN) -->
                <div class="bg-ub-blue text-white w-20 h-14 flex items-center justify-center font-bold text-xl rounded-lg shadow-lg group-hover:scale-105 transition duration-300 overflow-hidden">
                    <span>UPEN</span>
                </div>
                
                <!-- Texto de marca -->
                <div class="flex flex-col leading-none">
                    <span class="font-serif font-bold text-xl text-ub-blue tracking-tight">Ubicampus</span>
                    <span class="text-xs text-gray-500 font-sans tracking-widest uppercase mt-1">Universidad</span>
                </div>
            </a>

            <!-- Navegación: Página oficial y Moodle -->
            <div class="flex items-center gap-8">
                
                <!-- Enlace a la página oficial UPEN -->
                <a href="https://upnay.edu.mx/" target="_blank" class="hidden md:flex items-center text-sm font-medium text-gray-600 hover:text-ub-blue hover:underline transition pl-4 md:border-l border-gray-300">
                    <!-- Indicador verde animado -->
                    <span class="w-2 h-2 bg-green-500 rounded-full mr-2 animate-pulse"></span>
                    Ir a Página Oficial UPEN
                    <!-- Icono flecha -->
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4 ml-1">
                        <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 19.5 15-15m0 0H8.25m11.25 0v11.25" />
                    </svg>
                </a>

                <!-- Enlace a Moodle -->
                <a href="https://upnay.edu.mx/mupen/login/index.php" target="_blank" class="group flex items-center gap-2 text-gray-600 hover:text-[#0f2545] transition-colors">
                    <span class="w-2 h-2 bg-blue-500 rounded-full"></span>
                    <span class="font-medium">Moodle</span>
                    <!-- Icono flecha -->
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4 text-gray-400 group-hover:text-[#0f2545]">
                        <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 19.5 15-15m0 0H8.25m11.25 0v11.25" />
                    </svg>
                </a>
            </div> 
        </div> 

        <!-- Grupo Derecho: Menú Azul -->
        <div class="bg-ub-blue text-white flex items-stretch h-16 md:h-20 shadow-2xl rounded-bl-xl overflow-hidden">
            
            <!-- Acceso al menú de usuario -->
            <a href="menu.html" class="flex items-center gap-2 px-6 hover:bg-ub-dark transition border-r border-white/10">
                <i class="ph ph-user-circle text-2xl"></i>
                <span class="font-semibold hidden md:inline">Acceso</span>
            </a>

            <!-- Botón hamburguesa (menú) -->
            <button class="flex items-center gap-2 px-6 hover:bg-ub-dark transition group">
                <!-- Líneas del icono -->
                <div class="flex flex-col items-end gap-1.5 group-hover:gap-2 transition-all duration-300">
                    <span class="w-6 h-0.5 bg-white"></span>
                    <span class="w-4 h-0.5 bg-white"></span>
                    <span class="w-6 h-0.5 bg-white"></span>
                </div>
            </button>
        </div>
    </header>

    <!-- ================================================ -->
    <!-- SECCIÓN HERO (Presentación principal) -->
    <!-- Incluye imagen de fondo, títulos y lema -->
    <!-- ================================================ -->
    <main class="relative w-full min-h-screen flex flex-col justify-center items-center text-center pt-20 pb-20 overflow-hidden">
        
        <!-- Imagen de fondo con fallback -->
        <div class="absolute top-0 left-0 w-full h-full z-0 pointer-events-none">
            <img src="/img/Upen dron.jpeg"
                 onerror="this.src='https://images.unsplash.com/photo-1541339907198-e08756dedf3f?q=80&w=1470&auto=format&fit=crop'"
                 alt="University Campus"
                 class="w-full h-[90%] object-cover object-center opacity-90 blur-sm">
        </div>

        <!-- Gradiente blanco para mayor legibilidad -->
        <div class="absolute top-0 left-0 w-full h-[90%] z-10 bg-gradient-to-b from-white/30 via-white/60 to-white pointer-events-none"></div>

        <!-- Contenido principal del hero -->
        <div class="relative z-20 px-4 max-w-4xl mx-auto mt-10">
            
            <!-- Títulos y lema -->
            <div class="fade-in-up" style="animation-delay: 0.1s;">
                <h2 class="font-sans font-light text-ub-blue uppercase tracking-[0.2em] text-sm mb-4">Plataforma Universitaria</h2>
                
                <!-- Título principal -->
                <h1 class="font-serif text-5xl md:text-7xl lg:text-8xl text-gray-900 tracking-tight leading-none mb-2">
                    Welcome to <br>
                    <span class="text-transparent bg-clip-text bg-gradient-to-r from-ub-blue to-blue-600">Ubicampus</span>
                </h1>

                <!-- Lema -->
                <p class="font-serif italic text-2xl text-gray-600 mt-4">"Aprende y conecta"</p>
            </div>

            <!-- Elemento de retroalimentación (oculto por defecto) -->
            <p id="searchFeedback" class="text-red-500 font-medium mt-3 hidden text-sm bg-white/80 inline-block px-3 py-1 rounded-full shadow-sm"></p>
        </div>

        <!-- Indicador de scroll -->
        <div class="absolute bottom-10 left-1/2 -translate-x-1/2 z-20 animate-bounce text-ub-blue/50">
            <i class="ph ph-caret-down text-3xl"></i>
        </div>

    </main>

    <!-- ================================================ -->
    <!-- SECCIÓN SOBRE UBICAMPUS -->
    <!-- Información descriptiva acerca del proyecto -->
    <!-- ================================================ -->
    <section class="relative z-20 bg-white px-6 pb-24">
        <div class="max-w-5xl mx-auto">
            <div class="border-l-4 border-ub-blue pl-8 py-2 mb-16">
                
                <!-- Título de sección -->
                <h3 class="font-serif text-3xl md:text-4xl font-bold text-gray-900 mb-6">Sobre Ubicampus</h3>
                
                <!-- Descripción -->
                <p class="text-lg md:text-xl text-gray-700 leading-relaxed font-light">
                    Ubicampus es una plataforma diseñada para mejorar la experiencia académica,
                    administrativa y social dentro de una universidad moderna. Su objetivo es facilitar
                    procesos, optimizar tiempos y brindar herramientas tecnológicas a estudiantes,
                    profesores y personal administrativo así como dar a conocer las diferentes áreas del campus.
                </p>
            </div>
        </div>
    </section>

    <!-- ================================================ -->
    <!-- PIE DE PÁGINA -->
    <!-- ================================================ -->
    <footer class="bg-ub-blue text-white py-12 text-center border-t border-white/10">
        
        <!-- Marca o firma final -->
        <div class="flex items-center justify-center gap-3 mb-4 opacity-80">
            <i class="ph ph-student text-2xl"></i>
            <span class="font-serif text-xl tracking-wide">Ubicampus</span>
        </div>
    </footer>

</body>
</html>
