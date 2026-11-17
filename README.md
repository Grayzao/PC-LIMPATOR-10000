<div align="center">
  <img src="./logo.png" alt="PC LIMPATOR 10.000 Logo" width="160" />

  <h1>PC LIMPATOR 10.000</h1>
  <p>
    <strong>Suite Profissional de Manutenção, Otimização, Pós-Formatação e Diagnóstico Avançado para Windows</strong>
  </p>

  <p>
    <img src="https://img.shields.io/badge/Windows-10%20%2F%2011-0078D6?style=for-the-badge&logo=windows&logoColor=white" alt="Windows 10/11" />
    <img src="https://img.shields.io/badge/Interface-.NET%20WPF%20Dark%20Pro-161821?style=for-the-badge&logo=dotnet&logoColor=white" alt="WPF Dark UI" />
    <img src="https://img.shields.io/badge/Motor-PowerShell%20%2B%20C%23%20Nativo-22C55E?style=for-the-badge" alt="Motor Nativo" />
    <img src="https://img.shields.io/badge/Elevação-Admin%20UAC-EF4444?style=for-the-badge" alt="Admin UAC" />
    <img src="https://img.shields.io/badge/Versão-1.0.1-10B981?style=for-the-badge" alt="Versão 1.0.1" />
  </p>
</div>

---

## Visão Executiva

O **PC LIMPATOR 10.000** é uma ferramenta completa e autônoma para Windows 10 e Windows 11, projetada para reunir em um único executável portátil (**`PC LIMPATOR 10.000.exe`**) todo o ciclo de manutenção preventiva, aceleração de desempenho, automação pós-formatação, atualização universal de sistema/programas e diagnóstico técnico de hardware.

Com interface gráfica **Dark Pro** em `.NET WPF`, elevação automática de privilégios via UAC e execução assíncrona com logs coloridos em tempo real, o aplicativo elimina scripts manuais complexos e entrega resultados seguros, auditáveis e de nível profissional com poucos cliques.

---

## Idealizador e Criador do Projeto

<table>
  <tr>
    <td width="90" align="center">
      <img src="./logo.png" width="64" alt="Gray Emblem" />
    </td>
    <td>
      <strong>Idealizador e Criador:</strong> <strong>Gray</strong><br />
      <strong>Contato:</strong> <a href="mailto:jonasbrandx@gmail.com">jonasbrandx@gmail.com</a><br />
      <strong>Missão do Projeto:</strong> Oferecer uma ferramenta confiável, rápida, segura e sem complicações para manutenção, otimização, pós-formatação e diagnóstico de PCs Windows — unindo automação inteligente, transparência total das ações executadas e uma experiência visual moderna e intuitiva.
    </td>
  </tr>
</table>

---

## Interface Gráfica Profissional (Dark UI)

A interface do **PC LIMPATOR 10.000** foi construída em **WPF (Windows Presentation Foundation)** com foco em legibilidade, resposta instantânea e controle total do usuário:

- **Estética Dark Pro:** Fundo preto fosco profundo (`#0A0A0D` / `#0F1015`), superfícies e bordas em cinza sutil (`#161821` / `#1E202B` / `#2A2D3A`) e tipografia limpa (`Segoe UI`).
- **Dashboard de Telemetria de Hardware em Tempo Real:** Exibição automática na tela inicial de **CPU**, **Memória RAM** (uso e capacidade total), **Armazenamento (SSD/HDD)** com espaço livre/usado, **GPU (Placa de Vídeo)** e **Status de Drivers**, além de detecção automática de Notebook/Desktop e plano de energia ativo.
- **Cartões de Status Visuais (Verde / Vermelho):** Todas as etapas e opções selecionáveis utilizam código visual imediato e inequívoco:
  - **Verde (`[ATIVO / MARCADO]`)** — Opção selecionada e pronta para execução.
  - **Vermelho (`[DESMARCADO]`)** — Opção desativada, ignorada com segurança na execução.
  - Botões rápidos **"Marcar Todos"** e **"Desmarcar Todos"** para personalizar lotes em segundos.
