[index.html](https://github.com/user-attachments/files/24603281/index.html)
<!doctype html>
<html lang="pt-BR" class="h-full">
 <head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mapa das Dívidas - Organize suas Finanças</title>
  <script src="https://cdn.tailwindcss.com"></script>

  <!-- Removidos SDKs do Canva (não necessários fora do Canva) -->
  <!-- <script src="/_sdk/element_sdk.js"></script> -->
  <!-- <script src="/_sdk/data_sdk.js" type="text/javascript"></script> -->

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&display=swap" rel="stylesheet">
  <style>
    body { box-sizing: border-box; font-family: 'Plus Jakarta Sans', sans-serif; }
    .gradient-text {
      background: linear-gradient(135deg, #10b981 0%, #059669 100%);
      -webkit-background-clip: text; -webkit-text-fill-color: transparent;
      background-clip: text;
    }
    .hero-gradient { background: linear-gradient(180deg, #022c22 0%, #064e3b 50%, #065f46 100%); }
    .card-glow { box-shadow: 0 0 60px rgba(16, 185, 129, 0.15); }
    .pulse-glow { animation: pulseGlow 2s ease-in-out infinite; }
    @keyframes pulseGlow { 0%, 100% { box-shadow: 0 0 20px rgba(16, 185, 129, 0.4); } 50% { box-shadow: 0 0 40px rgba(16, 185, 129, 0.6); } }
    .float { animation: float 6s ease-in-out infinite; }
    @keyframes float { 0%, 100% { transform: translateY(0px); } 50% { transform: translateY(-20px); } }
    .slide-up { animation: slideUp 0.8s ease-out forwards; }
    @keyframes slideUp { from { opacity: 0; transform: translateY(30px); } to { opacity: 1; transform: translateY(0); } }
    .check-item { animation: checkIn 0.5s ease-out forwards; opacity: 0; }
    @keyframes checkIn { from { opacity: 0; transform: translateX(-20px); } to { opacity: 1; transform: translateX(0); } }
    .testimonial-card { backdrop-filter: blur(10px); }
  </style>
 </head>
 <body class="h-full bg-slate-950 text-white overflow-auto">

  <!-- Hero Section -->
  <section class="hero-gradient min-h-screen relative overflow-hidden">
   <div class="absolute inset-0 opacity-10">
    <svg class="w-full h-full" viewBox="0 0 100 100" preserveAspectRatio="none">
     <defs>
      <pattern id="grid" width="10" height="10" patternUnits="userSpaceOnUse">
       <path d="M 10 0 L 0 0 0 10" fill="none" stroke="currentColor" stroke-width="0.5" />
      </pattern>
     </defs>
     <rect width="100" height="100" fill="url(#grid)" />
    </svg>
   </div>

   <div class="absolute top-20 left-10 w-20 h-20 bg-emerald-500/10 rounded-full blur-xl float"></div>
   <div class="absolute top-40 right-20 w-32 h-32 bg-emerald-400/10 rounded-full blur-2xl float" style="animation-delay: -2s;"></div>
   <div class="absolute bottom-40 left-1/4 w-24 h-24 bg-emerald-600/10 rounded-full blur-xl float" style="animation-delay: -4s;"></div>

   <div class="relative z-10 max-w-6xl mx-auto px-6 py-16 md:py-24">
    <div class="flex justify-center mb-8 slide-up">
     <div class="inline-flex items-center gap-2 bg-emerald-500/20 border border-emerald-500/30 rounded-full px-4 py-2">
      <span class="w-2 h-2 bg-emerald-400 rounded-full animate-pulse"></span>
      <span class="text-emerald-300 text-sm font-medium">+2.500 pessoas já organizaram suas finanças</span>
     </div>
    </div>

    <h1 id="hero-title" class="text-4xl md:text-6xl lg:text-7xl font-extrabold text-center mb-6 slide-up" style="animation-delay: 0.1s;">
      <span class="text-white">Mapa das</span> <span class="gradient-text"> Dívidas</span>
    </h1>

    <p id="hero-subtitle" class="text-xl md:text-2xl text-emerald-100/80 text-center max-w-3xl mx-auto mb-10 slide-up" style="animation-delay: 0.2s;">
      A planilha definitiva para você sair do vermelho, organizar suas dívidas e retomar o controle da sua vida financeira
    </p>

    <div class="flex justify-center mb-16 slide-up" style="animation-delay: 0.3s;">
      <button id="cta-button-hero" class="group relative bg-emerald-500 hover:bg-emerald-400 text-slate-900 font-bold text-lg md:text-xl px-10 py-5 rounded-2xl transition-all duration-300 transform hover:scale-105 pulse-glow">
        <span class="flex items-center gap-3">
          QUERO SAIR DAS DÍVIDAS AGORA
          <svg class="w-6 h-6 group-hover:translate-x-1 transition-transform" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 7l5 5m0 0l-5 5m5-5H6" />
          </svg>
        </span>
      </button>
    </div>

    <div class="relative max-w-4xl mx-auto slide-up" style="animation-delay: 0.4s;">
     <div class="bg-gradient-to-br from-slate-800/80 to-slate-900/80 rounded-3xl p-4 md:p-8 card-glow border border-emerald-500/20">
      <svg viewBox="0 0 800 450" class="w-full rounded-2xl">
       <rect width="800" height="450" fill="#1e293b" />
       <rect x="0" y="0" width="800" height="50" fill="#0f172a" />
       <text x="30" y="32" fill="#10b981" font-size="18" font-weight="bold">📊 MAPA DAS DÍVIDAS - Controle Total</text>
       <rect x="0" y="50" width="800" height="40" fill="#064e3b" />
       <text x="30" y="77" fill="white" font-size="14" font-weight="600">Credor</text>
       <text x="180" y="77" fill="white" font-size="14" font-weight="600">Valor Total</text>
       <text x="310" y="77" fill="white" font-size="14" font-weight="600">Parcelas</text>
       <text x="420" y="77" fill="white" font-size="14" font-weight="600">Juros %</text>
       <text x="520" y="77" fill="white" font-size="14" font-weight="600">Status</text>
       <text x="650" y="77" fill="white" font-size="14" font-weight="600">Prioridade</text>

       <rect x="0" y="90" width="800" height="45" fill="#1e293b" />
       <text x="30" y="120" fill="#e2e8f0" font-size="13">Cartão Nubank</text>
       <text x="180" y="120" fill="#f87171" font-size="13">R$ 3.450,00</text>
       <text x="310" y="120" fill="#e2e8f0" font-size="13">12x de R$ 345</text>
       <text x="420" y="120" fill="#fbbf24" font-size="13">14.9%</text>
       <rect x="520" y="107" width="80" height="24" rx="12" fill="#dc2626" />
       <text x="535" y="124" fill="white" font-size="11">Em aberto</text>
       <rect x="650" y="107" width="60" height="24" rx="12" fill="#ef4444" />
       <text x="663" y="124" fill="white" font-size="11">ALTA</text>

       <rect x="0" y="135" width="800" height="45" fill="#0f172a" />
       <text x="30" y="165" fill="#e2e8f0" font-size="13">Empréstimo Banco</text>
       <text x="180" y="165" fill="#f87171" font-size="13">R$ 8.200,00</text>
       <text x="310" y="165" fill="#e2e8f0" font-size="13">24x de R$ 420</text>
       <text x="420" y="165" fill="#fbbf24" font-size="13">2.5%</text>
       <rect x="520" y="152" width="80" height="24" rx="12" fill="#f59e0b" />
       <text x="530" y="169" fill="white" font-size="11">Pagando</text>
       <rect x="650" y="152" width="60" height="24" rx="12" fill="#f59e0b" />
       <text x="660" y="169" fill="white" font-size="11">MÉDIA</text>

       <rect x="0" y="180" width="800" height="45" fill="#1e293b" />
       <text x="30" y="210" fill="#e2e8f0" font-size="13">Financiamento Carro</text>
       <text x="180" y="210" fill="#4ade80" font-size="13">R$ 15.000,00</text>
       <text x="310" y="210" fill="#e2e8f0" font-size="13">48x de R$ 450</text>
       <text x="420" y="210" fill="#4ade80" font-size="13">1.2%</text>
       <rect x="520" y="197" width="80" height="24" rx="12" fill="#22c55e" />
       <text x="530" y="214" fill="white" font-size="11">Em dia</text>
       <rect x="650" y="197" width="60" height="24" rx="12" fill="#22c55e" />
       <text x="660" y="214" fill="white" font-size="11">BAIXA</text>

       <rect x="0" y="250" width="800" height="200" fill="#0f172a" />
       <rect x="30" y="280" width="220" height="100" rx="15" fill="#064e3b" />
       <text x="50" y="315" fill="#6ee7b7" font-size="12">TOTAL DE DÍVIDAS</text>
       <text x="50" y="355" fill="white" font-size="28" font-weight="bold">R$ 26.650</text>

       <rect x="280" y="280" width="220" height="100" rx="15" fill="#7c2d12" />
       <text x="300" y="315" fill="#fca5a5" font-size="12">JUROS ACUMULADOS</text>
       <text x="300" y="355" fill="white" font-size="28" font-weight="bold">R$ 4.230</text>

       <rect x="530" y="280" width="220" height="100" rx="15" fill="#1e3a5f" />
       <text x="550" y="315" fill="#93c5fd" font-size="12">ECONOMIA PROJETADA</text>
       <text x="550" y="355" fill="#4ade80" font-size="28" font-weight="bold">R$ 2.890</text>

       <rect x="30" y="410" width="740" height="20" rx="10" fill="#1e293b" />
       <rect x="30" y="410" width="280" height="20" rx="10" fill="url(#progressGradient)" />
       <defs>
        <linearGradient id="progressGradient" x1="0%" y1="0%" x2="100%" y2="0%">
         <stop offset="0%" style="stop-color:#10b981" />
         <stop offset="100%" style="stop-color:#059669" />
        </linearGradient>
       </defs>
       <text x="400" y="425" fill="white" font-size="12" text-anchor="middle">38% das dívidas quitadas 🎯</text>
      </svg>
     </div>
    </div>
   </div>
  </section>

  <!-- Pain Points Section -->
  <section class="bg-slate-900 py-20">
   <div class="max-w-6xl mx-auto px-6">
    <h2 class="text-3xl md:text-4xl font-bold text-center mb-4">Você se identifica com isso?</h2>
    <p class="text-slate-400 text-center mb-12 text-lg">Se pelo menos uma dessas situações é familiar, esse produto foi feito para você</p>
    <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-6">
     <div class="bg-slate-800/50 border border-red-500/20 rounded-2xl p-6 hover:border-red-500/40 transition-all duration-300">
      <div class="w-14 h-14 bg-red-500/20 rounded-xl flex items-center justify-center mb-4"><span class="text-3xl">😰</span></div>
      <h3 class="text-xl font-semibold mb-2 text-red-400">Perda de controle</h3>
      <p class="text-slate-400">Não sabe exatamente quanto deve e para quem. As dívidas parecem um emaranhado impossível de entender.</p>
     </div>
     <div class="bg-slate-800/50 border border-red-500/20 rounded-2xl p-6 hover:border-red-500/40 transition-all duration-300">
      <div class="w-14 h-14 bg-red-500/20 rounded-xl flex items-center justify-center mb-4"><span class="text-3xl">💳</span></div>
      <h3 class="text-xl font-semibold mb-2 text-red-400">Juros acumulando</h3>
      <p class="text-slate-400">Cada mês que passa, os juros crescem e você sente que está trabalhando só para pagar banco.</p>
     </div>
     <div class="bg-slate-800/50 border border-red-500/20 rounded-2xl p-6 hover:border-red-500/40 transition-all duration-300">
      <div class="w-14 h-14 bg-red-500/20 rounded-xl flex items-center justify-center mb-4"><span class="text-3xl">😔</span></div>
      <h3 class="text-xl font-semibold mb-2 text-red-400">Ansiedade financeira</h3>
      <p class="text-slate-400">Noites mal dormidas pensando em como vai pagar as contas do próximo mês.</p>
     </div>
     <div class="bg-slate-800/50 border border-red-500/20 rounded-2xl p-6 hover:border-red-500/40 transition-all duration-300">
      <div class="w-14 h-14 bg-red-500/20 rounded-xl flex items-center justify-center mb-4"><span class="text-3xl">📉</span></div>
      <h3 class="text-xl font-semibold mb-2 text-red-400">Nome sujo</h3>
      <p class="text-slate-400">Restrição no CPF impedindo você de realizar sonhos como financiar uma casa ou carro.</p>
     </div>
     <div class="bg-slate-800/50 border border-red-500/20 rounded-2xl p-6 hover:border-red-500/40 transition-all duration-300">
      <div class="w-14 h-14 bg-red-500/20 rounded-xl flex items-center justify-center mb-4"><span class="text-3xl">🔄</span></div>
      <h3 class="text-xl font-semibold mb-2 text-red-400">Ciclo vicioso</h3>
      <p class="text-slate-400">Pega empréstimo para pagar outro empréstimo. A bola de neve só aumenta.</p>
     </div>
     <div class="bg-slate-800/50 border border-red-500/20 rounded-2xl p-6 hover:border-red-500/40 transition-all duration-300">
      <div class="w-14 h-14 bg-red-500/20 rounded-xl flex items-center justify-center mb-4"><span class="text-3xl">👨‍👩‍👧</span></div>
      <h3 class="text-xl font-semibold mb-2 text-red-400">Família afetada</h3>
      <p class="text-slate-400">As dívidas geram brigas, estresse e afetam o relacionamento com quem você ama.</p>
     </div>
    </div>
   </div>
  </section>

  <!-- Solution Section -->
  <section class="bg-gradient-to-b from-slate-900 to-emerald-950 py-20">
   <div class="max-w-6xl mx-auto px-6">
    <div class="text-center mb-16">
      <span class="inline-block bg-emerald-500/20 text-emerald-400 px-4 py-2 rounded-full text-sm font-semibold mb-4">A SOLUÇÃO</span>
      <h2 class="text-3xl md:text-5xl font-bold mb-6">O Mapa das Dívidas vai te dar <span class="gradient-text"> clareza total</span></h2>
      <p class="text-xl text-slate-300 max-w-2xl mx-auto">Uma planilha estratégica e visual que transforma o caos financeiro em um plano de ação claro e executável</p>
    </div>

    <div class="grid lg:grid-cols-2 gap-12 items-center">
     <div class="space-y-6">
      <div class="flex gap-4 items-start bg-slate-800/30 rounded-2xl p-6 border border-emerald-500/10 hover:border-emerald-500/30 transition-all">
       <div class="w-12 h-12 bg-emerald-500 rounded-xl flex items-center justify-center flex-shrink-0">
        <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 19v-6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2a2 2 0 002-2zm0 0V9a2 2 0 012-2h2a2 2 0 012 2v10m-6 0a2 2 0 002 2h2a2 2 0 002-2m0 0V5a2 2 0 012-2h2a2 2 0 012 2v14a2 2 0 01-2 2h-2a2 2 0 01-2-2z" /></svg>
       </div>
       <div><h3 class="text-xl font-semibold mb-2">Dashboard Visual Completo</h3><p class="text-slate-400">Veja todas as suas dívidas em um único lugar, com gráficos que mostram sua evolução e progresso.</p></div>
      </div>

      <div class="flex gap-4 items-start bg-slate-800/30 rounded-2xl p-6 border border-emerald-500/10 hover:border-emerald-500/30 transition-all">
       <div class="w-12 h-12 bg-emerald-500 rounded-xl flex items-center justify-center flex-shrink-0">
        <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 7h8m0 0v8m0-8l-8 8-4-4-6 6" /></svg>
       </div>
       <div><h3 class="text-xl font-semibold mb-2">Método Bola de Neve</h3><p class="text-slate-400">Sistema automático que prioriza quais dívidas pagar primeiro para economizar milhares em juros.</p></div>
      </div>

      <div class="flex gap-4 items-start bg-slate-800/30 rounded-2xl p-6 border border-emerald-500/10 hover:border-emerald-500/30 transition-all">
       <div class="w-12 h-12 bg-emerald-500 rounded-xl flex items-center justify-center flex-shrink-0">
        <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 7V3m8 4V3m-9 8h10M5 21h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z" /></svg>
       </div>
       <div><h3 class="text-xl font-semibold mb-2">Calendário de Pagamentos</h3><p class="text-slate-400">Nunca mais esqueça uma data de vencimento. Alertas visuais para cada compromisso.</p></div>
      </div>

      <div class="flex gap-4 items-start bg-slate-800/30 rounded-2xl p-6 border border-emerald-500/10 hover:border-emerald-500/30 transition-all">
       <div class="w-12 h-12 bg-emerald-500 rounded-xl flex items-center justify-center flex-shrink-0">
        <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8c-1.657 0-3 .895-3 2s1.343 2 3 2 3 .895 3 2-1.343 2-3 2m0-8c1.11 0 2.08.402 2.599 1M12 8V7m0 1v8m0 0v1m0-1c-1.11 0-2.08-.402-2.599-1M21 12a9 9 0 11-18 0 9 9 0 0118 0z" /></svg>
       </div>
       <div><h3 class="text-xl font-semibold mb-2">Simulador de Quitação</h3><p class="text-slate-400">Descubra em quantos meses você pode ficar livre das dívidas e quanto vai economizar.</p></div>
      </div>
     </div>

     <div class="relative">
      <div class="bg-gradient-to-br from-emerald-500/20 to-slate-800/50 rounded-3xl p-8 border border-emerald-500/20">
       <svg viewBox="0 0 400 400" class="w-full">
        <circle cx="200" cy="200" r="120" fill="none" stroke="#10b981" stroke-width="8" stroke-dasharray="20 10" opacity="0.3" />
        <circle cx="200" cy="200" r="80" fill="#064e3b" />
        <text x="200" y="190" text-anchor="middle" fill="white" font-size="16" font-weight="bold">VOCÊ NO</text>
        <text x="200" y="215" text-anchor="middle" fill="#10b981" font-size="20" font-weight="bold">CONTROLE</text>

        <g transform="translate(200, 60)"><circle r="35" fill="#1e293b" stroke="#10b981" stroke-width="2" /><text y="5" text-anchor="middle" fill="white" font-size="10">Dívidas</text><text y="18" text-anchor="middle" fill="#10b981" font-size="12" font-weight="bold">Mapeadas</text></g>
        <g transform="translate(320, 140)"><circle r="35" fill="#1e293b" stroke="#10b981" stroke-width="2" /><text y="5" text-anchor="middle" fill="white" font-size="10">Juros</text><text y="18" text-anchor="middle" fill="#10b981" font-size="12" font-weight="bold">Calculados</text></g>
        <g transform="translate(320, 260)"><circle r="35" fill="#1e293b" stroke="#10b981" stroke-width="2" /><text y="5" text-anchor="middle" fill="white" font-size="10">Prioridades</text><text y="18" text-anchor="middle" fill="#10b981" font-size="12" font-weight="bold">Definidas</text></g>
        <g transform="translate(200, 340)"><circle r="35" fill="#1e293b" stroke="#10b981" stroke-width="2" /><text y="5" text-anchor="middle" fill="white" font-size="10">Economia</text><text y="18" text-anchor="middle" fill="#10b981" font-size="12" font-weight="bold">Projetada</text></g>
        <g transform="translate(80, 260)"><circle r="35" fill="#1e293b" stroke="#10b981" stroke-width="2" /><text y="5" text-anchor="middle" fill="white" font-size="10">Progresso</text><text y="18" text-anchor="middle" fill="#10b981" font-size="12" font-weight="bold">Visível</text></g>
        <g transform="translate(80, 140)"><circle r="35" fill="#1e293b" stroke="#10b981" stroke-width="2" /><text y="5" text-anchor="middle" fill="white" font-size="10">Plano de</text><text y="18" text-anchor="middle" fill="#10b981" font-size="12" font-weight="bold">Ação</text></g>
       </svg>
      </div>
     </div>
    </div>
   </div>
  </section>

  <!-- Testimonials -->
  <section class="bg-slate-950 py-20">
   <div class="max-w-6xl mx-auto px-6">
    <h2 class="text-3xl md:text-4xl font-bold text-center mb-4">Quem usou, <span class="gradient-text">aprovou</span></h2>
    <p class="text-slate-400 text-center mb-12 text-lg">Veja o que nossos clientes estão dizendo</p>
    <div class="grid md:grid-cols-3 gap-6">
     <div class="bg-gradient-to-br from-slate-800/80 to-slate-900/80 rounded-2xl p-6 border border-slate-700/50 testimonial-card">
      <div class="flex gap-1 mb-4"><span class="text-yellow-400">★</span><span class="text-yellow-400">★</span><span class="text-yellow-400">★</span><span class="text-yellow-400">★</span><span class="text-yellow-400">★</span></div>
      <p class="text-slate-300 mb-6">"Em 8 meses consegui quitar R$ 12.000 em dívidas usando o método da planilha. Antes eu nem sabia por onde começar!"</p>
      <div class="flex items-center gap-3">
       <div class="w-12 h-12 bg-emerald-500/20 rounded-full flex items-center justify-center"><span class="text-xl">👩</span></div>
       <div><p class="font-semibold">Marina Santos</p><p class="text-sm text-slate-400">São Paulo, SP</p></div>
      </div>
     </div>

     <div class="bg-gradient-to-br from-slate-800/80 to-slate-900/80 rounded-2xl p-6 border border-slate-700/50 testimonial-card">
      <div class="flex gap-1 mb-4"><span class="text-yellow-400">★</span><span class="text-yellow-400">★</span><span class="text-yellow-400">★</span><span class="text-yellow-400">★</span><span class="text-yellow-400">★</span></div>
      <p class="text-slate-300 mb-6">"A visualização das dívidas me deu clareza. Descobri que estava pagando R$ 300/mês só de juros desnecessários!"</p>
      <div class="flex items-center gap-3">
       <div class="w-12 h-12 bg-emerald-500/20 rounded-full flex items-center justify-center"><span class="text-xl">👨</span></div>
       <div><p class="font-semibold">Ricardo Oliveira</p><p class="text-sm text-slate-400">Belo Horizonte, MG</p></div>
      </div>
     </div>

     <div class="bg-gradient-to-br from-slate-800/80 to-slate-900/80 rounded-2xl p-6 border border-slate-700/50 testimonial-card">
      <div class="flex gap-1 mb-4"><span class="text-yellow-400">★</span><span class="text-yellow-400">★</span><span class="text-yellow-400">★</span><span class="text-yellow-400">★</span><span class="text-yellow-400">★</span></div>
      <p class="text-slate-300 mb-6">"Simples de usar e super completa. Até minha esposa que não entendia nada de planilhas conseguiu usar!"</p>
      <div class="flex items-center gap-3">
       <div class="w-12 h-12 bg-emerald-500/20 rounded-full flex items-center justify-center"><span class="text-xl">👨</span></div>
       <div><p class="font-semibold">Carlos Eduardo</p><p class="text-sm text-slate-400">Curitiba, PR</p></div>
      </div>
     </div>
    </div>

    <p class="text-center text-slate-500 text-sm mt-8">
      *Depoimentos reais. Resultados variam de acordo com renda, disciplina e condições de cada pessoa.
    </p>
   </div>
  </section>

  <!-- Pricing Section -->
  <section id="pricing" class="bg-gradient-to-b from-slate-950 to-emerald-950 py-20">
   <div class="max-w-4xl mx-auto px-6">
    <div class="text-center mb-12">
      <span class="inline-block bg-red-500/20 text-red-400 px-4 py-2 rounded-full text-sm font-semibold mb-4 animate-pulse">🔥 OFERTA POR TEMPO LIMITADO</span>
      <h2 class="text-3xl md:text-5xl font-bold mb-4">Invista no seu <span class="gradient-text">futuro financeiro</span></h2>
    </div>

    <div class="bg-gradient-to-br from-slate-800 to-slate-900 rounded-3xl p-8 md:p-12 border-2 border-emerald-500/50 card-glow relative overflow-hidden">
     <div class="absolute top-6 right-6 bg-emerald-500 text-slate-900 font-bold px-4 py-1 rounded-full text-sm">MAIS VENDIDO</div>

     <div class="grid md:grid-cols-2 gap-8 items-center">
      <div>
       <h3 class="text-2xl font-bold mb-6">O que você recebe:</h3>
       <ul class="space-y-4">
        <li class="flex items-center gap-3 check-item" style="animation-delay: 0.1s;"><span class="w-6 h-6 bg-emerald-500 rounded-full flex items-center justify-center flex-shrink-0"><svg class="w-4 h-4 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7" /></svg></span><span>Planilha Mapa das Dívidas completa</span></li>
        <li class="flex items-center gap-3 check-item" style="animation-delay: 0.2s;"><span class="w-6 h-6 bg-emerald-500 rounded-full flex items-center justify-center flex-shrink-0"><svg class="w-4 h-4 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7" /></svg></span><span>Dashboard visual interativo</span></li>
        <li class="flex items-center gap-3 check-item" style="animation-delay: 0.3s;"><span class="w-6 h-6 bg-emerald-500 rounded-full flex items-center justify-center flex-shrink-0"><svg class="w-4 h-4 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7" /></svg></span><span>Calculadora de juros automática</span></li>
        <li class="flex items-center gap-3 check-item" style="animation-delay: 0.4s;"><span class="w-6 h-6 bg-emerald-500 rounded-full flex items-center justify-center flex-shrink-0"><svg class="w-4 h-4 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7" /></svg></span><span>Método Bola de Neve integrado</span></li>
        <li class="flex items-center gap-3 check-item" style="animation-delay: 0.5s;"><span class="w-6 h-6 bg-emerald-500 rounded-full flex items-center justify-center flex-shrink-0"><svg class="w-4 h-4 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7" /></svg></span><span>Vídeo tutorial de uso</span></li>
        <li class="flex items-center gap-3 check-item" style="animation-delay: 0.6s;"><span class="w-6 h-6 bg-emerald-500 rounded-full flex items-center justify-center flex-shrink-0"><svg class="w-4 h-4 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7" /></svg></span><span>Suporte por e-mail</span></li>
        <li class="flex items-center gap-3 check-item" style="animation-delay: 0.7s;"><span class="w-6 h-6 bg-emerald-500 rounded-full flex items-center justify-center flex-shrink-0"><svg class="w-4 h-4 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7" /></svg></span><span>Atualizações gratuitas</span></li>
       </ul>
      </div>

      <div class="text-center">
       <p class="text-slate-400 mb-2">De <span id="original-price" class="line-through text-red-400">R$ 67,00</span></p>
       <p class="text-slate-300 mb-1">Por apenas</p>
       <p class="text-6xl font-extrabold gradient-text mb-2" id="sale-price">R$ 27,00</p>
       <p class="text-emerald-400 mb-6">ou 6x de R$ 8,50</p>

       <button id="cta-button-pricing" class="w-full bg-emerald-500 hover:bg-emerald-400 text-slate-900 font-bold text-xl py-5 rounded-2xl transition-all duration-300 transform hover:scale-105 pulse-glow mb-4">
        QUERO MINHA PLANILHA AGORA
       </button>

       <div class="flex items-center justify-center gap-2 text-slate-400 text-sm">
        <svg class="w-5 h-5 text-emerald-500" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 15v2m-6 4h12a2 2 0 002-2v-6a2 2 0 00-2-2H6a2 2 0 00-2 2v6a2 2 0 002 2zm10-10V7a4 4 0 00-8 0v4h8z" /></svg>
        Pagamento 100% seguro
       </div>
      </div>
     </div>
    </div>
   </div>
  </section>

  <!-- Guarantee Section -->
  <section class="bg-emerald-950 py-16">
   <div class="max-w-4xl mx-auto px-6">
    <div class="bg-gradient-to-r from-emerald-900/50 to-slate-900/50 rounded-3xl p-8 md:p-12 border border-emerald-500/30 flex flex-col md:flex-row items-center gap-8">
     <div class="flex-shrink-0">
      <div class="w-32 h-32 bg-emerald-500/20 rounded-full flex items-center justify-center border-4 border-emerald-500">
       <svg class="w-16 h-16 text-emerald-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z" /></svg>
      </div>
     </div>
     <div>
      <h3 class="text-2xl md:text-3xl font-bold mb-4">Garantia incondicional de <span id="guarantee-days" class="text-emerald-400">7 dias</span></h3>
      <p class="text-slate-300 text-lg">Se por qualquer motivo você não ficar satisfeito com a planilha, basta enviar um e-mail em até 7 dias e devolvemos 100% do seu dinheiro. Sem perguntas, sem burocracia.</p>
     </div>
    </div>
   </div>
  </section>

  <!-- FAQ Section -->
  <section class="bg-slate-950 py-20">
   <div class="max-w-3xl mx-auto px-6">
    <h2 class="text-3xl md:text-4xl font-bold text-center mb-12">Perguntas <span class="gradient-text">Frequentes</span></h2>
    <div class="space-y-4" id="faq-container">
     <div class="faq-item bg-slate-800/50 rounded-2xl border border-slate-700/50 overflow-hidden">
      <button class="faq-trigger w-full p-6 text-left flex items-center justify-between" onclick="toggleFaq(this)">
       <span class="font-semibold text-lg">Funciona no Excel e Google Sheets?</span>
       <svg class="faq-icon w-6 h-6 text-emerald-400 transition-transform" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" /></svg>
      </button>
      <div class="faq-content px-6 pb-6 hidden"><p class="text-slate-400">Sim! A planilha é compatível com Microsoft Excel e Google Sheets. Você pode usar no computador, tablet ou celular.</p></div>
     </div>

     <div class="faq-item bg-slate-800/50 rounded-2xl border border-slate-700/50 overflow-hidden">
      <button class="faq-trigger w-full p-6 text-left flex items-center justify-between" onclick="toggleFaq(this)">
       <span class="font-semibold text-lg">Preciso saber usar planilhas?</span>
       <svg class="faq-icon w-6 h-6 text-emerald-400 transition-transform" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" /></svg>
      </button>
      <div class="faq-content px-6 pb-6 hidden"><p class="text-slate-400">Não! A planilha foi feita para ser simples. Você só precisa preencher os dados e ela faz todo o trabalho. Além disso, incluímos um vídeo tutorial completo.</p></div>
     </div>

     <div class="faq-item bg-slate-800/50 rounded-2xl border border-slate-700/50 overflow-hidden">
      <button class="faq-trigger w-full p-6 text-left flex items-center justify-between" onclick="toggleFaq(this)">
       <span class="font-semibold text-lg">Como recebo o produto?</span>
       <svg class="faq-icon w-6 h-6 text-emerald-400 transition-transform" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" /></svg>
      </button>
      <div class="faq-content px-6 pb-6 hidden"><p class="text-slate-400">Após a confirmação do pagamento, você recebe imediatamente por e-mail o link para download da planilha e acesso ao vídeo tutorial.</p></div>
     </div>

     <div class="faq-item bg-slate-800/50 rounded-2xl border border-slate-700/50 overflow-hidden">
      <button class="faq-trigger w-full p-6 text-left flex items-center justify-between" onclick="toggleFaq(this)">
       <span class="font-semibold text-lg">Posso usar em mais de um dispositivo?</span>
       <svg class="faq-icon w-6 h-6 text-emerald-400 transition-transform" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" /></svg>
      </button>
      <div class="faq-content px-6 pb-6 hidden"><p class="text-slate-400">Sim! A planilha é sua para sempre. Pode usar no computador, notebook, tablet e celular. Basta ter o Excel ou Google Sheets instalado.</p></div>
     </div>
    </div>
   </div>
  </section>

  <!-- Final CTA -->
  <section class="bg-gradient-to-b from-slate-950 to-emerald-950 py-20">
   <div class="max-w-4xl mx-auto px-6 text-center">
    <h2 class="text-3xl md:text-5xl font-bold mb-6">Está na hora de <span class="gradient-text">virar o jogo</span></h2>
    <p class="text-xl text-slate-300 mb-10 max-w-2xl mx-auto">Cada dia que passa sem organização é mais dinheiro jogado fora em juros. Comece agora sua jornada rumo à liberdade financeira.</p>
    <button id="cta-button-final" class="bg-emerald-500 hover:bg-emerald-400 text-slate-900 font-bold text-xl px-12 py-6 rounded-2xl transition-all duration-300 transform hover:scale-105 pulse-glow">
      QUERO SAIR DAS DÍVIDAS AGORA →
    </button>
    <p class="mt-6 text-slate-400"><span class="text-emerald-400">✓</span> Acesso imediato &nbsp; <span class="text-emerald-400">✓</span> Garantia de 7 dias &nbsp; <span class="text-emerald-400">✓</span> Suporte incluído</p>
   </div>
  </section>

  <!-- Footer -->
  <footer class="bg-slate-950 border-t border-slate-800 py-8">
   <div class="max-w-6xl mx-auto px-6 text-center">
    <p class="text-slate-500 text-sm">© 2024 Mapa das Dívidas. Todos os direitos reservados.</p>
    <p class="text-slate-600 text-xs mt-2">Este produto não garante resultados. Os resultados dependem do esforço individual de cada pessoa.</p>
   </div>
  </footer>

  <script>
    // FAQ Toggle
    function toggleFaq(button) {
      const content = button.nextElementSibling;
      const icon = button.querySelector('.faq-icon');
      const isHidden = content.classList.contains('hidden');

      document.querySelectorAll('.faq-content').forEach(c => c.classList.add('hidden'));
      document.querySelectorAll('.faq-icon').forEach(i => i.style.transform = 'rotate(0deg)');

      if (isHidden) {
        content.classList.remove('hidden');
        icon.style.transform = 'rotate(180deg)';
      }
    }

    // Animate check items on scroll
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => { if (entry.isIntersecting) entry.target.style.opacity = '1'; });
    }, { threshold: 0.1 });

    document.querySelectorAll('.check-item').forEach(item => observer.observe(item));

    // CTAs: hero scroll; pricing/final go checkout (edite o link)
    const CHECKOUT_URL = "https://pay.kiwify.com.br/d8fIcuO";

    function scrollToPricing() {
      const pricing = document.getElementById("pricing");
      if (pricing) pricing.scrollIntoView({ behavior: "smooth", block: "start" });
    }

    document.addEventListener("DOMContentLoaded", () => {
      const hero = document.getElementById("cta-button-hero");
      const pricing = document.getElementById("cta-button-pricing");
      const finalCta = document.getElementById("cta-button-final");

      if (hero) hero.addEventListener("click", scrollToPricing);
      if (pricing) pricing.addEventListener("click", () => window.location.href = CHECKOUT_URL);
      if (finalCta) finalCta.addEventListener("click", () => window.location.href = CHECKOUT_URL);
    });
  </script>
 </body>
</html>
