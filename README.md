# Desarrollo-del-proyecto-U1.Avance-3-4-HTML5_etiquetas-b-sicas-estructura-de-documentos-y-sem-ntica
incorporando la estructura correcta de un documento HTML5, etiquetas básicas y elementos semánticos que permitan organizar mejor el contenido de su proyecto, emprendimiento o sistema web.
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Sistemas de Información</title>
    <style>
        body {
            background-color: #e8f5e9;
            font-family: 'Segoe UI', Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        header, nav, main, section, article, aside, footer {
            padding: 20px;
            margin: 10px;
        }
        header {
            background-color: #1b5e20;
            color: white;
            text-align: center;
        }
        nav {
            background-color: #388e3c;
            text-align: center;
        }
        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
            font-weight: bold;
        }
        section {
            background-color: #f1f8e9;
            border-radius: 6px;
            opacity: 0;
            transform: translateY(10px);
            max-height: 0;
            overflow: hidden;
            transition: opacity .35s ease, transform .35s ease, max-height .45s ease;
            pointer-events: none;
        }
        section.active {
            opacity: 1;
            transform: translateY(0);
            max-height: 1200px;
            pointer-events: auto;
        }
        aside {
            display: block;
            opacity: 0;
            transform: translateY(8px);
            max-height: 0;
            overflow: hidden;
            transition: opacity .35s ease, transform .35s ease, max-height .45s ease;
        }
        aside.active {
            opacity: 1;
            transform: translateY(0);
            max-height: 400px;
        }
        nav a.active-link {
            background-color: rgba(255,255,255,0.12);
            padding: 6px 10px;
            border-radius: 6px;
            box-shadow: 0 1px 0 rgba(0,0,0,0.06) inset;
        }
        footer {
            background-color: #1b5e20;
            color: white;
            text-align: center;
        }
        .bottom-left {
            position: fixed;
            bottom: 20px;
            left: 20px;
            width: 120px;
            border-radius: 6px;
            box-shadow: 0 2px 8px rgba(0,0,0,0.15);
        }
        /* Imagen en Quiénes Somos */
        #quienes-somos img {
            display: block;
            margin: 16px auto 0;
            max-width: 600px;
            width: 100%;
            border-radius: 8px;
        }
    </style>
</head>
<body>

    <header>
        <h1>Soluciones Tecnológicas Integrales</h1>
    </header>

    <nav>
        <a href="#inicio" data-target="inicio">Inicio</a>
        <a href="#quienes-somos" data-target="quienes-somos">Quiénes Somos</a>
        <a href="#servicios" data-target="servicios">Servicios</a>
        <a href="#contacto" data-target="contacto">Contacto</a>
    </nav>

    <main>
        <section id="inicio">
            <article>
                <h2>Inicio</h2>
                <p>Bienvenido a nuestro catálogo digital para la gestión de servicios y soporte técnico. Este proyecto busca integrar soluciones tecnológicas adaptadas a las necesidades de los usuarios.</p>
            </article>
        </section>

        <section id="quienes-somos">
            <article>
                <h2>Quiénes Somos</h2>
                <p>
                    Somos un equipo dedicado al desarrollo de sistemas de información que facilitan la gestión de servicios tecnológicos. Nuestro proyecto se centra en ofrecer herramientas digitales que permitan a empresas y usuarios organizar, controlar y optimizar sus procesos de soporte técnico. Con más de 100 palabras, esta sección describe la misión, visión y valores de nuestro emprendimiento, destacando la innovación, la accesibilidad y el compromiso con la calidad.
                </p>
                <img src="https://thf.bing.com/th/id/OIP.rhMrmWsix7Vp4CI0YnwrwQHaEU?w=313&h=182&c=7&r=0&o=7&cb=thfc1falcon2&dpr=1.5&pid=1.7&rm=3" alt="Imagen del proyecto">
            </article>
        </section>

        <section id="servicios">
            <article>
                <h2>Servicios</h2>
                <ul>
                    <li>Gestión de tickets de soporte</li>
                    <li>Catálogo digital de productos</li>
                    <li>Asistencia técnica remota</li>
                    <li>Consultoría en sistemas de información</li>
                </ul>
                <div style="max-width:900px;margin:18px auto 0;">
                    <iframe width="100%" height="500" src="https://www.youtube.com/embed/STNnG5K3jdM?start=15&rel=0" title="¿Cómo se crean las páginas web? (todas las formas)" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen loading="lazy" style="border-radius:8px;display:block;"></iframe>
                </div>
            </article>
        </section>

        <section id="contacto">
            <article>
                <h2>Contacto</h2>
                <p>Correo: jair18042007.com</p>
                <p>Teléfono: +593 963654518</p>
                <p>Dirección: Santo Domingo, Ecuador</p>
                <p>
                    Síguenos en:
                    <a href="https://www.facebook.com/share/14dKGgcFMSz/" target="_blank">Facebook</a> |
                    <a href="https://twitter.com" target="_blank">Twitter</a> |
                    <a href="https://instagram.com" target="_blank">Instagram</a>
                </p>
            </article>
        </section>

        <aside>
            <h3>Información Complementaria</h3>
            <p>Promoción vigente: 20% de descuento en servicios de consultoría.</p>
            <p>Horarios de atención: Lunes a Viernes de 9h00 a 18h00.</p>
        </aside>
    </main>

    <footer>
        <p><strong>Nombre:</strong> Cristopher Jair Robalino Montes</p>
        <p><strong>Asignatura:</strong> DESARROLLO DE APLICACIONES WEB</p>
        <p><strong>Año:</strong> 2026</p>
    </footer>

    <!-- Imagen fija en esquina inferior izquierda -->
    <img src="https://eva.pregrado.uea.edu.ec/eva2626/web/pluginfile.php/1/theme_moove/logo/1780768848/logo_eva_pregrado_2626.png" alt="Logo EVA" class="bottom-left">

    <script>
        const navLinks = document.querySelectorAll('nav a[data-target]');
        const sections = document.querySelectorAll('main section');
        const aside = document.querySelector('aside');

        function showSection(id) {
            sections.forEach(section => {
                section.classList.toggle('active', section.id === id);
            });
            if (aside) {
                aside.classList.toggle('active', id === 'contacto');
            }
            // update URL hash without jumping
            history.replaceState(null, '', '#' + id);
        }

        navLinks.forEach(link => {
            link.addEventListener('click', event => {
                event.preventDefault();
                const target = event.currentTarget.getAttribute('data-target');
                showSection(target);
                // update active link
                navLinks.forEach(l => l.classList.toggle('active-link', l === event.currentTarget));
            });
        });

        // show section based on hash or default to inicio
        const initial = location.hash ? location.hash.replace('#','') : 'inicio';
        // set active link for initial
        const initialLink = document.querySelector(`nav a[data-target="${initial}"]`);
        if (initialLink) initialLink.classList.add('active-link');
        showSection(initial);
    </script>

</body>
</html>