- **Console e Progresso em Tempo Real:** Barra de progresso dinâmica e log detalhado com destaque por nível (`OK`, `INFO`, `WARN`, `ERR`) rodando em segundo plano sem travar a janela.
- **Navegação Instantânea e Segura:** Botão visível **"← Cancelar e voltar ao início"** (ou atalho **`ESC`**) em todas as telas de módulo para interromper seleções ou retornar imediatamente ao menu principal.

---

## Detalhamento Completo dos 4 Módulos

### Módulo 1 — Limpeza e Otimização

Executa uma manutenção profunda dividida em etapas inteligentes que preservam dados pessoais, senhas e favoritos:

1. **Limpeza de Resíduos e Caches:**
   - Temporários do Usuário (`%TEMP%`) e do Windows (`C:\Windows\Temp`).
   - Cache `Prefetch` antigo (> 7 dias, preservando o cache de inicialização recente).
   - Relatórios de erro do Windows (`WER Archive`, `WER Queue` e `WER` do usuário).
   - Despejos de memória (`CrashDumps` do usuário e `Minidump` do sistema).
   - Cache de downloads do **Windows Update** (`SoftwareDistribution\Download`) com pausa/retomada segura de serviços.
   - Cache de **Otimização de Entrega** (`Delivery Optimization`).
   - Cache de miniaturas do Explorer (`thumbcache_*.db`) e cache de shaders DirectX (`D3DSCache`).
   - Caches de navegadores (**Google Chrome**, **Microsoft Edge**, **Brave**, **Vivaldi**, **Opera GX** e **Mozilla Firefox**) — **preservando senhas, histórico, cookies e favoritos**.
   - Esvaziamento da Lixeira e limpeza de cache DNS (`Flush DNS`).
2. **Atualização Automática de Drivers:**
   - Varredura de dispositivos Plug and Play via `pnputil.exe /scan-devices` e busca/instalação de drivers ausentes ou desatualizados via **Windows Update**.
3. **Otimizações Avançadas de Desempenho, Rede e Sistema:**
   - Criação de **Ponto de Restauração do Sistema** antes das alterações.
   - **Sysinternals RAMMap (`Empty Working Sets`)**: Baixa e executa o utilitário oficial da Microsoft (`RAMMap64.exe -Ew -accepteula`) de forma silenciosa em segundo plano, liberando memória física em uso imediatamente.
   - **TRIM (SSD)** ou **Desfragmentação (HDD)** conforme detecção automática da mídia do disco do sistema.
   - Limpeza profunda de componentes WinSxS (`DISM /StartComponentCleanup`).
   - Ajuste de efeitos visuais para melhor desempenho e revisão de programas de inicialização no Gerenciador de Tarefas.
   - Ativação do plano de energia **Alto Desempenho / Desempenho Máximo** e desativação opcional da hibernação (`hiberfil.sys`) para liberar espaço em disco.
   - Otimização da pilha de rede (`Flush DNS`, reset de catálogo Winsock e ajuste de `TCP Auto-Tuning`).
   - **Debloat nativo embutido** (100% PowerShell, sem baixar scripts externos), ajustes de **Privacidade** (remoção de telemetria `DiagTrack`, ID de publicidade e sugestões), **Personalização** (Modo Escuro, extensões de arquivo visíveis, barra de tarefas limpa) e reparo de integridade com **`DISM /RestoreHealth`** + **`sfc /scannow`**.

---

### Módulo 2 — PC Recém-Formatado (Automático)

Automatiza por completo a preparação de um Windows recém-instalado do zero:

