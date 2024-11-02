<script>
    import Logo from './Logo_sin_fondo.png';
</script>

<style>
    
	.all {
		margin: 0;
		padding: 0;
		text-decoration: none;
		border: none;
		outline: none;
		font-family: 'Poppins', sans-serif;
		font-size: 10px;
		width: 100%;
		height: 100vh;
		overflow-x: hidden;
		background-color: black;
		color: white;
	}

    
	span {
		color: #b74b4b;
	}

    .container {
        display: grid;
        grid-template-columns: repeat(2, 1fr); /* Dos columnas */
        gap: 20px; /* Espacio entre tarjetas */
        justify-content: center;
        margin-top: 100px;
        padding: 20px;
    }

    .card {
        background-color: #000000;
        color: #ffffff;
        padding: 20px;
        border-radius: 5px;
        box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        display: flex;
        align-items: center;
        gap: 20px;
    }

    .image-container {
        width: 150px;
        height: 200px;
        background-color: #ddd;
        border-radius: 5px;
    }

    .card-content {
        display: flex;
        flex-direction: column;
    }

    .card-title {
        font-size: 24px;
        font-weight: bold;
        margin-bottom: 10px;
    }

    .card-description {
        font-size: 16px;
        line-height: 1.5;
        margin-bottom: 20px;
    }

    
	.btn {
		display: inline-block;
		padding: 1rem 2.8rem;
		background-color: black;
		border-radius: 4rem;
		font-size: 1.6rem;
		color: #b74b4b;
		letter-spacing: 0.3rem;
		font-weight: 600;
		border: 2px solid #b74b4b;
		transition: 0.3s ease;
		cursor: pointer;
	}

	.btn:hover {
		transform: scale3d(1.03);
		background-color: #b74b4b;
		color: black;
		box-shadow: 0 0 25px #b74b4b;
	}

    .header {
		margin-top: 20px;
		position: fixed;
		top: 0;
		left: 0;
		width: 100%;
		padding: 1rem 9%;
		background-color: transparent;
		filter: drop-shadow(10px);
		display: flex;
		justify-content: space-between;
		align-items: center;
		z-index: 100;
	}

    
	nav a {
		font-size: 20px;
		color: white;
		margin-left: 4rem;
		font-weight: 500;
		transition: 0.3s ease;
		border-bottom: 3px solid transparent;
	}

	nav a:hover,
	nav a.active {
		color: #b74b4b;
		border-bottom: 3px solid #b74b4b;
	}

	@media (max-width: 995px) {
		nav {
			position: absolute;
			display: none;
			top: 0;
			right: 0;
			width: 40%;
			border-left: 3px solid #b74b4b;
			border-bottom: 3px solid #b74b4b;
			border-bottom-left-radius: 2rem;
			padding: 1rem solid;
			background-color: #161616;
			border-top: 0.1rem solid rgba(0, 0, 0, 0.1);
		}

		nav.active {
			display: block;
		}

		nav a {
			display: block;
			font-size: 15px;
			margin: 3rem 0;
		}

		nav a:hover,
		nav a.active {
			padding: 1rem;
			border-radius: 0.5rem;
			border-bottom: 0.5rem solid #b74b4b;
		}
    }
		
	
</style>

<div class="all">
    <div class="header">
        <p  class="logo"> <img src={Logo} height="60px" width="60" alt="" /> </p>
        
    
        <nav class="active">
            <a href="/">Inicio</a>
            <a href="#">Redes sociales</a>
            <a href="/InicioSesion">Inicia Sesion</a>
            <a href="#">Servicios</a>
        </nav>
    </div>
    
    <div class="container">
        <div class="card">
            <div class="image-container">
                <!-- Aquí va la imagen -->
            </div>
            <div class="card-content">
                <h1 class="card-title"><span>Libro 1 </span></h1>
                <p class="card-description">Esta es una breve descripción del libro 1.</p>
                <button class="btn">Leer más</button>
            </div>
        </div>
    
        <div class="card">
            <div class="image-container">
                <!-- Aquí va la imagen -->
            </div>
            <div class="card-content">
                <h1 class="card-title"><span>Libro 2</span></h1>
                <p class="card-description">Esta es una breve descripción del libro 2.</p>
                <button class="btn">Leer más</button>
            </div>
        </div>
    
        <div class="card">
            <div class="image-container">
                <!-- Aquí va la imagen -->
            </div>
            <div class="card-content">
                <h1 class="card-title"><span>Libro 3</span></h1>
                <p class="card-description">Esta es una breve descripción del libro 3.</p>
                <button class="btn">Leer más</button>
            </div>
        </div>
    
        <div class="card">
            <div class="image-container">
                <!-- Aquí va la imagen -->
            </div>
            <div class="card-content">
                <h1 class="card-title"><span>Libro 4</span></h1>
                <p class="card-description">Esta es una breve descripción del libro 4.</p>
                <button class="btn">Leer más</button>
            </div>
        </div>
    </div>
    
</div>
