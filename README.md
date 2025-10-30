<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Menu de Procedimentos - KG Beauty</title>
    
    <!-- Tailwind CSS para estilização rápida e responsiva --><script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Google Fonts para uma tipografia mais elegante --><link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;600;700&family=Lato:wght@300;400;700&display=swap" rel="stylesheet">
    
    <!-- Feather Icons for close button --><script src="https://unpkg.com/feather-icons"></script>
    
    <style>
        /* Estilos personalizados que complementam o Tailwind CSS */
        body {
            /* Cor de fundo suave da sua identidade visual */
            background-color: #FBF9F4;
        }
        .font-heading {
            font-family: 'Cormorant Garamond', serif;
        }
        .font-body {
            font-family: 'Lato', sans-serif;
        }
        /* Simulação da estrutura de um app de celular */
        .mobile-app-container {
            max-width: 450px;
            margin: auto;
            min-height: 100vh;
            /* Fundo branco sólido */
            background-color: #FFFFFF;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
        }
        /* Cor de destaque dourada, inspirada na marca */
        .text-brand-gold {
            color: #B9975B;
        }
        .bg-brand-gold {
            background-color: #B9975B;
        }
        .border-brand-light {
           border-color: #F0EAE0;
        }
        /* Animação do Spinner */
        .spinner {
            border: 4px solid rgba(0, 0, 0, 0.1);
            width: 36px;
            height: 36px;
            border-radius: 50%;
            border-left-color: #B9975B;
            animation: spin 1s ease infinite;
        }
        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
        /* Estilo para o resultado do Gemini para preservar a formatação */
        .gemini-response {
            white-space: pre-wrap;
            line-height: 1.6;
        }
        /* Estilo para o banner da logo */
        .logo-banner {
            width: 100%;
            height: 180px; /* Altura fixa para o banner */
            object-fit: cover; /* Garante que a imagem cubra a área sem distorcer, cortando se necessário */
            object-position: center; /* Centraliza a imagem no banner */
            display: block;
            background-color: #FBF9F4;
        }
    </style>
