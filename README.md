<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <title>qualquer coisa menos um Simulador ENEM</title>
  <link rel="stylesheet" href="https://unpkg.com/lucide@latest/dist/umd/lucide.min.css">
  <style>
    * {
      box-sizing: border-box;
      transition: all 0.3s ease;
    }

    body {
      font-family: 'Segoe UI', sans-serif;
      background: #f4f6f8;
      margin: 0;
      padding: 0;
    }
  

    header {
      background: linear-gradient(90deg, #3f51b5, #5c6bc0);
      color: white;
      padding: 20px;
      text-align: center;
      font-size: 26px;
      font-weight: bold;
      letter-spacing: 1px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.2);
    }

    main {
      max-width: 850px;
      margin: 30px auto;
      background: white;
      padding: 30px;
      border-radius: 16px;
      box-shadow: 0 6px 16px rgba(0,0,0,0.1);
    }

    h1, h2 {
      text-align: center;
      color: #333;
    }

    .question-container {
      margin-bottom: 30px;
      padding: 25px;
      background: #f9f9f9;
      border-radius: 12px;
      border-left: 6px solid #3f51b5;
    }

    .question-container.humanas {
      border-left-color: #388e3c;
    }

    .question {
      font-weight: bold;
      margin-bottom: 15px;
    }

    .options label {
      display: block;
      margin-bottom: 10px;
      cursor: pointer;
    }

    .options input {
      margin-right: 10px;
    }

    .hidden {
      display: none;
    }

    button {
      background-color: #3f51b5;
      color: white;
      border: none;
      padding: 12px 18px;
      margin: 10px 5px;
      border-radius: 10px;
      cursor: pointer;
      font-size: 16px;
      box-shadow: 0 3px 6px rgba(0,0,0,0.2);
    }

    button:hover {
      transform: scale(1.05);
      background-color: #303f9f;
    }

    .humanasBtn {
      background-color: #388e3c;
    }

    .humanasBtn:hover {
      background-color: #2e7d32;
    }

    #resultado p {
      border-bottom: 1px solid #eee;
      padding-bottom: 10px;
      margin-bottom: 10px;
    }

    #resultado h3 {
      text-align: center;
      color: #2e7d32;
    }

    .icon {
      vertical-align: middle;
      margin-right: 8px;
    }
 <style>
  .hidden {
    display: none;
  }
</style>
</head>
<body> 

  <!-- SCRIPTS -->
  <script src="https://unpkg.com/lucide@latest"></script>
  <script>
    lucide.createIcons();

    function rSimulado() {
      document.getElementById("tela-inicial").style.display = "none";
      document.getElementById("simulado-section").style.display = "block";
    }

    function iniciarSimulado(area) {
      alert("Simulado de " + area + " iniciado!");
      // Aqui depois você pode colocar a função que mostra as questões.
    }
  </script>
</body>
  <header><i data-lucide="file-text" class="icon"></i>Simulador ENEM</header>
  <main>
</div>
 <body class="bg-gray-100 flex items-center justify-center min-h-screen">

  <!-- TELA INICIAL -->
  <div id="tela-inicial" class="bg-white p-8 rounded-2xl shadow-md text-center">
    <h1 class="text-2xl font-bold mb-4">Bem-vindo ao Projeto ENEM</h1>
    <p class="mb-6">Escolha uma opção abaixo:</p>

    <button onclick="mostrarSimulado()" class="flex items-center justify-center gap-2 bg-blue-600 text-white px-6 py-3 rounded-xl shadow hover:bg-blue-700 mb-4">
      <i data-lucide="pencil-line"></i> Simulado
    </button>

    <button class="flex items-center justify-center gap-2 bg-green-600 text-white px-6 py-3 rounded-xl shadow hover:bg-green-700">
      <i data-lucide="lightbulb"></i> Indicação de Conteúdo
    </button>
  </div>

  <!-- SIMULADO - ESCOLHA DE ÁREA -->
  <div id="simulado-section" class="hidden bg-white p-8 rounded-2xl shadow-md text-center">
    <h1 class="text-3xl font-bold text-gray-900 flex items-center justify-center gap-2 mb-6">
      <i data-lucide="file-text"></i> Simulador ENEM
    </h1>

    <h2 class="text-2xl font-semibold mb-4 text-gray-800">Escolha a área:</h2>
    <div class="flex justify-center gap-4 mb-8">
  <button onclick="iniciarSimulado('exatas')" class="flex items-center justify-center gap-2 bg-purple-600 text-white px-6 py-3 rounded-xl shadow hover:bg-purple-700 mb-4">
    <i data-lucide="atom"></i> Exatas
  </button>
  <button onclick="iniciarSimulado('humanas')" class="flex items-center justify-center gap-2 bg-yellow-600 text-white px-6 py-3 rounded-xl shadow hover:bg-yellow-700">
    <i data-lucide="book-open"></i> Humanas
  </button>
