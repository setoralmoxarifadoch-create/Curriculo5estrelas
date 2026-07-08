# Curriculo5estrelas 
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Currículo 5 Estrelas - Gerador de Currículos</title>
    <style>
        /* Paleta de Cores: Azul França (#318CE7) e Azul Marinho (#002147) */
        :root {
            --azul-franca: #318CE7;
            --azul-marinho: #002147;
            --cinza-claro: #f4f6f9;
            --branco: #ffffff;
            --texto: #333333;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--cinza-claro);
            color: var(--texto);
            line-height: 1.6;
        }

        /* Header & Logo Minimalista */
        header {
            background-color: var(--azul-marinho);
            color: var(--branco);
            padding: 20px;
            text-align: center;
            border-bottom: 5px solid var(--azul-franca);
        }

        .logo-container {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            margin-bottom: 5px;
        }

        .logo-icon {
            width: 40px;
            height: 40px;
            background-color: var(--azul-franca);
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            font-size: 24px;
            border-radius: 4px;
        }

        .logo-texto {
            font-size: 28px;
            font-weight: 800;
            letter-spacing: 1px;
            text-transform: uppercase;
        }

        header p {
            font-size: 14px;
            color: #b0c4de;
        }

        /* Container Principal */
        .container {
            max-width: 1000px;
            margin: 30px auto;
            padding: 0 20px;
        }

        /* Planos de Serviço */
        .planos-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            margin-bottom: 40px;
        }

        .plano-card {
            background: var(--branco);
            border: 2px solid #e0e0e0;
            border-radius: 8px;
            padding: 20px;
            text-align: center;
            transition: transform 0.3s;
        }

        .plano-card:hover {
            transform: translateY(-5px);
        }

        .plano-card.destaque {
            border-color: var(--azul-franca);
            box-shadow: 0 4px 15px rgba(49, 140, 231, 0.2);
        }

        .plano-titulo {
            font-size: 20px;
            color: var(--azul-marinho);
            margin-bottom: 10px;
        }

        .plano-preco {
            font-size: 24px;
            font-weight: bold;
            color: var(--azul-franca);
            margin-bottom: 15px;
        }

        /* Formulário */
        .form-section {
            background: var(--branco);
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.05);
            margin-bottom: 30px;
        }

        .form-section h2 {
            color: var(--azul-marinho);
            margin-bottom: 20px;
            border-bottom: 2px solid var(--azul-franca);
            padding-bottom: 5px;
        }

        .grid-inputs {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 15px;
        }

        @media (max-width: 768px) {
            .grid-inputs { grid-template-columns: 1fr; }
        }

        .input-group {
            margin-bottom: 15px;
            display: flex;
            flex-direction: column;
        }

        .input-group.full-width {
            grid-column: span 2;
        }

        @media (max-width: 768px) {
            .input-group.full-width { grid-column: span 1; }
        }

        label {
            font-weight: 600;
            margin-bottom: 5px;
            font-size: 14px;
        }

        input[type="text"], input[type="email"], input[type="tel"], select, textarea {
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
            font-size: 15px;
            width: 100%;
        }

        input:focus, textarea:focus, select:focus {
            outline: none;
            border-color: var(--azul-franca);
        }

        .btn-gerar {
            background-color: var(--azul-franca);
            color: var(--branco);
            border: none;
            padding: 15px 30px;
            font-size: 18px;
            font-weight: bold;
            border-radius: 4px;
            cursor: pointer;
            width: 100%;
            transition: background 0.2s;
        }

        .btn-gerar:hover {
            background-color: var(--azul-marinho);
        }

        /* Termos Legais e Rodapé */
        .termos-legais {
            font-size: 12px;
            color: #666;
            text-align: justify;
            margin-top: 30px;
            background: #eee;
            padding: 15px;
            border-radius: 4px;
        }

        footer {
            text-align: center;
            padding: 30px;
            font-size: 14px;
            color: #666;
        }
    </style>
