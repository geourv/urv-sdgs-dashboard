# Estructura i manteniment del lloc web

Aquest repositori conté una pàgina web estàtica allotjada a **GitHub Pages**. La web es construeix amb **HTML, CSS i JavaScript** sense ús d'un servidor.

## Estructura de carpetes

```
urv-sdgs-dashboard/
│── index.html              		# Pàgina principal de la web
│── README.md               		# Documentació del projecte
│── LICENSE                 		# Llicència del repositori
│── .gitignore             		# Fitxer d'exclusions de Git
│
├── pages/                  		# Pàgines internes de la web
│   ├── about.html          		# Informació sobre el projecte
│   ├── course-details.html 		# Detalls d'assignatures
│   ├── data-code-resources.html 	# Recursos, codi i dades 
│   ├── degree-barchart.html        	# Gràfics de barres sobre ODS (ensenyaments)
│   ├── debree-wordcloud.html       	# Núvols de paraules sobre ODS (ensenyaments)
│   ├── faculty-doughnut.html       	# Gràfics de tipus donut sobre ODS (facultats)
│   ├── faculty-wordcloud.html      	# Núvols de paraules sobre ODS (facultats)
│   ├── info.html           		# Informació addicional
│   ├── methods.html        		# Explicació de la metodologia
│   ├── what-sdg-are.html   		# Explicació sobre què són els ODS
│   ├── why-monitoring-sdg.html 	# Raons per monitoritzar els ODS
│
├── data/                   		# Dades i fitxers JSON
│   ├── example.json        		# Dades d'ODS i paraules clau agrupades
│
├── downloads/             		# Fitxers descarregables (PDFs, CSV, etc.)
│
├── assets/                 		# Recursos visuals, CSS, JS...
│   ├── css/                		# Fulls d'estil
│   │   ├── styles.css      		# Full d'estil principal
│   │
│   ├── includes/           		# Fragments HTML reutilitzables
│   │   ├── head.html       		# Capçalera comuna
│   │   ├── footer.html     		# Peu de pàgina
│   │   ├── topbar.html     		# Barra superior
│   │   ├── sidebar.html    		# Barra lateral de navegació
│   │
│   ├── js/                 		# Scripts JavaScript
│   │   ├── script.js       		# Codi general per la web
│   │   ├── head-loader.js      	# Carrega la capçalera
│   │   ├── footer-loader.js    	# Carrega el peu de pàgina
│   │   ├── topbar-loader.js    	# Carrega la barra superior
│   │   ├── sidebar-loader.js   	# Carrega la barra lateral
│   │
│   ├── logos/              		# Logos d'ODS o institucionals
│   │   ├── edited/         		# Versions editades de logos
│   │   │   ├── cat/        		# Logos en català
│   │   │   │   ├── cat_ods_01.svg 	# Logotip ODS 01 en català
│
└── .git/                   		# Carpeta interna de Git

## Com utilitzar

### 1. Activar GitHub Pages
1. Ves a **Settings** → **Pages**.
2. A "Branch", selecciona **main** i la carpeta `/(root)`.
3. Guarda els canvis i accedeix a la web des de `https://nom-usuari.github.io/nom-repositori/`.

### 2. Editar el contingut
- **Treballar en local i no fer commits si la web no funciona**.
- **Modificar pàgines** → Editar o afegir fitxers `.html`. a `pages/`.
- **Afegir estils personalitzats** → Modifica `assets/css/styles.css`.
- **Carregar dades dinàmiques** → Utilitza JSON des de `data/` i carrega'l amb `fetch()` a `assets/js/script.js`.

