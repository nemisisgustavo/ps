# ps<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Universo Gamer: Curiosidades e Mais!</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            background-color: #f8f8f8;
            color: #333;
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        header {
            background-color: #2c3e50;
            color: #fff;
            padding: 1em 0;
            text-align: center;
        }

        header .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        header h1 {
            margin: 0;
        }

        nav ul {
            list-style: none;
            padding: 0;
            margin: 0;
            display: flex;
        }

        nav li {
            margin-left: 20px;
        }

        nav a {
            color: #fff;
            text-decoration: none;
            transition: color 0.3s ease;
        }

        nav a:hover {
            color: #f39c12;
        }

        main {
            padding: 30px 0;
        }

        .conteudo-secao {
            background-color: #fff;
            padding: 30px;
            margin-bottom: 30px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }

        .conteudo-secao h2 {
            color: #3498db;
            margin-bottom: 20px;
            border-bottom: 2px solid #3498db;
            padding-bottom: 10px;
        }

        .card-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
        }

        .card {
            background-color: #ecf0f1;
            padding: 20px;
            border-radius: 5px;
            box-shadow: 0 1px 3px rgba(0, 0, 0, 0.05);
        }

        .card h3 {
            color: #e67e22;
            margin-top: 0;
            margin-bottom: 10px;
        }

        .saiba-mais {
            background-color: #3498db;
            color: #fff;
            border: none;
            padding: 10px 15px;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .saiba-mais:hover {
            background-color: #2980b9;
        }

        .detalhe-modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.5);
            justify-content: center;
            align-items: center;
        }

        .modal-conteudo {
            background-color: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            position: relative;
            width: 80%;
            max-width: 600px;
        }

        .fechar-modal {
            position: absolute;
            top: 10px;
            right: 15px;
            font-size: 20px;
            font-weight: bold;
            color: #333;
            cursor: pointer;
        }

        .form-group {
            margin-bottom: 15px;
        }

        .form-group label {
            display: block;
            margin-bottom: 5px;
            color: #555;
        }

        .form-group input[type="text"],
        .form-group input[type="email"],
        .form-group textarea {
            width: 100%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 4px;
            box-sizing: border-box;
        }

        .form-group textarea {
            resize: vertical;
        }

        form button[type="submit"] {
            background-color: #27ae60;
            color: #fff;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1em;
            transition: background-color 0.3s ease;
        }

        form button[type="submit"]:hover {
            background-color: #219653;
        }

        footer {
            background-color: #2c3e50;
            color: #fff;
            text-align: center;
            padding: 1em 0;
            position: relative;
            bottom: 0;
            width: 100%;
        }

        footer .container {
            padding: 15px;
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>Universo Gamer</h1>
            <nav>
                <ul>
                    <li><a href="#curiosidades">Curiosidades</a></li>
                    <li><a href="#historia">História dos Games</a></li>
                    <li><a href="#mundial">E-sports no Mundo</a></li>
                    <li><a href="#contato">Contato</a></li>
                </ul>
            </nav>
        </div>
    </header>
    <main class="container">
        <section id="curiosidades" class="conteudo-secao">
            <h2>Curiosidades Fascinantes do Mundo dos Games</h2>
            <div class="card-grid">
                <div class="card">
                    <h3>O Primeiro Videogame Comercial</h3>
                    <p>Descubra a história do "Computer Space", lançado em 1971, e como ele iniciou uma revolução.</p>
                    <button class="saiba-mais" data-curiosidade="primeiro-game">Saiba Mais</button>
                </div>
                <div class="card">
                    <h3>O Jogo Mais Vendido de Todos os Tempos</h3>
                    <p>Acredite se quiser, mas o Tetris reina absoluto em vendas! Veja os números impressionantes.</p>
                    <button class="saiba-mais" data-curiosidade="jogo-vendido">Saiba Mais</button>
                </div>
                <div class="card">
                    <h3>Um Controle de Piano para Atari?</h3>
                    <p>Conheça essa invenção bizarra que mostra como a criatividade (e talvez a loucura) moveu o mundo dos games.</p>
                    <button class="saiba-mais" data-curiosidade="controle-piano">Saiba Mais</button>
                </div>
                </div>
            <div id="detalhe-curiosidade" class="detalhe-modal">
                <div class="modal-conteudo">
                    <span class="fechar-modal">&times;</span>
                    <h4 id="titulo-detalhe"></h4>
                    <p id="texto-detalhe"></p>
                </div>
            </div>
        </section>

        <section id="historia" class="conteudo-secao">
            <h2>Uma Breve História da Evolução dos Games</h2>
            <p>Desde os primórdios com jogos arcade até a realidade virtual de hoje, a jornada dos games é épica!</p>
            <ul>
                <li><strong>Anos 70:</strong> O nascimento dos arcades e os primeiros consoles domésticos.</li>
                <li><strong>Anos 80:</strong> A era de ouro dos 8-bits e a explosão dos computadores pessoais nos jogos.</li>
                <li><strong>Anos 90:</strong> A revolução 16-bits e a chegada do 3D.</li>
                <li><strong>Anos 2000:</strong> A ascensão da internet nos jogos e a popularização dos consoles modernos.</li>
                <li><strong>Atualmente:</strong> Realidade virtual, jogos mobile e a força dos e-sports.</li>
            </ul>
        </section>

        <section id="mundial" class="conteudo-secao">
            <h2>O Fenômeno dos E-sports no Cenário Mundial</h2>
            <p>Descubra como os jogos eletrônicos se tornaram uma competição global com milhões de fãs e grandes premiações.</p>
            <p>De campeonatos de League of Legends a torneios de Counter-Strike, o cenário competitivo é vibrante e profissional.</p>
            </section>

        <section id="contato" class="conteudo-secao">
            <h2>Entre em Contato Conosco</h2>
            <p>Tem alguma curiosidade que gostaria de compartilhar? Alguma sugestão? Fale com a gente!</p>
            <form>
                <div class="form-group">
                    <label for="nome">Nome:</label>
                    <input type="text" id="nome" name="nome" required>
                </div>
                <div class="form-group">
                    <label for="email">Email:</label>
                    <input type="email" id="email" name="email" required>
                </div>
                <div class="form-group">
                    <label for="mensagem">Mensagem:</label>
                    <textarea id="mensagem" name="mensagem" rows="5" required></textarea>
                </div>
                <button type="submit">Enviar Mensagem</button>
            </form>
        </section>
    </main>
    <footer>
        <div class="container">
            <p>&copy; 2025 Universo Gamer - Compartilhando a Paixão por Games</p>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const botoesSaibaMais = document.querySelectorAll('.saiba-mais');
            const modalDetalhe = document.getElementById('detalhe-curiosidade');
            const tituloDetalhe = document.getElementById('titulo-detalhe');
            const textoDetalhe = document.getElementById('texto-detalhe');
            const botaoFecharModal = document.querySelector('.fechar-modal');

            const curiosidades = {
                'primeiro-game': {
                    titulo: 'Computer Space (1971)',
                    texto: 'Considerado o primeiro videogame comercial, "Computer Space" era uma adaptação do jogo de computador "Spacewar!". Funcionava com moedas e era encontrado em bares e fliperamas, marcando o início de uma indústria bilionária.'
                },
                'jogo-vendido': {
                    titulo: 'Tetris: Um Fenômeno Global',
                    texto: 'Com mais de 500 milhões de cópias vendidas em diversas plataformas, Tetris é um testemunho da simplicidade e do vício que um bom jogo pode causar. Criado na União Soviética, conquistou o mundo.'
                },
                'controle-piano': {
                    titulo: 'O Bizarro Controle de Piano do Atari',
                    texto: 'Para o jogo "Star Raiders" do Atari 2600, existia um controle especial que se assemelhava a um teclado de piano. Com diversas teclas e funcionalidades, era uma tentativa ambiciosa de oferecer mais complexidade de controle.'
                }
                // Adicione mais detalhes de curiosidades aqui usando o 'data-curiosidade' como chave
            };

            botoesSaibaMais.forEach(botao => {
                botao.addEventListener('click', function() {
                    const curiosidadeId = this.getAttribute('data-curiosidade');
                    if (curiosidades[curiosidadeId]) {
                        tituloDetalhe.textContent = curiosidades[curiosidadeId].titulo;
                        textoDetalhe.textContent = curiosidades[curiosidadeId].texto;
                        modalDetalhe.style.display = 'flex';
                    }
                });
            });

            botaoFecharModal.addEventListener('click', function() {
                modalDetalhe.style.display = 'none';
            });

            window.addEventListener('click', function(event) {
                if (event.target === modalDetalhe) {
                    modalDetalhe.style.display = 'none';
                }
            });
        });
    </script>
</body>
</html>
