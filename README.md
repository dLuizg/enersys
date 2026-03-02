Com certeza. Aqui está o conteúdo formatado em Markdown, pronto para ser copiado e colado diretamente no seu arquivo `README.md` na raiz do repositório do GitHub.

# SmartEdge IoT: Orquestrador de Redes Inteligentes com IA Generativa de Borda

!([https://img.shields.io/badge/Status-Em%20Desenvolvimento-green](https://www.google.com/search?q=https://img.shields.io/badge/Status-Em%2520Desenvolvimento-green))

## 📋 Sobre o Projeto

Este aplicativo é o resultado do **Projeto Integrado (PI)** do 1º Trimestre de 2026 do curso de **Ciência da Computação da UNIFEOB**. O objetivo central é fornecer uma interface de comunicação eficaz entre usuários e ecossistemas de **Internet das Coisas (IoT)**, utilizando Inteligência Artificial Generativa local (_Edge AI_) para orquestração de dispositivos.

O projeto foi concebido sob a premissa de atividade extensionista, focando em atender demandas de automação residencial e de pequenos comércios na cidade de **São João da Boa Vista/SP**, priorizando a privacidade do cidadão e a resiliência tecnológica.

## 🚀 Proposta de Valor: O Plano A (Edge AI)

Diferente das soluções tradicionais que dependem de nuvens proprietárias, nossa solução implementa o processamento de linguagem natural **on-device** para garantir latência mínima e segurança máxima.

### Principais Funcionalidades:

- **Controle por Intenção Natural:** O usuário comanda a rede com frases simples (ex: _"Prepare a sala para a reunião"_), e a IA traduz a intenção em múltiplos comandos MQTT simultâneos.
- **Privacidade por Design (Edge AI):** Utilização do modelo **Gemma 3n 2b** rodando localmente no smartphone via MediaPipe Tasks. Nenhum dado sensível de uso ou voz sai do dispositivo.
- **Resiliência Total:** Controle total de dispositivos via Wi-Fi local, funcionando mesmo em situações de queda da conexão com a internet externa.
- **Interface Adaptativa (GenUI):** Dashboards gerados dinamicamente pela IA conforme o contexto e a urgência das notificações da rede IoT.

## 🛠️ Stack Tecnológica

- **Framework:** [Flutter](https://flutter.dev/) (Multiplataforma)
- **Linguagem:** Dart
- **Inteligência Artificial:**
- Local: **Gemma 3n 2b** (quantizado em 4-bit/8-bit)
- Nuvem (Fallback): Gemini 2.5 Flash

- **Protocolo de Comunicação:** MQTT (via broker Mosquitto)
- **Arquitetura de Software:** MVVM (Model-View-ViewModel) com gerenciamento de estado via **Riverpod**.

## 📐 Metodologia: Design Sprint

O ciclo de desenvolvimento seguiu as etapas do **Design Sprint** para validação rápida de hipóteses:

1. **Entender:** Imersão nos desafios de infraestrutura e serviços em São João da Boa Vista.
2. **Definir:** Foco no problema da latência e falta de privacidade em soluções de IoT atuais.
3. **Sketch:** Ideação de uma interface conversacional pura e dinâmica.
4. **Decidir:** Seleção da arquitetura de IA de borda (Edge AI) como diferencial técnico.
5. **Prototipar:** Desenvolvimento iterativo em Flutter com integração ao broker MQTT local.
6. **Validar:** Testes de campo e medição do tempo de resposta da inferência local.

## 🧪 Estratégia de Testes Automatizados

Para atender aos requisitos de qualidade da UNIFEOB, o projeto implementa:

- **Testes Unitários:** Validação da lógica do agente orquestrador e parsing de intenções.
- **Testes de Widget:** Garantia de que as interfaces dinâmicas (GenUI) mantêm acessibilidade.
- **Mocking:** Simulação de estados de sensores e respostas de IA via `mockito` para garantir integridade no pipeline de CI/CD.

## 🌍 Objetivos de Desenvolvimento Sustentável (ODS)

Este projeto está alinhado à **Agenda 2030** da ONU:

- **ODS 9:** Indústria, Inovação e Infraestrutura.
- **ODS 11:** Cidades e Comunidades Sustentáveis (Eficiência energética via monitoramento).
- **ODS 12:** Consumo e Produção Responsáveis (Redução de desperdício em comércios locais).

## 📥 Como Rodar o Projeto

_(Instruções destinadas à banca avaliadora)_

1. Certifique-se de ter o **Flutter 3.x** estável instalado.
2. Configure um broker MQTT local (ou utilize o IP do servidor de teste da equipe).
3. Baixe o modelo Gemma 3n quantizado (`.task`) e coloque na pasta `assets/models/`.
4. Execute o comando para baixar as dependências:bash
   flutter pub get

```

```

5. Execute o projeto no emulador ou dispositivo físico:

```bash
flutter run

```

---

**Equipe UNIFEOB - Ciência da Computação:**

- Luiz Gustavo P. Diniz
- Eduardo Baldo
- Matteo Enrico Ferri Bonvento
- Nicolas Victoio Buciolli de Souza

**Orientadora:** Profª Mariangela Martimbianco Santos

---

_Este software é open-source sob a licença MIT._

```

Isto já inclui a estrutura de cabeçalhos, badges e o detalhamento técnico do **Plano A (Edge AI)** que desenvolvemos. Deixei os espaços para os nomes da equipe prontos para preenchimento. Esqueci de algo que você gostaria de incluir?

```
