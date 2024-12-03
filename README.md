:root {
    --blanco: #f4f4f4;
    --darkblue: #00008B; 
    --SteelBlue: #4682B4;
    --RoyalBlue: #4169E1;
    --MediumBlue: #0000CD;
    --DarkBlue: #00008B;
    --Navy: #000080;
    --MidnightBlue: #191970;
    --negro: #3E363F;
    --gris-oscuro: #2a2a2a;
    --DarkSlateGray: #2F4F4F;
    --gris-claro: #e0e0e0;
    --fondo: #808b96;
    --sombra: rgba(0, 0, 0, 0.1);
    --sombra-dura: rgba(0, 0, 0, 0.3);
    --transicion: 0.3s;
    --animacion-duracion: 0.6s;
    --azul-Marino: #1B3A57;
    --azul-acero: #14146b;
}


body
{
    margin: 0;
    font-family: 'Lato', sans-serif;
    background: var(--gris-claro);
}

.contenedor-dashboard
{
    display: flex;
    min-height: 100vh;
}

.barra-lateral
{
    width: 250px;
    background-color: var(--azul-Marino);
    color: var(--blanco);
    display: flex;
    flex-direction: column;
}

.logo
{
    text-align: center;
    padding: 20px;
    font-size: 20px;
    font-weight: normal;
    background-color: var(--azul-Marino);
    border-bottom: 1.5px solid rgba(137, 104, 104, 0.5);
    margin: 0;
}

.logo h2
{
    font-size: 24px;
    font-family: 'Lato', sans-serif;
    font-weight: 300px;
    color: var(--gris-claro);
    margin-top: 0;
    margin-bottom: 0;
    line-height: 1.2px;
}


.menu {
    list-style-type: none;
    padding: 0;
    margin: 0;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    gap: 10px;
    background-color: var(--azul-Marino);
    border-bottom: 1px solid rgba(137, 104, 104, 0.5);
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
    transition: background-color 0.3s ease;
    height: 100vh;
    overflow-y: auto;
    position: sticky;
    top: 0;
    z-index: 1;
    overflow-x: hidden;
    max-width: 250px;
    padding-top: 30px;
    padding-bottom: 20px;
    max-height: 100vh;
}

.menu .opcion {
    padding: 15px;
    border-bottom: 1px solid var(--sombra-dura);
    text-decoration: none;
    color: var(--blanco);
    display: flex;
    align-items: center;  /* Centra verticalmente el contenido */
    justify-content: center;  /* Centra horizontalmente el contenido */
    font-size: 15px;
    transition: background-color 0.3s ease;
    gap: 10px;
    cursor: pointer;
    width: 100%;  /* Asegura que el ancho sea 100% */
    text-align: center;  /* Asegura que el texto dentro de la opción esté centrado */
}

.menu .opcion:hover {
    background-color: #4682B4; /* Azul Acero */
    color: var(--blanco);
}

.menu .opcion:active {
    background-color: #007BFF; /* Azul Eléctrico */
    color: #FFFFFF; /* Blanco Puro */
}

.menu .opcion svg {
    margin-right: 10px;  /* Ajusta el espacio entre el ícono y el texto */
    fill: var(--blanco);
    transition: fill 0.3s ease;
}