</head>
<body class="font-body">

    <div class="mobile-app-container">
        <!-- Cabeçalho com o nome da marca -->
        <header class="text-center">
            <!-- Usando imagens otimizadas (se tiver) -->
            <picture>
                <source type="image/webp" srcset="assets/kg-beauty-banner.webp 1x, assets/kg-beauty-banner@2x.webp 2x">
                <img src="assets/kg-beauty-banner.jpg" srcset="assets/kg-beauty-banner@2x.jpg 2x" alt="KG Beauty" class="logo-banner" width="450" height="180">
            </picture>
        </header>

        <!-- Conteúdo principal com o menu de procedimentos --><main id="menu-container" class="px-6 pb-28">

            <!-- Seção de Cílios --><section id="cilios" class="mb-10">
                <h1 class="font-heading text-4xl text-brand-gold font-semibold border-b-2 border-brand-light pb-3 mb-6">Cílios</h1>
                <div class="procedure-item">
                    <div class="flex justify-between items-start mb-1">
                        <div class="flex items-center gap-2">
                            <h2 class="text-xl font-semibold text-gray-800">LASH LIFTING</h2>
                            <button class="generate-explanation-btn text-brand-gold hover:text-yellow-700" data-procedure="LASH LIFTING" title="O que é isso?">
                                <i data-feather="help-circle" class="w-4 h-4"></i>
                            </button>
                        </div>
                        <p class="text-xl font-bold text-brand-gold whitespace-nowrap ml-4">R$130</p>
                    </div>
                    <p class="text-gray-600 text-sm leading-relaxed mb-2">
                        Técnica que nutre, curva, e colore os cílios naturais, embelezando seu olhar e proporcionando a sensação de fios alongados. Substitui o uso diário do curvex e máscara, mantendo o olhar aberto e marcante de forma natural. Durabilidade de até 60 dias.
                    </p>
                    <button class="generate-aftercare-btn text-xs text-brand-gold font-semibold py-1 px-2 rounded-md border border-brand-gold hover:bg-brand-gold hover:text-white transition-colors" data-procedure="LASH LIFTING">✨ Dicas de Cuidado</button>
                </div>
            </section>

            <!-- Seção de Sobrancelhas --><section id="sobrancelhas" class="mb-10">
                <h1 class="font-heading text-4xl text-brand-gold font-semibold border-b-2 border-brand-light pb-3 mb-6">Sobrancelhas</h1>
                
                <div class="space-y-6">
                    <div class="procedure-item">
                        <div class="flex justify-between items-start mb-1">
                            <div class="flex items-center gap-2">
                                <h2 class="text-xl font-semibold text-gray-800">BROW LAMINATION</h2>
                                <button class="generate-explanation-btn text-brand-gold hover:text-yellow-700" data-procedure="BROW LAMINATION" title="O que é isso?">
                                    <i data-feather="help-circle" class="w-4 h-4"></i>
                                </button>
                            </div>
                            <p class="text-xl font-bold text-brand-gold whitespace-nowrap ml-4">R$130</p>
                        </div>
                        <p class="text-gray-600 text-sm leading-relaxed mb-2">
                            Técnica moderna que alinha e modela os fios, proporcionando um efeito de sobrancelhas mais cheias e definidas. Durabilidade de até 60 dias.
                        </p>
                        <button class="generate-aftercare-btn text-xs text-brand-gold font-semibold py-1 px-2 rounded-md border border-brand-gold hover:bg-brand-gold hover:text-white transition-colors" data-procedure="BROW LAMINATION">✨ Dicas de Cuidado</button>
                    </div>
                    
                    <!-- Novos itens inseridos abaixo de Brow Lamination e acima do Buço -->
                    <div class="procedure-item">
                        <div class="flex justify-between items-start mb-1">
                            <div class="flex items-center gap-2">
                                <h2 class="text-xl font-semibold text-gray-800">DESIGN DE SOBRANCELHAS</h2>
                                <button class="generate-explanation-btn text-brand-gold hover:text-yellow-700" data-procedure="DESIGN DE SOBRANCELHAS" title="O que é isso?">
                                    <i data-feather="help-circle" class="w-4 h-4"></i>
                                </button>
                            </div>
                            <p class="text-xl font-bold text-brand-gold whitespace-nowrap ml-4">R$35</p>
                        </div>
                        <p class="text-gray-600 text-sm leading-relaxed mb-2">
                            Projeto personalizado com as medidas do seu rosto, mantendo a naturalidade, valorizando seu olhar de forma harmônica e elegante sem afinar.
                        </p>
                        <button class="generate-aftercare-btn text-xs text-brand-gold font-semibold py-1 px-2 rounded-md border border-brand-gold hover:bg-brand-gold hover:text-white transition-colors" data-procedure="DESIGN DE SOBRANCELHAS">✨ Dicas de Cuidado</button>
                    </div>

                    <div class="procedure-item">
                        <div class="flex justify-between items-start mb-1">
                            <div class="flex items-center gap-2">
                                <h2 class="text-xl font-semibold text-gray-800">DESIGN COM TINTURA</h2>
                                <button class="generate-explanation-btn text-brand-gold hover:text-yellow-700" data-procedure="DESIGN COM TINTURA" title="O que é isso?">
                                    <i data-feather="help-circle" class="w-4 h-4"></i>
                                </button>
                            </div>
                            <p class="text-xl font-bold text-brand-gold whitespace-nowrap ml-4">R$50</p>
                        </div>
                        <p class="text-gray-600 text-sm leading-relaxed mb-2">
                            Ideal para cobertura de fios grisalhos, loiros e mesmo os escuros. Com uma tintura específica para a região, intensifica a cor natural e adiciona mais brilho e volume. Durabilidade de 20 a 30 dias.
                        </p>
                        <button class="generate-aftercare-btn text-xs text-brand-gold font-semibold py-1 px-2 rounded-md border border-brand-gold hover:bg-brand-gold hover:text-white transition-colors" data-procedure="DESIGN COM TINTURA">✨ Dicas de Cuidado</button>
                    </div>

                    <div class="procedure-item">
                        <div class="flex justify-between items-start mb-1">
                            <div class="flex items-center gap-2">
                                <h2 class="text-xl font-semibold text-gray-800">DESIGN COM HENNA</h2>
                                <button class="generate-explanation-btn text-brand-gold hover:text-yellow-700" data-procedure="DESIGN COM HENNA" title="O que é isso?">
                                    <i data-feather="help-circle" class="w-4 h-4"></i>
                                </button>
                            </div>
                            <p class="text-xl font-bold text-brand-gold whitespace-nowrap ml-4">R$45</p>
                        </div>
                        <p class="text-gray-600 text-sm leading-relaxed">
                            Ideal para quem possui falhas, a henna pigmenta além dos pelos, a pele, proporcionando um efeito de sombra nas sobrancelhas de intensidade personalizável. Durabilidade de 3 a 10 dias.
                        </p>
                        <button class="generate-aftercare-btn text-xs text-brand-gold font-semibold py-1 px-2 rounded-md border border-brand-gold hover:bg-brand-gold hover:text-white transition-colors" data-procedure="DESIGN COM HENNA">✨ Dicas de Cuidado</button>
                    </div>
                    
                    <div class="procedure-item">
                        <div class="flex justify-between items-start mb-1">
                            <h2 class="text-xl font-semibold text-gray-800">BUÇO (FIO EGÍPCIO)</h2>
                            <p class="text-xl font-bold text-brand-gold whitespace-nowrap ml-4">R$15</p>
                        </div>
                        <p class="text-gray-600 text-sm leading-relaxed">
                             Técnica que remove os pelos da região do buço sem agredir a pele, utilizando linhas de algodão. Minimiza irritações, proporciona acabamento limpo e duradouro, ideal para peles sensíveis.
                        </p>
                    </div>
                </div>
            </section>
            
            <!-- Seção de Combos --><section id="combos">
                <h1 class="font-heading text-4xl text-brand-gold font-semibold border-b-2 border-brand-light pb-3 mb-6">Combos</h1>
                
                 <div class="space-y-6">
                    <div class="procedure-item">
                        <div class="flex justify-between items-start mb-1">
                            <h2 class="text-xl font-semibold text-gray-800">LASH LIFTING + BROW LAMINATION</h2>
                            <p class="text-xl font-bold text-brand-gold whitespace-nowrap ml-4">R$240</p>
                        </div>
                    </div>

                    <div class="procedure-item">
                        <div class="flex justify-between items-start mb-1">
                            <h2 class="text-xl font-semibold text-gray-800 leading-tight max-w-xs">DESIGN + BROW LAMINATION + LASH LIFTING + BUÇO</h2>
                            <p class="text-xl font-bold text-brand-gold whitespace-nowrap ml-4">R$290</p>
                        </div>
                    </div>

                    <div class="procedure-item">
                        <div class="flex justify-between items-start mb-1">
                            <h2 class="text-xl font-semibold text-gray-800">DESIGN COM TINTURA + BUÇO</h2>
                            <p class="text-xl font-bold text-brand-gold whitespace-nowrap ml-4">R$55</p>
                        </div>
                    </div>
                 </div>
            </section>

        </main>
    </div>

    <!-- Botão Flutuante (FAB) para o Assistente de Beleza --><button id="aiAdvisorButton" class="fixed bottom-6 right-6 bg-brand-gold text-white font-bold py-3 px-5 rounded-full shadow-lg hover:bg-yellow-700 transition-transform transform hover:scale-105 flex items-center gap-2">
        <span class="text-lg">✨</span>
        <span>Me Ajude a Escolher</span>
    </button>

    <!-- Botão Flutuante para WhatsApp (canto inferior esquerdo) -->
    <!-- Substitua o número de exemplo (5511991234567) pelo seu número em formato internacional sem "+" ou zeros iniciais -->
    <a id="whatsappLink"
       href="https://wa.me/5511991234567?text=Ol%C3%A1%2C%20gostaria%20de%20agendar%20um%20procedimento%20na%20KG%20Beauty."
       target="_blank"
       rel="noopener noreferrer"
       aria-label="Contato via WhatsApp"
       class="fixed bottom-6 left-6 bg-green-600 text-white font-bold py-3 px-4 rounded-full shadow-lg hover:bg-green-700 transition-transform transform hover:scale-105 flex items-center gap-2">
        <!-- Ícone simples do WhatsApp (SVG) -->
        <svg width="20" height="20" viewBox="0 0 24 24" fill="none" aria-hidden="true" xmlns="http://www.w3.org/2000/svg">
            <path d="M20.52 3.48A11.88 11.88 0 0012 .5C6.21.5 1.7 4.99 1.7 10.79c0 1.89.5 3.66 1.45 5.24L.5 23.5l7.8-2.03a11.84 11.84 0 005.7 1.44c5.79 0 10.3-4.49 10.3-10.29 0-2.75-1.07-5.33-3.28-7.14z" fill="currentColor"/>
            <path d="M17.28 14.34c-.33-.16-1.95-.97-2.25-1.08-.3-.11-.52-.16-.74.16s-.85 1.08-1.05 1.3c-.19.22-.39.25-.72.08-.33-.16-1.4-.52-2.67-1.64-.99-.88-1.66-1.97-1.85-2.29-.19-.33-.02-.51.14-.67.14-.14.33-.36.5-.55.16-.19.22-.33.33-.55.11-.22.05-.41-.03-.57-.08-.16-.74-1.78-1.01-2.44-.27-.64-.55-.55-.74-.56l-.63-.01c-.2 0-.52.08-.79.37-.27.29-1.04 1.01-1.04 2.46 0 1.45 1.06 2.85 1.21 3.05.14.19 2.09 3.2 5.06 4.49 3.02 1.31 3.02.87 3.57.82.55-.05 1.95-.79 2.23-1.55.27-.77.27-1.43.19-1.57-.08-.15-.29-.25-.62-.41z" fill="#ffffff"/>
        </svg>
        <span>Agendar (WhatsApp)</span>
    </a>

    <!-- Modal do Assistente de Beleza --><div id="aiAdvisorModal" class="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center p-4 hidden z-50">
        <div class="bg-white rounded-lg shadow-2xl w-full max-w-md m-auto relative flex flex-col max-h-[90vh]">
            <button class="absolute top-3 right-3 text-gray-400 hover:text-gray-700" id="closeAdvisorModal">
                <i data-feather="x"></i>
            </button>
            <h2 class="font-heading text-2xl text-brand-gold p-6 pb-4">✨ Assistente de Beleza AI</h2>
            <!-- Wrapper rolável --><div class="flex-1 overflow-y-auto p-6 pt-0">
                <p class="text-gray-600 mb-4 text-sm">Descreva o visual que você deseja ou suas dúvidas e nossa IA irá sugerir os melhores procedimentos para você!</p>
                <textarea id="userInput" class="w-full h-24 border border-gray-300 rounded-md p-2 text-sm focus:ring-2 focus:ring-brand-gold focus:border-transparent transition" placeholder="Ex: 'Quero um olhar mais marcante, mas sem parecer artificial.' ou 'Minhas sobrancelhas são falhadas, o que posso fazer?'"></textarea>
                <button id="getRecommendationBtn" class="w-full bg-brand-gold text-white font-bold py-2 px-4 rounded-md mt-4 hover:bg-yellow-700 transition-colors">
                    Obter Recomendação
                </button>
                <div id="advisorResult" class="mt-4">
                    <!-- O resultado da IA aparecerá aqui --></div>
            </div>
        </div>
    </div>
    
    <!-- Modal para Dicas de Cuidado --><div id="aftercareModal" class="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center p-4 hidden z-50">
        <div class="bg-white rounded-lg shadow-2xl w-full max-w-md m-auto relative flex flex-col max-h-[90vh]">
             <button class="absolute top-3 right-3 text-gray-400 hover:text-gray-700" id="closeAftercareModal">
                <i data-feather="x"></i>
            </button>
            <h2 id="aftercareTitle" class="font-heading text-2xl text-brand-gold p-6 pb-4">✨ Dicas de Cuidado</h2>
            <!-- Wrapper rolável --><div class="flex-1 overflow-y-auto p-6 pt-0">
                <div id="aftercareResult" class="text-gray-700 text-sm">
                     <!-- O resultado da IA aparecerá aqui --></div>
            </div>
        </div>
    </div>
    
    <!-- Modal para Explicação de Termo --><div id="explanationModal" class="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center p-4 hidden z-50">
        <div class="bg-white rounded-lg shadow-2xl w-full max-w-md m-auto relative flex flex-col max-h-[90vh]">
             <button class="absolute top-3 right-3 text-gray-400 hover:text-gray-700" id="closeExplanationModal">
                <i data-feather="x-circle"></i>
            </button>
            <h2 id="explanationTitle" class="font-heading text-2xl text-brand-gold p-6 pb-4">✨ O que é?</h2>
            <!-- Wrapper rolável --><div class="flex-1 overflow-y-auto p-6 pt-0">
                <div id="explanationResult" class="text-gray-700 text-sm">
                     <!-- O resultado da IA aparecerá aqui --></div>
            </div>
        </div>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            feather.replace(); // Inicia os ícones

            // Elementos dos Modais
            const aiAdvisorButton = document.getElementById('aiAdvisorButton');
            const aiAdvisorModal = document.getElementById('aiAdvisorModal');
            const closeAdvisorModal = document.getElementById('closeAdvisorModal');
            const getRecommendationBtn = document.getElementById('getRecommendationBtn');
            const advisorResult = document.getElementById('advisorResult');
            const userInput = document.getElementById('userInput');
            
            const aftercareModal = document.getElementById('aftercareModal');
            const closeAftercareModal = document.getElementById('closeAftercareModal');
            const aftercareResult = document.getElementById('aftercareResult');
            const aftercareTitle = document.getElementById('aftercareTitle');

            // Elementos do novo Modal de Explicação
            const explanationModal = document.getElementById('explanationModal');
            const closeExplanationModal = document.getElementById('closeExplanationModal');
            const explanationResult = document.getElementById('explanationResult');
            const explanationTitle = document.getElementById('explanationTitle');

            // --- Lógica do Assistente de Beleza ---

            // Abre o modal do assistente
            aiAdvisorButton.addEventListener('click', () => {
                aiAdvisorModal.classList.remove('hidden');
            });

            // Fecha o modal do assistente
            closeAdvisorModal.addEventListener('click', () => {
                aiAdvisorModal.classList.add('hidden');
            });

            // Lida com o clique para obter recomendação
            getRecommendationBtn.addEventListener('click', async () => {
                const userQuery = userInput.value;
                if (!userQuery.trim()) {
                    advisorResult.innerHTML = `<p class="text-red-500 text-sm">Por favor, descreva o que você deseja.</p>`;
                    return;
                }

                advisorResult.innerHTML = '<div class="flex justify-center items-center p-4"><div class="spinner"></div></div>';
                
                const menuText = getMenuAsText();
                const systemPrompt = "Você é uma especialista em beleza e consultora da KG Beauty. Seu tone é amigável, profissional e encorajador. Analise o desejo da cliente e, com base no menu de procedimentos da KG Beauty fornecido, sugira os melhores serviços ou combos. Explique o porquê da sua recomendação de forma clara. Sempre liste os procedimentos sugeridos e seus preços. Formate sua resposta de forma legível. Não use Markdown.";
                const userPrompt = `--- MENU DE PROCEDIMENTOS KG BEAUTY ---\n${menuText}\n--- FIM DO MENU ---\n\nCom base no menu acima, ajude esta cliente.\n\nDesejo da cliente: "${userQuery}"\n\nSua recomendação:`;

                try {
                    const resultText = await generateContent(userPrompt, systemPrompt);
                    advisorResult.innerHTML = `<div class="gemini-response p-3 bg-gray-50 rounded-lg border border-gray-200">${resultText}</div>`;
                } catch (error) {
                    console.error("Error calling Gemini API:", error);
                    advisorResult.innerHTML = `<p class="text-red-500 text-sm">Desculpe, não foi possível obter uma recomendação no momento. Tente novamente mais tarde.</p>`;
                }
            });
            
            // --- Lógica das Dicas de Cuidado ---
            
            document.querySelectorAll('.generate-aftercare-btn').forEach(button => {
                button.addEventListener('click', async (event) => {
                    const procedureName = event.target.dataset.procedure;
                    
                    aftercareTitle.textContent = `✨ Dicas para ${procedureName}`;
                    aftercareResult.innerHTML = '<div class="flex justify-center items-center p-4"><div class="spinner"></div></div>';
                    aftercareModal.classList.remove('hidden');

                    const prompt = `Como especialista da KG Beauty, forneça uma lista de dicas de cuidados essenciais pós-procedimento para "${procedureName}". As dicas devem ser em formato de lista com marcadores (use '- ' no início de cada item), fáceis de entender para uma cliente, e focadas em maximizar a durabilidade e os resultados do procedimento. Fale em português do Brasil, com um tom profissional e cuidadoso. Não use Markdown.`;
                    
                    try {
                        const resultText = await generateContent(prompt);
                        aftercareResult.innerHTML = `<div class="gemini-response">${resultText}</div>`;
                    } catch (error) {
                        console.error("Error calling Gemini API:", error);
                        aftercareResult.innerHTML = `<p class="text-red-500 text-sm">Desculpe, não foi possível obter as dicas no momento. Tente novamente mais tarde.</p>`;
                    }
                });
            });

            // Fecha o modal de dicas
            closeAftercareModal.addEventListener('click', () => {
                aftercareModal.classList.add('hidden');
            });
            
            // --- Lógica da Explicação de Termo ---
            
            document.querySelectorAll('.generate-explanation-btn').forEach(button => {
                button.addEventListener('click', async (event) => {
                    // Usar currentTarget para garantir que pegamos o botão, mesmo se o clique for no ícone dentro dele
                    const procedureName = event.currentTarget.dataset.procedure;
                    
                    explanationTitle.textContent = `✨ O que é ${procedureName}?`;
                    explanationResult.innerHTML = '<div class="flex justify-center items-center p-4"><div class="spinner"></div></div>';
                    explanationModal.classList.remove('hidden');

                    const prompt = `Como especialista da KG Beauty, explique o procedimento "${procedureName}" para uma cliente de forma muito simples, amigável e breve (máximo de 3-4 frases). Evite jargões técnicos. Foque no resultado final que a cliente verá. Fale em português do Brasil. Não use Markdown.`;
                    
                    try {
                        const resultText = await generateContent(prompt);
                        explanationResult.innerHTML = `<div class="gemini-response">${resultText}</div>`;
                    } catch (error) {
                        console.error("Error calling Gemini API:", error);
                        explanationResult.innerHTML = `<p class="text-red-500 text-sm">Desculpe, não foi possível obter a explicação no momento. Tente novamente mais tarde.</p>`;
                    }
                });
            });

            // Fecha o modal de explicação
            closeExplanationModal.addEventListener('click', () => {
                explanationModal.classList.add('hidden');
            });

            // --- Funções Auxiliares ---
            
            // Função para extrair o texto do menu do HTML
            function getMenuAsText() {
                const menuContainer = document.getElementById('menu-container');
                let text = '';
                
                const sections = menuContainer.querySelectorAll('section');
                sections.forEach(section => {
                    const title = section.querySelector('h1').textContent;
                    text += `\n${title.toUpperCase()}\n\n`;
                    
                    const items = section.querySelectorAll('.procedure-item');
                    items.forEach(item => {
                        const name = item.querySelector('h2').textContent.trim();
                        const price = item.querySelector('p:not([class*="text-gray-600"])').textContent.trim();
                        const descriptionEl = item.querySelector('p[class*="text-gray-600"]');
                        const description = descriptionEl ? descriptionEl.textContent.trim() : '';
                        text += `${name} - ${price}\n`;
                        if(description) {
                           text += `${description}\n`;
                        }
                        text += '\n';
                    });
                });
                return text;
            }

            // Função principal para chamar a API Gemini
            async function generateContent(userQuery, systemPrompt = null) {
                const apiKey = "AIzaSyClwv4goMd2zgNoiyftF5UA1IBWnsPILQs"; // API Key é gerenciada pelo ambiente de execução
                const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash-preview-09-2025:generateContent?key=${apiKey}`;

                const payload = {
                    contents: [{ parts: [{ text: userQuery }] }],
                };
                
                if (systemPrompt) {
                    payload.systemInstruction = {
                        parts: [{ text: systemPrompt }]
                    };
                }

                let response;
                let attempts = 0;
                const maxAttempts = 5;
                let delay = 1000; // 1 segundo

                while (attempts < maxAttempts) {
                    try {
                        response = await fetch(apiUrl, {
                            method: 'POST',
                            headers: { 'Content-Type': 'application/json' },
                            body: JSON.stringify(payload)
                        });

                        if (response.ok) {
                            const result = await response.json();
                            const candidate = result.candidates?.[0];
                            if (candidate && candidate.content?.parts?.[0]?.text) {
                                return candidate.content.parts[0].text;
                            } else {
                                throw new Error("Resposta da API inválida ou vazia.");
                            }
                        } else if (response.status === 429 || response.status >= 500) {
                            // Erro de "Too Many Requests" ou erro de servidor, tentar novamente
                            console.warn(`Tentativa ${attempts + 1} falhou com status ${response.status}. Tentando novamente em ${delay}ms...`);
                            await new Promise(resolve => setTimeout(resolve, delay));
                            delay *= 2; // Aumenta o tempo de espera (backoff exponencial)
                            attempts++;
                        } else {
                            // Outro tipo de erro, não tentar novamente
                            const errorBody = await response.text();
                            console.error("Erro na API:", response.status, errorBody);
                            throw new Error(`Erro na API com status: ${response.status}`);
                        }
                    } catch (error) {
                        console.error(`Erro na tentativa ${attempts + 1}:`, error);
                         if (attempts + 1 >= maxAttempts) {
                             throw error; // Lança o erro após a última tentativa
                         }
                        await new Promise(resolve => setTimeout(resolve, delay));
                        delay *= 2;
                        attempts++;
                    }
                }
                throw new Error("Não foi possível se comunicar com a API após várias tentativas.");
            }
        });
    </script>
</body>
</html>