- **Debloat Inicial Nativo (embutido):** Remove aplicativos pré-instalados desnecessários (Clipchamp, Cortana, Bing News/Weather/Finance/Sports/Search, Dicas, Office Hub, Solitaire, People, Power Automate, To Do, Feedback Hub, Mapas, Filmes e TV, Outlook novo, Dev Home e Copilot) e desativa Bing/sugestões/conteúdo patrocinado no Iniciar — sem downloads externos e sem erros de "Acesso negado". Microsoft Store, Terminal, Calculadora, Fotos, Xbox e Spotify são preservados.
- **Todos os Runtimes Essenciais:** Instala automaticamente bibliotecas **Visual C++ Redistributable (2005 a 2022, x86/x64)**, **.NET Desktop Runtime (6, 8, 9 e 10)**, **.NET Framework 3.5 e 4.8**, **DirectX**, **XNA Framework** e **Java JRE**.
- **Programas do Dia a Dia (via `winget`):** Instalação silenciosa e personalizável de **Google Chrome**, **Discord**, **Steam**, **7-Zip**, **WinRAR**, **VLC Player** e **Spotify**.
- **Detecção Automática de GPU por Vendor ID PCI:** Identifica placas **NVIDIA** (`VEN_10DE`), **AMD** (`VEN_1002`) ou **Intel** (`VEN_8086`), instala drivers via Windows Update e baixa/instala o aplicativo oficial do fabricante (**NVIDIA App**, **AMD Software: Adrenalin Edition** ou **Intel Driver & Support Assistant**).
- **Privacidade & Personalização:** Desativa telemetria/anúncios, ativa Modo Escuro, exibe extensões de arquivo e limpa a barra de tarefas.
- **Windows Update Completo com Retomada Pós-Reinício:** Instala atualizações cumulativas e drivers, agenda retomada automática após reinicialização via Tarefa Agendada (`CleanPCCarla`) e executa até **5 rodadas** até deixar o sistema 100% atualizado, finalizando com `RAMMap`, atualização de apps e Relatório de Saúde.

---

### Módulo 3 — Atualizar Tudo

Mantém o computador atualizado em uma única execução:

- Varredura de hardware e dispositivos via `pnputil`.
- Busca e instalação completa de atualizações de sistema, segurança e drivers pelo **Windows Update**.
- Atualização silenciosa em lote de todos os programas instalados via **`winget upgrade --all`**.

---

### Módulo 4 — Relatório de Saúde do PC

Realiza um diagnóstico técnico completo do equipamento e exporta os relatórios automaticamente para a **Área de Trabalho**:

- **`Relatorio Saude PC.txt`:** Resumo do sistema (SO, Build, CPU, RAM, GPU e versão do driver), saúde **S.M.A.R.T.** dos discos físicos (status, temperatura, desgaste de SSD em `%`, horas ligado e erros de leitura não corrigidos), sensores térmicos **ACPI** e auditoria de drivers/dispositivos com código de erro.
- **`Relatorio Bateria.html`:** Gerado automaticamente em notebooks com capacidade de projeto vs. capacidade atual carregada (`mWh`), porcentagem de vida útil da bateria e relatório detalhado via `powercfg /batteryreport`.

---

## Como Usar

1. Acesse a pasta [`Executavel/`](./Executavel) ou a seção **Releases** do repositório e baixe o arquivo **`PC LIMPATOR 10.000.exe`** (ou **`PCLimpator10000.exe`**).
2. Clique com o botão direito sobre o executável e selecione **"Executar como administrador"** *(ou dê duplo clique — o aplicativo solicitará elevação automática via UAC)*.
3. Na tela inicial, confira a telemetria do seu computador e escolha um dos **4 Módulos**.
4. Nos módulos com seleção personalizada, clique nos cartões para alternar entre **Verde (Ativo)** e **Vermelho (Desmarcado)** ou utilize **Marcar Todos / Desmarcar Todos**.
5. Acompanhe o progresso e os logs ao vivo no painel inferior. A qualquer momento, pressione **`ESC`** ou clique em **"← Cancelar e voltar ao início"** para retornar à tela inicial.

---

## Estrutura de Distribuição

```text
PC LIMPATOR 10000/
├── Executavel/
│   ├── PC LIMPATOR 10.000.exe   # Executável principal (GUI WPF + Motor embarcado)
│   └── PCLimpator10000.exe      # Alias sem espaços para automação/linha de comando
├── logo.png                     # Emblema oficial do projeto
└── README.md                    # Documentação oficial
```

> **Requisitos:** Windows 10 ou Windows 11 (x64), privilégios de Administrador e conexão com a internet para etapas de drivers, `winget`, `RAMMap` e Windows Update.

---

## Histórico de Versões

- **v1.0.1** — Debloat agora é **100% nativo** (remoção segura de Appx + pacotes provisionados com tratamento individual de erros e ajustes de registro), sem baixar o script externo Win11Debloat e sem o erro de **Acesso negado**.
- **v1.0.0** — Lançamento inicial do PC LIMPATOR 10.000.