.contenedor-principal
{
    flex: 1;
    padding: 0px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.contenedor-principal h1
{
    font-size: 10px;
    font-weight: bold;
    margin-bottom: 20px;
    text-align: center;
    color: var(--blanco);
}

.contenedor-tabla
{
    overflow-x: auto;
    background-color: var(--gris-claro);
    padding: 0px;
    border-radius: 10px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    
}

table
{
    width: 100%;
    border-collapse: collapse;
    margin-top: 0px;
}

thead
{
    background-color: var(--gris-oscuro);
    color: var(--blanco);
}
th, td
{
    padding: 50px;
    text-align: center;
    border: solid 1px #3E363F;
}

tbody, tr:nth-child(even)
{
    background-color: var(--sombra);
}

tbody tr:hover
{
    background-color: var(--gris-claro);
}
button
{
    background-color: var(--gris-oscuro);
    color: var(--blanco);
    border: none;
    padding: 8px 12px;
    border-radius: 5px;
    cursor: pointer;
    font-size: 14px;
    transition: background-color 0.3s ease;
}

button:hover
{
    background-color: var(--gris-claro);
}

header {
    background-color: #111111; /* Fondo negro */
    padding: 20px;
    text-align: center;
    color: #F4F4F4; /* Gris Claro para el texto */
    font-size: 1.5rem;
    font-weight: bold;
}

/* Secciones informativas */
section {
    background-color: #F4F4F4; /* Gris Claro para el fondo de las secciones */
    padding: 40px;
    margin: 20px auto;
    max-width: 800px;
    border-radius: 8px;
    color: #1B3A57; /* Texto en Azul Marino */
}

/* Botones secundarios */
button.secondary {
    background-color: #4682B4; /* Azul Acero */
    color: #FFFFFF; /* Blanco puro */
    border: none;
    padding: 10px 20px;
    border-radius: 5px;
    cursor: pointer;
    font-size: 1rem;
    margin: 10px;
}

/* Botones principales de acción */
button.primary {
    background-color: #007BFF; /* Azul Eléctrico */
    color: #FFFFFF; /* Blanco puro */
    border: none;
    padding: 12px 24px;
    border-radius: 5px;
    cursor: pointer;
    font-size: 1rem;
    font-weight: bold;
}

/* Iconos con borde metálico */
.icon {
    border: 2px solid #C0C0C0; /* Gris Plateado para bordes */
    padding: 10px;
    display: inline-block;
    border-radius: 50%;
    margin: 10px;
}

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
    background-color: #2E3B4E; /* Azul Profundo */
    color: #FFFFFF; /* Blanco Puro */
    font-family: Arial, sans-serif;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3); /* Sombra para dar profundidad */
    border-bottom: 3px solid #4E5B6E; /* Azul Grisáceo */
}

/* Title Styles */
header h1 {
    font-size: 2rem; /* Aumenté el tamaño */
    font-weight: bold;
    color: #FFFFFF; /* Blanco Puro */
    text-transform: uppercase; /* Título en mayúsculas */
}

/* Button Container */
.button-container {
    display: flex;
    gap: 0; /* Eliminé el espacio entre los botones */
}

.titulo
{
    font-size: 2rem; /* Aumenté el tamaño */
    font-weight: bold;
    margin-bottom: 20px;
    text-align: center;
    color: var(--negro);
    text-transform: uppercase; /* Título en mayúsculas */
    margin-top: 40px; /* Aumento de margen superior para centrar el título */
    margin-bottom: 40px; /* Aumento de margen inferior para separar el título de la tabla */
    margin-bottom: 20px; /* Aumento de margen inferior para separar el título de la tabla */
    margin-top: 20px; /* Aumento de margen superior para separar el título de la tabla */
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    
}
/* Estilos para la navegación */
nav {
    background-color: var(--azul-Marino); /* Azul Marino */
    padding: 15px 30px; /* Aumento de padding para más espacio */
    display: flex;
    justify-content: space-around;
    align-items: center;
    border-bottom: 3px solid #D1D3D4; /* Gris Claro */
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3); /* Sombra para más profundidad */
}

/* Estilos de los enlaces de navegación */
nav a {
    color: #FFFFFF; /* Blanco Puro */
    text-decoration: none;
    font-size: 16px; /* Aumenté el tamaño */
    font-weight: bold;
    padding: 12px 20px; /* Botones de navegación más grandes */
    border-radius: 5px;
    transition: background-color 0.3s, color 0.3s;
}

nav a:hover {
    background-color: #4682B4; /* Azul Acero */
    color: #F4F4F4; /* Gris Claro */
}

nav a:active {
    background-color: #007BFF; /* Azul Eléctrico */
    color: #FFFFFF; /* Blanco Puro */
}