</div> <!-- fechamento correto da div -->
    <div id="simulado" class="hidden">
  <div id="questionario" class="mb-6"></div>
  <div class="text-center">
    <button onclick="anterior()" class="bg-gray-300 px-4 py-2 rounded-xl mx-1"><i data-lucide="arrow-left"></i> Anterior</button>
    <button onclick="proxima()" class="bg-gray-300 px-4 py-2 rounded-xl mx-1"><i data-lucide="arrow-right"></i> Próxima</button>
    <button id="finalizarBtn" class="hidden bg-green-600 text-white px-4 py-2 rounded-xl mx-1" onclick="finalizarSimulado()"><i data-lucide="check-circle"></i> Finalizar</button>
  </div>
</div>
</div>

  <!-- SCRIPTS -->
  <script src="https://unpkg.com/lucide@latest"></script>
  <script>
    lucide.createIcons();

    function mostrarSimulado() {
      document.getElementById("tela-inicial").style.display = "none";
      document.getElementById("simulado-section").style.display = "block";
    }

    function iniciarSimulado(area) {
      alert("Simulado de " + area + " iniciado!");
    }
  </script>
</body>
<div id="simulado" class="hidden">
      <div id="questionario"></div>
      <div style="text-align:center;">
        <button onclick="anterior()"><i data-lucide="arrow-left" class="icon"></i>Anterior</button>
        <button onclick="proxima()"><i data-lucide="arrow-right" class="icon"></i>Próxima</button>
        <button id="finalizarBtn" class="hidden" onclick="finalizarSimulado()"><i data-lucide="check-circle" class="icon"></i>Finalizar</button>
        <button onclick="mostrarSimulado()">Simulado</button>
      </div>
  <div style="text-align: center; margin-top: 30px;">
    <button onclick="window.location.reload()" style="padding: 12px 20px; background-color: #4CAF50; color: white; border: none; border-radius: 8px; cursor: pointer;">
      Voltar para a Página Inicial
    </button>
  </div>
</div>
    </div>
<div id="resultado" class="hidden"></div>
  </section>

  <!-- Indicação de conteúdo -->
  <section id="indicacao" class="hidden">
    <h2 style="text-align:center;">Indicação de Conteúdo</h2>
    <p style="text-align:center;">Baseado nos seus erros, aqui aparecerão recomendações personalizadas.</p>
    <!-- Aqui você pode futuramente inserir uma lógica para indicar conteúdos -->
  </section>
</main>
    <div id="areaSelection" class="hidden">
  <p style="text-align:center;">Escolha a área:</p>
  <div style="text-align:center;">
    <button onclick="startSimulado('exatas')"><i data-lucide="flask-conical" class="icon"></i> Exatas</button>
    <button onclick="startSimulado('humanas')"><i data-lucide="book-open" class="icon"></i> Humanas</button>
  </div>
      
</div>

    <div id="simulado" class="hidden">
      <div id="questionario"></div>
      <div style="text-align:center;">
        <button onclick="anterior()"><i data-lucide="arrow-left" class="icon"></i>Anterior</button>
        <button onclick="proxima()"><i data-lucide="arrow-right" class="icon"></i>Próxima</button>
        <button id="finalizarBtn" class="hidden" onclick="finalizarSimulado()"><i data-lucide="check-circle" class="icon"></i>Finalizar</button>
        <div class="text-center mt-6">
  <button onclick="voltarInicio()" class="bg-red-500 text-white px-6 py-3 rounded-xl shadow hover:bg-red-600 transition flex items-center justify-center gap-2">
    <i data-lucide="arrow-left"></i> Voltar ao Início
  </button>