</head>
<body>

    <header>
        <div class="logo-container">
            <div class="logo-icon">5★</div>
            <div class="logo-texto">Currículo 5 Estrelas</div>
        </div>
        <p>Seu objetivo profissional moldado para o sucesso</p>
    </header>

    <div class="container">

        <section class="planos-container">
            <div class="plano-card">
                <h3 class="plano-titulo">Plano Básico</h3>
                <div class="plano-preco">Grátis</div>
                <p>Currículo focado em 1 página + 1 Dica de Ouro com Frase Motivacional.</p>
            </div>
            <div class="plano-card destaque">
                <h3 class="plano-titulo">Plano Intermediário</h3>
                <div class="plano-preco">R$ 1,75</div>
                <p>Layout com cabeçalhos personalizados + 5 Dicas de Entrevista + Modelo de E-mail Atrativo.</p>
            </div>
            <div class="plano-card">
                <h3 class="plano-titulo">Plano Premium</h3>
                <div class="plano-preco">R$ 2,99</div>
                <p>Layout Exclusivo + 15 Dicas Avançadas + Guia de Vagas Indeed + Suporte Direto.</p>
            </div>
        </section>

        <form id="formCurriculo">
            
            <section class="form-section">
                <h2>1. Escolha o seu Plano de Emissão</h2>
                <div class="input-group">
                    <label for="plano">Selecione o plano desejado:</label>
                    <select id="plano" required>
                        <option value="gratis">Grátis (2 PDFs: Currículo + 1 Dica de Ouro)</option>
                        <option value="intermediario">Intermediário - R$ 1,75 (Layout Colorido + 5 Dicas + Modelo E-mail)</option>
                        <option value="premium">Premium - R$ 2,99 (Layout Top + 15 Dicas + Integração Indeed)</option>
                    </select>
                </div>
                <div class="grid-inputs">
                    <div class="input-group">
                        <label for="cpf">CPF (Necessário para emissão e validação dos planos pagos):</label>
                        <input type="text" id="cpf" placeholder="000.000.000-00">
                    </div>
                </div>
            </section>

            <section class="form-section">
                <h2>2. Dados Pessoais</h2>
                <div class="grid-inputs">
                    <div class="input-group full-width">
                        <label for="nome">Nome Completo:</label>
                        <input type="text" id="nome" required placeholder="Ex: João da Silva">
                    </div>
                    <div class="input-group">
                        <label for="email">E-mail:</label>
                        <input type="email" id="email" required placeholder="Ex: joao@email.com">
                    </div>
                    <div class="input-group">
                        <label for="WhatsApp">Celular / WhatsApp:</label>
                        <input type="tel" id="whatsapp" required placeholder="Ex: (24) 99999-9999">
                    </div>
                    <div class="input-group full-width">
                        <label for="endereco">Endereço Residencial:</label>
                        <input type="text" id="endereco" required placeholder="Rua, Número, Bairro, Cidade - Estado">
                    </div>
                    <div class="input-group">
                        <label for="escolaridade">Nível de Escolaridade:</label>
                        <select id="escolaridade" required>
                            <option value="Fundamental">Ensino Fundamental</option>
                            <option value="Medio">Ensino Médio</option>
                            <option value="Tecnico">Ensino Técnico</option>
                            <option value="Superior">Ensino Superior</option>
                        </select>
                    </div>
                    <div class="input-group">
                        <label for="foto">Deseja incluir foto no currículo?</label>
                        <select id="foto">
                            <option value="nao">Não</option>
                            <option value="sim">Sim (Inserir no próximo passo)</option>
                        </select>
                    </div>
                </div>
            </section>

            <section class="form-section">
                <h2>3. Foco Profissional Único</h2>
                <p style="font-size: 13px; color: #666; margin-bottom: 15px;">
                    *Atenção: Para aumentar suas chances, preencha as experiências e cursos voltados <strong>apenas</strong> para o cargo desejado.
                </p>
                <div class="input-group">
                    <label for="objetivo">Cargo Pretendido (Ex: Almoxerife):</label>
                    <input type="text" id="objetivo" required placeholder="Digite estritamente o cargo que deseja concorrer">
                </div>
                <div class="input-group">
                    <label for="experiencia">Experiências Profissionais voltadas a este cargo:</label>
                    <textarea id="experiencia" rows="4" placeholder="Descreva suas experiências anteriores relacionadas a esta vaga..." required></textarea>
                </div>
                <div class="input-group">
                    <label for="formacao">Cursos e Especializações voltadas a este cargo:</label>
                    <textarea id="formacao" rows="4" placeholder="Ex: Curso de Logística, Almoxarifado Prático, etc..." required></textarea>
                </div>
            </section>

            <button type="submit" class="btn-gerar">Avançar para Gerar Currículo 5 Estrelas</button>
        </form>

        <div class="termos-legais">
            <strong>Informações Legais e Termos de Uso:</strong><br>
            Nos termos do Artigo 49 do Código de Defesa do Consumidor (Lei nº 8.078/90), o direito de arrependimento de 7 dias é aplicado a produtos e serviços digitais. Contudo, por se tratar de um produto digital personalizado e de entrega e consumo imediatos (geração automatizada de documento exclusivo com base nos dados fornecidos pelo usuário), após a efetiva prestação do serviço e download do material, o direito de desistência e reembolso não poderá ser exercido, visto que o produto já foi integralmente usufruído e entregue conforme as especificações solicitadas. Ao prosseguir, você concorda com estes termos.
        </div>

    </div>

    <footer>
        <p>Chave Pix para Apoio ao Projeto: <strong>24992524024</strong></p>
        <p>© 2026 Currículo 5 Estrelas. Positividade e muita sorte na sua jornada profissional!</p>
    </footer>

</body>
</html>