.container {
    display: flex;
    flex-wrap: wrap; /* Permite que las tarjetas se acomoden en múltiples filas si no caben */
    gap: 16px; /* Espaciado entre tarjetas */
    justify-content: center; /* Centra las tarjetas horizontalmente */
    margin: 20px;
  }
  
  /* Estilos de las tarjetas */
  .card {
    display: flex;
    flex-direction: row; /* Alineación horizontal del contenido */
    background-color: #f9f9f9;
    border: 1px solid #ddd;
    border-radius: 8px;
    overflow: hidden;
    width: 350px; /* Ancho de cada tarjeta */
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  }
  
  /* Imagen de la tarjeta */
  .card-img {
    width: 120px;
    height: 120px;
    background-color: #eaeaea;
    flex-shrink: 0; /* Mantiene el tamaño fijo de la imagen */
  }
  
  /* Información de la tarjeta */
  .card-info {
    padding: 16px;
    flex: 1; /* Toma el resto del espacio disponible */
  }
  
  .text-title {
    font-size: 18px;
    font-weight: bold;
    margin: 0 0 8px;
    color: #333;
  }
  
  .text-body {
    font-size: 14px;
    color: #666;
  }
  
  /* Pie de la tarjeta */
  .card-footer {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 8px 16px;
    border-top: 1px solid #ddd;
  }
  
  .text-title {
    color: #1a73e8;
    font-weight: bold;
  }
  
  .card-button {
    cursor: pointer;
  }
  
  .card-button svg {
    fill: #555;
    width: 20px;
    height: 20px;
  }
  
  /* Responsivo */
  @media (max-width: 768px) {
    .card {
      width: 100%; /* Ocupa todo el ancho en pantallas pequeñas */
      flex-direction: column; /* Cambia la dirección a vertical */
    }
    
    .card-img {
      width: 100%; /* Imagen ocupa todo el ancho */
      height: 200px; /* Ajusta la altura */
    }
  }



  section.how-it-works {
    background-color: #FFFFFF; /* Blanco Puro */
    padding: 20px;
    border: 1px solid #C0C0C0; /* Plateado */
    border-radius: 8px;
    max-width: 800px;
    margin: 20px auto;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

section.how-it-works h3 {
    color: #1B3A57; /* Azul Marino */
    font-size: 1.8rem;
    text-align: center;
    margin-bottom: 20px;
}

.steps {
    display: flex;
    justify-content: space-around;
    gap: 10px;
}

.step {
    text-align: center;
    flex: 1;
    background-color: #4682B4; /* Azul Acero */
    padding: 10px;
    border-radius: 8px;
    transition: transform 0.3s ease, background-color 0.3s ease;
}

.step:hover {
    background-color: #007BFF; /* Azul Eléctrico */
    transform: translateY(-5px);
}

.step img {
    width: 80px;
    height: 80px;
    margin-bottom: 10px;
    border: 2px solid #C0C0C0; /* Plateado */
    border-radius: 50%;
    background-color: #FFFFFF; /* Blanco Puro */
}

.step p {
    color: #FFFFFF; /* Blanco Puro */
    font-size: 1rem;
    margin: 0;
}



#cotizaciones {
    background-color: #F4F4F4; /* Gris Claro */
    padding: 30px;
    text-align: center;
    border-radius: 10px;
    box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
}

/* Estilo para el título */
#cotizaciones h2 {
    color: #1B3A57; /* Azul Marino */
    font-size: 2em;
    margin-bottom: 15px;
    font-weight: bold;
}

/* Estilo para el párrafo */
#cotizaciones p {
    color: #4682B4; /* Azul Acero */
    font-size: 1.1em;
    margin-bottom: 25px;
    font-weight: normal;
}

/* Estilo para el botón */
.quote-button {
    background-color: #007BFF; /* Azul Eléctrico */
    color: #FFFFFF; /* Blanco Puro */
    border: none;
    padding: 15px 30px;
    font-size: 1.1em;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s ease, transform 0.3s ease;
}

/* Efecto hover para el botón */
.quote-button:hover {
    background-color: #4682B4; /* Azul Acero */
    transform: scale(1.05);
}

/* Estilo para el borde del botón */
.quote-button:focus {
    outline: none;
    box-shadow: 0 0 0 3px #C0C0C0; /* Plateado */
}




/* Estilos generales */
#marcas {
    background-color: #F4F4F4;
    padding: 50px;
    text-align: center;
}

#marcas h2 {
    color: #1B3A57;
    font-size: 2em;
    margin-bottom: 30px;
}

/* Estilos del contenedor de marcas */
.brands {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 30px;
    padding: 0 10px;
}

/* Estilos de cada marca */

.brand {
    background-color: #FFFFFF;
    border-radius: 10px;
    border: 1px solid #C0C0C0;
    padding: 20px;
    text-align: center;
    width: 180px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease;
}

/* Efecto al pasar el cursor sobre cada marca */
.brand:hover {
    transform: translateY(-10px);
}

/* Estilos de la imagen de cada marca */
.brand img {
    max-width: 100px;
    height: auto;
    margin-bottom: 15px;
}

/* Estilos del nombre de la marca */
.brand p {
    color: #4682B4;
    font-size: 1.2em;
    font-weight: bold;
}

/* Medios de pantalla (responsividad) */
@media (max-width: 768px) {
    .brand {
        width: 150px;
    }
}

@media (max-width: 480px) {
    .brand {
        width: 120px;
    }
}
