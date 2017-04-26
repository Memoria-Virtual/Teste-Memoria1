# Teste-Memoria1
Galera, esse teste é apenas pra pegar pratica dentro da variavel phaser.game
<!doctype html> 
<html lang="en"> 
<head> 
	<meta charset="UTF-8" />
    
	<title>Teste do Phaser</title>
    \\Aqui a gente informa que vamos utilizar javascript e que a nossa biblioteca está no endereço citado como src
	<script type="text/javascript" src="js/phaser.min.js"></script>
    
    \\estilo utilizado apenas para crir uma margem por estetica e nada mais
    <style type="text/css">
        body {
            margin: 0;
        }
    </style>
</head>
<body>

<script type="text/javascript">

var game = new Phaser.Game(800, 600, Phaser.AUTO, '', { preload: preload, create: create, update: update });

function preload() {
    
    game.load.image('imgarrasta', 'assets/imgarrasta.png');
    game.load.image('quadro', 'assets/quadro2.png');
     game.load.image('donaanima', 'assets/donaanima.png');
    game.load.image('fundo', 'assets/fundo.png');
}

function create() {
    
    game.add.sprite(0, 0, 'fundo');
    game.add.sprite(280, 180, 'quadro');
    game.add.sprite(500, 400, 'imgarrasta');
    game.add.sprite(0, 0, 'donaanima');
    game.add.sprite(100, 400, 'imgarrasta');


}

function update() {
}

</script>

</body>
</html>
