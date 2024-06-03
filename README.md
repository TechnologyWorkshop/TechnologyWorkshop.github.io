<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Technology Workshop - Helm</title>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap">
    <style>
        body {
            background-color: #0b3a53;
            color: #ffffff;
            font-family: 'Montserrat', sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
        }
        header {
            width: 100%;
            padding: 20px 0;
            display: flex;
            justify-content: center;
            align-items: center;
			margin-bottom: 20px;
        }
        header img {
            height: 150px;
        }
        main {
            background-color: #ffffff;
            border-radius: 8px;
            padding: 20px;
            max-width: 800px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            margin-top: -30px;
            color: #333;
        }
        h1 {
            color: #0b3a53;
            font-size: 2.5em;
        }
        p {
            font-size: 1.2em;
            line-height: 1.6;
            margin: 20px 0;
        }
		
		.boat {
			width: 100vw;
			position: absolute;
			top: auto;
			bottom: 8px;
			left: 0;
			right: 0;
			min-height: 10vw;
			z-index: 1070;
		}
		
		.boat .boat-ship {
			position: absolute;
			margin-top: 0.5vw;
			left: 3.25vw;
			bottom: 2vw;
			max-width: 15vw;
			z-index: 1060;
			-webkit-animation: boat-bob 7s ease-in-out infinite;
			animation: boat-bob 7s ease-in-out infinite;
			transition: all .3s ease-in-out;
		}
		
		.boat .wave-wrapper {
		position: absolute;
		margin: 0;
		left: 0;
		right: 15px;
		bottom: -8px;
		height: 15vw;
		overflow: hidden;
		z-index: 1014;
		background-color: transparent;
		transition: all .3s ease-in-out;
	}
	
		.boat .wave-wrapper .waves {
		position: relative;
		width: 100%;
		height: 3vw;
		margin-top: 9.5vw;
		margin-bottom: -7px;
		min-height: 0.5vw;
		max-height: 2vw;
		transition: all .3s ease-in-out;
	}
	
	.boat:after {
    content: "ahoy!";
    font-family: "Space Mono", "Courier New", monaco, monospace;
    font-size: .75rem;
    padding: 0.75em;
    color: #091C84;
    background: #F8DCDF;
    position: absolute;
    bottom: 8vw;
    left: 13.5vw;
    line-height: 1;
    z-index: 1005;
    opacity: 0;
    transition: all .3s ease-in-out;
}

.boat .wave-wrapper:before {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    content: " ";
    height: 3.5vw;
    width: 100%;
    background: #1B53C2;
    transition: all .3s ease-in-out;
}

*, *::before, *::after {
    box-sizing: inherit;
}

svg[Kenmerkstijl] {
    shape-rendering: auto;
}
    </style>
</head>
<body style="background-image: url('https://helm.sh/img/topography.png'); font-family: Public Sans, Helvetica, Arial, sans-serif;; color:#090E6F;">
    <header>
        <img src="https://helm.sh/img/helm.svg" alt="Helm Logo">
    </header>
    <main>
        <h1>Helm</h1>
        <p>Helm is een pakketmanager voor Kubernetes, een open-source platform voor het automatiseren van de deployment, scaling en management van containerized applicaties. Helm helpt je bij het beheren van Kubernetes-applicaties door het organiseren van alle benodigde Kubernetes-manifestbestanden in een enkel pakket, genaamd een chart.</p>
        <p>Met Helm kun je gemakkelijk applicaties installeren, upgraden en beheren binnen je Kubernetes-cluster. Het vereenvoudigt de complexiteit van het handmatig beheren van Kubernetes-resources en biedt herhaalbare applicatie-installaties, versiebeheer en rollback mogelijkheden.</p>
        <p>Helm charts zijn herbruikbare pakketten van geconfigureerde Kubernetes-resources. Deze charts kunnen worden gedeeld en gebruikt om snel nieuwe applicaties te deployen in je Kubernetes-omgeving.</p>
    </main>
	
	<div class="boat boat-full"><img src="https://helm.sh/img/boat.svg" alt="boat" class="boat-ship"><div class="wave-wrapper"><svg class="waves" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 24 150 28" preserveAspectRatio="none" shape-rendering="auto"><defs><path id="gentle-wave" d="M-160 44c30 0 58-18 88-18s58 18 88 18 58-18 88-18 58 18 88 18v44h-352z"></path></defs><g class="parallax"><use xlink:href="#gentle-wave" x="48" y="0" fill="rgba(27,83,194,0.7"></use><use xlink:href="#gentle-wave" x="48" y="3" fill="rgba(27,83,194,0.5)"></use><use xlink:href="#gentle-wave" x="48" y="5" fill="rgba(27,83,194,0.3)"></use><use xlink:href="#gentle-wave" x="48" y="7" fill="rgba(27,83,194,1)"></use></g></svg></div></div>
	
</body>
</html>