</div>
        
      </div><div style="text-align: center; margin-top: 30px;">
</div>
    </div>

    <div id="resultado" class="hidden"></div>
  </main>

  <script src="https://unpkg.com/lucide@latest"></script>
  <script>
  lucide.createIcons();

    ]
  };
<script>
  let perguntas = [];
  let perguntaAtual = 0;
  let respostas = [];

  function iniciarSimulado(area) {
    document.getElementById(areaSelection').classList.add('hidden');
    document.getElementById('simulado').classList.remove('hidden');
    respostas = new Array(questoes[area].length).fill(null);
    indice = 0;
    renderizarQuestao(area);
  }

  function renderizarQuestao(area) {
    const questaoAtual = questoes[area][indice];
    let html = `<div class="question-container ${area === 'humanas' ? 'humanas' : ''}">
      <div class="question">${questaoAtual.pergunta}</div>
      <div class="options">`;
    questaoAtual.opcoes.forEach((opcao, i) => {
      html += `<label><input type="radio" name="resposta" value="${i}" ${respostas[indice] === i ? 'checked' : ''}>${opcao}</label>`;
    });
    html += `</div></div>`;
    document.getElementById('questionario').innerHTML = html;

    document.getElementById('finalizarBtn').classList.toggle('hidden', indice !== questoes[area].length - 1);
  }

  function proxima() {
    const selecionada = document.querySelector('input[name="resposta"]:checked');
    if (selecionada) respostas[indice] = parseInt(selecionada.value);
    if (indice < respostas.length - 1) {
      indice++;
      renderizarQuestao(getAreaAtual());
    }
  }

  function anterior() {
    if (indice > 0) {
      indice--;
      renderizarQuestao(getAreaAtual());
    }
  }

  function getAreaAtual() {
    return document.querySelector('.question-container.humanas') ? 'humanas' : 'exatas';
  }

  function finalizarSimulado() {
    const area = getAreaAtual();
    let resultadoHTML = '<h3>Resultado do Simulado</h3>';
    questoes[area].forEach((q, i) => {
      const correta = q.resposta === respostas[i];
      resultadoHTML += `<p><strong>${q.pergunta}</strong><br>
        Sua resposta: ${q.opcoes[respostas[i]] || 'Não respondida'}<br>
        Correta: ${q.opcoes[q.resposta]}<br>
        <em>${correta ? 'Correta!' : 'Errada.'} ${q.explicacao}</em></p>`;
    });
    document.getElementById('simulado').classList.add('hidden');
    document.getElementById('resultado').classList.remove('hidden');
    document.getElementById('resultado').innerHTML = resultadoHTML;
  }
</script>
</script>
<script>
let perguntas = [];
let perguntaAtual = 0;
let respostas = [];
const questoes = {
  exatas: [
    {
      pergunta: "1. Um trem percorre uma distância de 540 km em 6 horas. Se sua velocidade aumenta em 10 km/h, quanto tempo levaria para percorrer a mesma distância?",
      opcoes: ["4h", "4,5h", "5h", "5,5h"],
      resposta: 2,
      explicacao: "Velocidade inicial = 90 km/h. Nova velocidade = 100 km/h. Tempo = 540 ÷ 100 = 5h."
    },
    {
      pergunta: "2. Uma urna contém 5 bolas vermelhas e 3 azuis. Qual a probabilidade de se retirar uma azul ao acaso?",
      opcoes: ["1/2", "3/8", "5/8", "3/5"],
      resposta: 1,
      explicacao: "Probabilidade = favoráveis / total = 3 / 8."
    },
    {
      pergunta: "3. Qual o valor de x na equação: log(x) + log(2) = 1?",
      opcoes: ["2", "5", "10", "20"],
      resposta: 0,
      explicacao: "log(x) + log(2) = log(2x) = 1 → 2x = 10 → x = 5."
    },
    {
      pergunta: "4. Um resistor de 10Ω é atravessado por uma corrente de 2A. Qual a potência dissipada?",
      opcoes: ["10W", "20W", "40W", "100W"],
      resposta: 2,
      explicacao: "P = R × I² = 10 × 4 = 40W."
    },
    {
      pergunta: "5. Qual o volume de uma esfera com raio de 3 cm? (Use π ≈ 3)",
      opcoes: ["84 cm³", "108 cm³", "113 cm³", "124 cm³"],
      resposta: 1,
      explicacao: "V = 4/3 × π × r³ = 4/3 × 3 × 27 = 108 cm³."
    },
    {
      pergunta: "6. Uma PA tem primeiro termo 5 e razão 3. Qual o 20º termo?",
      opcoes: ["62", "65", "70", "75"],
      resposta: 1,
      explicacao: "An = a1 + (n - 1) × r = 5 + 19 × 3 = 62."
    },
    {
      pergunta: "7. A aceleração centrípeta de um corpo em movimento circular é dada por:",
      opcoes: ["v²/r", "v × r", "r²/v", "1/2 × v × r"],
      resposta: 0,
      explicacao: "ac = v² / r."
    },
    {
      pergunta: "8. O pH de uma solução é 3. Isso indica que a concentração de íons H+ é aproximadamente:",
      opcoes: ["10⁻³ mol/L", "10³ mol/L", "3 mol/L", "10⁻¹ mol/L"],
      resposta: 0,
      explicacao: "pH = -log[H+] → [H+] = 10⁻³ mol/L."
    },
    {
      pergunta: "9. Se o determinante de uma matriz 2x2 é 0, podemos afirmar que:",
      opcoes: ["Ela tem inversa", "É uma matriz identidade", "Não tem inversa", "É simétrica"],
      resposta: 2,
      explicacao: "Determinante zero → matriz não inversível."
    },
    {
      pergunta: "10. Um carro faz 12 km/L de gasolina. Com 30L, quantos km ele percorre?",
      opcoes: ["360 km", "240 km", "300 km", "280 km"],
      resposta: 0,
      explicacao: "12 × 30 = 360 km."
    }
  ],

  humanas: [
    {
      pergunta: "1. (Texto) 'A razão se eleva acima do mito'. Com base no pensamento iluminista, esse trecho representa:",
      opcoes: ["A valorização da fé", "A defesa da tradição", "A crítica à ciência", "A exaltação da razão"],
      resposta: 3,
      explicacao: "O Iluminismo defendia o uso da razão como guia da humanidade."
    },
    {
      pergunta: "2. A Guerra Fria foi caracterizada principalmente por:",
      opcoes: ["Conflitos diretos entre EUA e URSS", "Domínio nuclear da Europa", "Disputa ideológica sem confronto direto", "Neutralidade entre blocos"],
      resposta: 2,
      explicacao: "A Guerra Fria foi marcada por uma disputa indireta entre EUA e URSS."
    },
    {
      pergunta: "3. O conceito de 'Contrato Social', de Rousseau, defende:",
      opcoes: ["A obediência cega ao rei", "A renúncia à liberdade", "A legitimidade do poder pelo povo", "A concentração do poder na igreja"],
      resposta: 2,
      explicacao: "Para Rousseau, o poder deve emanar da vontade geral."
    },
    {
      pergunta: "4. O Brasil deixou de ser colônia em:",
      opcoes: ["1500", "1822", "1889", "1930"],
      resposta: 1,
      explicacao: "Em 1822, ocorreu a independência do Brasil."
    },
    {
      pergunta: "5. 'O trabalho alienado', segundo Marx, ocorre quando:",
      opcoes: ["O trabalhador domina os meios de produção", "Há equilíbrio entre capital e trabalho", "O trabalhador não se reconhece naquilo que produz", "Há mais-valia justa"],
      resposta: 2,
      explicacao: "Alienação é a perda de sentido do trabalho, central na crítica de Marx."
    },
    {
      pergunta: "6. A urbanização no Brasil se intensificou durante:",
      opcoes: ["O ciclo do ouro", "A colonização", "O período militar", "O século XX, com industrialização"],
      resposta: 3,
      explicacao: "A urbanização acelerou-se com a industrialização e êxodo rural no século XX."
    },
    {
      pergunta: "7. A globalização é um processo que:",
      opcoes: ["Diminui o comércio", "Reduz conexões", "Aumenta a interdependência entre países", "Favorece o isolamento"],
      resposta: 2,
      explicacao: "Globalização promove trocas comerciais, culturais e tecnológicas globais."
    },
    {
      pergunta: "8. A ditadura militar no Brasil ocorreu entre:",
      opcoes: ["1945 e 1960", "1964 e 1985", "1950 e 1988", "1930 e 1945"],
      resposta: 1,
      explicacao: "A ditadura teve início em 1964 e durou até 1985."
    },
    {
      pergunta: "9. A Revolução Industrial provocou:",
      opcoes: ["O fim do capitalismo", "O avanço do feudalismo", "Mudanças profundas no trabalho e na produção", "A valorização do artesanato"],
      resposta: 2,
      explicacao: "Houve mecanização, novas relações de trabalho e urbanização intensa."
    },
    {
      pergunta: "10. A Constituição de 1988 é conhecida como:",
      opcoes: ["Constituição Monárquica", "Constituição de Vargas", "Constituição Cidadã", "Carta de 1967"],
      resposta: 2,
      explicacao: "Chamada de 'Constituição Cidadã' por ampliar os direitos sociais e democráticos."
    }
  ]
};
function iniciarSimulado(area) {
  document.getElementById("simulado-section").classList.add("hidden");
  document.getElementById("simulado").classList.remove("hidden");

  perguntas = [...questoes[area]];
  perguntaAtual = 0;
  respostas = new Array(perguntas.length).fill(null);
  mostrarPergunta();
}
function voltarInicio() {
  document.getElementById("simulado").classList.add("hidden");
  document.getElementById("simulado-section").classList.remove("hidden");
}
function mostrarPergunta() {
  const pergunta = perguntas[perguntaAtual];
  if (!pergunta) return;

  const opcoesHtml = pergunta.opcoes.map((opcao, i) => `
    <label class="block my-2">
      <input type="radio" name="resposta" value="${i}" class="mr-2" ${respostas[perguntaAtual] === i ? 'checked' : ''}>
      ${opcao}
    </label>
  `).join("");

  document.getElementById("questionario").innerHTML = `
    <div class="text-left">
      <p class="text-lg font-semibold mb-4">${perguntaAtual + 1}. ${pergunta.pergunta}</p>
      ${opcoesHtml}
    </div>
  `;

  document.getElementById("finalizarBtn").classList.toggle("hidden", perguntaAtual !== perguntas.length - 1);
}

function proxima() {
  const selecionada = document.querySelector('input[name="resposta"]:checked');
  if (selecionada) respostas[perguntaAtual] = parseInt(selecionada.value);
  if (perguntaAtual < perguntas.length - 1) {
    perguntaAtual++;
    mostrarPergunta();
  }
}

function anterior() {
  if (perguntaAtual > 0) {
    perguntaAtual--;
    mostrarPergunta();
  }
}

function finalizarSimulado() {
  const resultadoDiv = document.getElementById("resultado");
  let acertos = 0;
  let resultadoHTML = "<h2 class='text-xl font-bold mb-4'>Resultado</h2>";

  perguntas.forEach((q, i) => {
    const correta = q.resposta;
    const marcada = respostas[i];
    const corretaTexto = q.opcoes[correta];
    const marcadaTexto = marcada != null ? q.opcoes[marcada] : "Não respondida";
    const acertou = marcada === correta;

    if (acertou) acertos++;

    resultadoHTML += `
      <p><strong>${i + 1}. ${q.pergunta}</strong><br>
      Sua resposta: ${marcadaTexto}<br>
      Correta: ${corretaTexto}<br>
      <span style='color: ${acertou ? 'green' : 'red'}'>${acertou ? 'Correta' : 'Errada'}</span><br>
      <em>Explicação: ${q.explicacao}</em></p><hr>
    `;
  });

  resultadoHTML += `<h3 class='text-lg font-semibold mt-4'>Você acertou ${acertos} de ${perguntas.length} questões.</h3>`;
  document.getElementById("simulado").classList.add("hidden");
  resultadoDiv.classList.remove("hidden");
  resultadoDiv.innerHTML = resultadoHTML;
}
</script>
</body>
</html>
