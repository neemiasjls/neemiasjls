## Projetos

### [DevConductor](https://github.com/neemiasjls/DevConductor-public)

Kit de plugins para o Claude Code que organiza o desenvolvimento com agentes de IA: decide **quem faz cada
tarefa, com qual modelo e com quais instruções**. Reúne skills e agentes abertos da comunidade (com origem e
licença de cada arquivo registradas) e acrescenta uma camada própria:

- **Agentes por função com roteamento de modelo:** planejamento, execução, revisão e arquitetura vão para o
  modelo mais forte; pesquisa e tarefas mecânicas, para os mais baratos.
- **Contexto sob medida:** um hook lê os arquivos do projeto (`.csproj`, `package.json`, `pom.xml`...) e liga
  só os plugins daquela stack.
- **Medição de uso:** soma tokens por sessão e por modelo, incluindo subagentes, para acompanhar o custo.
- **Segurança de skills:** toda skill nova passa por um verificador adaptado da Sentry antes de ser usada.
- **Memória e publicação:** retomada entre sessões e geração de vitrines públicas limpas, sem histórico.
- **Testes:** mais de 300 testes com `node --test` no GitHub Actions, em Linux e Windows, a cada envio.

`JavaScript` `Node.js` `Claude Code` `GitHub Actions`

### [Sistema de Gestão](https://github.com/neemiasjls/Sistema-de-Gestao-public)

Sistema web de gestão operacional e financeira de uma transportadora, desenvolvido por mim e em uso na
rotina da empresa. A vitrine pública usa dados fictícios.

- **Frontend** em React + TypeScript, instalável como PWA, com sessão e rotas por perfil (administrador e
  motorista).
- **API** em ASP.NET Core 8 com JWT, organizada em controllers REST e camada de serviços com as regras de
  negócio.
- **Leitura e geração de documentos:** XML de notas fiscais, PDF, planilhas e OCR; geração de `.xlsx` a
  partir de modelos.
- **Dados** em PostgreSQL com EF Core; site na Cloudflare Pages, API em Docker na Render e publicação
  automática a cada envio.

`C#` `.NET 8` `React` `TypeScript` `PostgreSQL` `Docker`

### [Connect Gamers](https://github.com/mariialbano/Connect_Gamers_React) · FIAP 2025

Rede social para gamers formarem squads, participarem de eventos e conversarem entre comunidades. O chat tem
moderação de conteúdo pela API da OpenAI. Projeto em equipe, em que fui
o maior contribuidor, e **vencedor na turma do desafio Palo Alto | Microsoft da FIAP**.

`React` `Node.js` `Express` `PostgreSQL` `OpenAI API` `Docker`

### [Gesture Switch](https://github.com/neemiasjls/gesture-switch)

Liga e desliga a luz da sala com gestos na frente da webcam. Um processo em **Python** usa OpenCV e o
MediaPipe Gesture Recognizer para encontrar os 21 pontos de cada mão, reconhecer palmas e punhos e contar os
dedos. O **Java** recebe só essas observações, confirma que o gesto ficou estável (para evitar acionamentos
acidentais), escolhe as teclas e envia o comando pela API REST do SmartThings. Há um modo de simulação para
testar sem acionar nada.

`Java` `Python` `OpenCV` `MediaPipe` `SmartThings API`

### [ReconForge](https://github.com/neemiasjls/ReconForge)

Ferramenta de reconhecimento e enumeração para pentest **em ambientes autorizados**, feita durante o curso de
Pentest da Desec. Usa só a biblioteca padrão do Python e orquestra ferramentas do Kali em três fases:

- **Passiva:** WHOIS e DNS (A, AAAA, MX, NS, TXT).
- **Varredura:** descoberta de hosts na rede e identificação de portas e serviços com Nmap.
- **Enumeração:** HTTP/HTTPS (títulos, headers, robots.txt), banners de FTP, SSH e e-mail, e
  compartilhamentos SMB.

Pede confirmação de autorização antes de qualquer varredura ativa, não faz exploração nem força bruta e gera
um resumo em Markdown, em português.

`Python` `Nmap` `Kali Linux`

### [VidaReal (HackGov)](https://github.com/mariialbano/HackGov) · FIAP

Plataforma GovTech de educação financeira e transparência para o cidadão, feita em grupo de cinco pessoas na
FIAP. Reúne abertura e acompanhamento de protocolos, simulação de inflação, metas financeiras, indicadores
municipais com dados abertos (IBGE e Banco Central), triagem de protocolos com classificador Naive Bayes,
chatbot com a API do Gemini e trilha de auditoria encadeada por hash.

`Java` `React` `Tailwind` `Gemini API`

<details>
<summary><b>Outros projetos</b></summary>

- [**NemyCookies**](https://github.com/neemiasjls/NemyCookies-public): site de pedidos e painel de gestão de um delivery de cookies, em uso no negócio (fiado, estoque, produção, custos e fidelidade). React · TypeScript · Supabase
- [**Payment API**](https://github.com/neemiasjls/payment-api): gateway de pagamentos em sandbox (autorização, captura, estorno) com Stripe Test Mode. C# · .NET
- [**SmartKey**](https://github.com/neemiasjls/SmartKey-API): chave digital temporária para hospedagens com assinatura ECDSA, válida só durante a estadia. Java
- [**Nemus**](https://github.com/neemiasjls/Nemus): finanças pessoais com partidas dobradas, orçamento por envelope e parcelamento de cartão. C# · React
- [**QR Code Manager**](https://github.com/neemiasjls/qrcode-manager-public): QR codes dinâmicos com painel, lotes e estatísticas. Next.js · Postgres
- [**Agenda**](https://github.com/neemiasjls/Agenda-public): agenda, clientes, financeiro e portal de agendamento para profissional autônoma. JavaScript · Cloudflare Workers · Supabase
- [**Supermarket Delivery**](https://github.com/neemiasjls/SuperMarketDelivery): delivery de supermercado full-stack com catálogo, carrinho e login JWT. TypeScript

</details>
