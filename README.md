# ENYO-TECH
Site oficial da ENYO TECH para venda de pacotes de internet da Vodacom Moçambique.

<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ENYO TECH - Vendas de Megas Vodacom</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f5f5f5;
            color: #333;
        }
        
        header {
            background-color: #e60000;
            color: white;
            padding: 1.5rem;
            text-align: center;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }
        
        h1 {
            font-size: 2.2rem;
            margin-bottom: 0.5rem;
        }
        
        .container {
            max-width: 900px;
            margin: 2rem auto;
            padding: 0 1rem;
        }
        
        .intro {
            text-align: center;
            margin-bottom: 2rem;
            padding: 1rem;
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
        }
        
        .intro p {
            font-size: 1.1rem;
            line-height: 1.6;
        }
        
        .tabs {
            display: flex;
            margin-bottom: 1.5rem;
            gap: 1rem;
            justify-content: center;
        }
        
        .tab-btn {
            padding: 0.8rem 1.5rem;
            font-size: 1rem;
            font-weight: 600;
            background-color: #f1f1f1;
            border: none;
            border-radius: 6px;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        
        .tab-btn.active {
            background-color: #e60000;
            color: white;
        }
        
        .tab-content {
            display: none;
        }
        
        .tab-content.active {
            display: block;
            animation: fadeIn 0.5s;
        }
        
        @keyframes fadeIn {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }
        
        .pacotes {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1.5rem;
            margin-bottom: 2rem;
        }
        
        .pacote {
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
        }
        
        .pacote:hover {
            transform: translateY(-5px);
        }
        
        .pacote-header {
            background-color: #e60000;
            color: white;
            padding: 1rem;
            text-align: center;
        }
        
        .pacote-body {
            padding: 1.5rem;
            text-align: center;
        }
        
        .pacote-preco {
            font-size: 1.8rem;
            font-weight: bold;
            margin: 1rem 0;
            color: #e60000;
        }
        
        .btn {
            display: inline-block;
            background-color: #25d366;
            color: white;
            padding: 0.8rem 1.5rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
            font-size: 1rem;
            width: 100%;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }
        
        .btn:hover {
            background-color: #128c7e;
            transform: scale(1.05);
        }
        
        .whatsapp-icon {
            margin-right: 5px;
        }
        
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 1.5rem;
            margin-top: 2rem;
        }
        
        @media (max-width: 768px) {
            .pacotes {
                grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
            }
            
            h1 {
                font-size: 1.8rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>ENYO TECH</h1>
        <p>Pacotes de Internet Vodacom</p>
    </header>
    
    <div class="container">
        <div class="intro">
            <p>Compre seus pacotes de internet da Vodacom com os melhores preços! <br>Basta escolher o pacote desejado e finalizar sua compra via WhatsApp.</p>
        </div>
        
        <div class="tabs">
            <button class="tab-btn active" onclick="openTab('diarios')">Pacotes Diários</button>
            <button class="tab-btn" onclick="openTab('mensais')">Pacotes Mensais</button>
        </div>
        
        <div id="diarios" class="tab-content active">
            <div class="pacotes">
                <div class="pacote">
                    <div class="pacote-header">
                        <h3>1 GB</h3>
                        <p>(1024 MB)</p>
                    </div>
                    <div class="pacote-body">
                        <p>Válido por 24 horas</p>
                        <div class="pacote-preco">20 MT</div>
                        <button class="btn" onclick="comprarPacote('Pacote Diário - 1GB (1024 MB) - 20 MT')">
                            <i class="whatsapp-icon">💬</i> Comprar
                        </button>
                    </div>
                </div>
                
                <div class="pacote">
                    <div class="pacote-header">
                        <h3>2 GB</h3>
                        <p>(2048 MB)</p>
                    </div>
                    <div class="pacote-body">
                        <p>Válido por 24 horas</p>
                        <div class="pacote-preco">40 MT</div>
                        <button class="btn" onclick="comprarPacote('Pacote Diário - 2GB (2048 MB) - 40 MT')">
                            <i class="whatsapp-icon">💬</i> Comprar
                        </button>
                    </div>
                </div>
                
                <div class="pacote">
                    <div class="pacote-header">
                        <h3>5 GB</h3>
                        <p>(5120 MB)</p>
                    </div>
                    <div class="pacote-body">
                        <p>Válido por 24 horas</p>
                        <div class="pacote-preco">100 MT</div>
                        <button class="btn" onclick="comprarPacote('Pacote Diário - 5GB (5120 MB) - 100 MT')">
                            <i class="whatsapp-icon">💬</i> Comprar
                        </button>
                    </div>
                </div>
                
                <div class="pacote">
                    <div class="pacote-header">
                        <h3>10 GB</h3>
                        <p>(10240 MB)</p>
                    </div>
                    <div class="pacote-body">
                        <p>Válido por 24 horas</p>
                        <div class="pacote-preco">180 MT</div>
                        <button class="btn" onclick="comprarPacote('Pacote Diário - 10GB (10240 MB) - 180 MT')">
                            <i class="whatsapp-icon">💬</i> Comprar
                        </button>
                    </div>
                </div>
            </div>
        </div>
        
        <div id="mensais" class="tab-content">
            <div class="pacotes">
                <div class="pacote">
                    <div class="pacote-header">
                        <h3>5 GB</h3>
                        <p>(5120 MB)</p>
                    </div>
                    <div class="pacote-body">
                        <p>Válido por 30 dias</p>
                        <div class="pacote-preco">170 MT</div>
                        <button class="btn" onclick="comprarPacote('Pacote Mensal - 5GB (5120 MB) - 170 MT')">
                            <i class="whatsapp-icon">💬</i> Comprar
                        </button>
                    </div>
                </div>
                
                <div class="pacote">
                    <div class="pacote-header">
                        <h3>12 GB</h3>
                        <p>(12288 MB)</p>
                    </div>
                    <div class="pacote-body">
                        <p>Válido por 30 dias</p>
                        <div class="pacote-preco">350 MT</div>
                        <button class="btn" onclick="comprarPacote('Pacote Mensal - 12GB (12288 MB) - 350 MT')">
                            <i class="whatsapp-icon">💬</i> Comprar
                        </button>
                    </div>
                </div>
                
                <div class="pacote">
                    <div class="pacote-header">
                        <h3>20 GB</h3>
                        <p>(20480 MB)</p>
                    </div>
                    <div class="pacote-body">
                        <p>Válido por 30 dias</p>
                        <div class="pacote-preco">500 MT</div>
                        <button class="btn" onclick="comprarPacote('Pacote Mensal - 20GB (20480 MB) - 500 MT')">
                            <i class="whatsapp-icon">💬</i> Comprar
                        </button>
                    </div>
                </div>
                
                <div class="pacote">
                    <div class="pacote-header">
                        <h3>51 GB</h3>
                        <p>(51200 MB)</p>
                    </div>
                    <div class="pacote-body">
                        <p>Válido por 30 dias</p>
                        <div class="pacote-preco">1100 MT</div>
                        <button class="btn" onclick="comprarPacote('Pacote Mensal - 51GB (51200 MB) - 1100 MT')">
                            <i class="whatsapp-icon">💬</i> Comprar
                        </button>
                    </div>
                </div>
                
                <div class="pacote">
                    <div class="pacote-header">
                        <h3>102 GB</h3>
                        <p>(102448 MB)</p>
                    </div>
                    <div class="pacote-body">
                        <p>Válido por 30 dias</p>
                        <div class="pacote-preco">2100 MT</div>
                        <button class="btn" onclick="comprarPacote('Pacote Mensal - 102GB (102448 MB) - 2100 MT')">
                            <i class="whatsapp-icon">💬</i> Comprar
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </div>
    
    <footer>
        <p>&copy; 2025 ENYO TECH - Todos os direitos reservados</p>
    </footer>
    
    <script>
        function openTab(tabName) {
            // Esconder todos os conteúdos de tab
            const tabContents = document.getElementsByClassName("tab-content");
            for (let i = 0; i < tabContents.length; i++) {
                tabContents[i].classList.remove("active");
            }
            
            // Remover a classe active de todos os botões
            const tabButtons = document.getElementsByClassName("tab-btn");
            for (let i = 0; i < tabButtons.length; i++) {
                tabButtons[i].classList.remove("active");
            }
            
            // Mostrar o conteúdo do tab selecionado
            document.getElementById(tabName).classList.add("active");
            
            // Destacar o botão clicado
            event.currentTarget.classList.add("active");
        }
        
        function comprarPacote(pacote) {
            const mensagem = `Olá! Gostaria de comprar: ${pacote}`;
            const numeroWhatsApp = "258849267984";
            const url = `https://wa.me/${numeroWhatsApp}?text=${encodeURIComponent(mensagem)}`;
            window.open(url, '_blank');
        }
    </script>
</body>
</html>
