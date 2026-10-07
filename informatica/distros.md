# Guia das Principais Distribuições Linux

As distribuições Linux organizam-se habitualmente por famílias de origem (bases de código e arquitetura de gestão de pacotes), pelo ciclo de desenvolvimento e pelo nível de experiência pretendido para o utilizador.

* * *

## 1. Família Debian / Ubuntu

### Debian

* **Foco:** Estabilidade estrita, segurança e compromisso com o software livre.
* **Gestor de Pacotes:** `apt` (ficheiros `.deb`).
* **Ciclo de Lançamento:** Fixo a cada ~2 anos, precedido de períodos longos de testes e congelamento.
* **Características:**
  * Conhecido como a "distribuição universal", serve de fundação para dezenas de outros projetos (incluindo o Ubuntu).
  * Prioriza a estabilidade a longo prazo face a versões recentes de programas, sendo a escolha de referência para servidores de produção e equipamentos críticos.
  * Política estrita de separação entre componentes livres e pacotes proprietários.

### Ubuntu

* **Foco:** Facilidade de utilização, ampla compatibilidade e adoção empresarial/nuvem.
* **Gestor de Pacotes:** `apt` (`.deb`) e `snap`.
* **Ciclo de Lançamento:** A cada 6 meses, com versões **LTS** (*Long Term Support*) a cada 2 anos (5 a 10 anos de suporte).
* **Características:**
  * Desenvolvido e mantido pela Canonical.
  * Ambiente padrão GNOME com modificações de usabilidade (barra lateral e painéis integrados).
  * Excelente suporte a hardware recente, drivers proprietários e vasta biblioteca de software documentado.

### Linux Mint

* **Foco:** Facilidade de transição e usabilidade direta para quem vem de sistemas Windows.
* **Gestor de Pacotes:** `apt` (`.deb`) e suporte nativo a `flatpak`.
* **Ciclo de Lançamento:** Baseado nas versões estáveis Ubuntu LTS.
* **Características:**
  * Destaca-se pelo ambiente de trabalho **Cinnamon**, que mantém a disposição tradicional de barra de tarefas inferior, menu de aplicações e tabuleiro de sistema.
  * Inclui codecs multimédia e utilitários pré-configurados prontos a usar.
  * Rejeita o ecossistema Snap da Canonical por omissão, dando primazia ao Flatpak.

### Pop!_OS

* **Foco:** Produtividade técnica, computação científica, desenvolvimento e videojogos.
* **Gestor de Pacotes:** `apt` (`.deb`) e `flatpak`.
* **Ciclo de Lançamento:** Alinhado com as versões do Ubuntu.
* **Características:**
  * Criado pela System76 para os seus próprios computadores, mas livre para qualquer máquina.
  * Disponibiliza imagens ISO distintas com controladores NVIDIA já integrados.
  * Ambiente de trabalho **COSMIC** (construído em Rust) com gestão nativa de janelas em mosaico (*auto-tiling*) e perfis avançados de poupança/desempenho energético para portáteis.

* * *

## 2. Família Red Hat / Fedora

### Fedora

* **Foco:** Inovação técnica, adocão de tecnologias de ponta e fidelidade ao código original (*upstream*).
* **Gestor de Pacotes:** `dnf` (ficheiros `.rpm`) e `flatpak`.
* **Ciclo de Lançamento:** Rápido, com novas versões aproximadamente a cada 6 meses.
* **Características:**
  * Patrocinado pela Red Hat, funciona como polo de teste e inovação das tecnologias que mais tarde chegam ao meio corporativo (ex.: pioneiro na adoção de Wayland, PipeWire, Btrfs e cgroups v2).
  * Apresenta uma das implementações mais limpas e originais do ambiente GNOME.
  * Muito popular entre programadores e engenheiros de software.

### Red Hat Enterprise Linux (RHEL) / AlmaLinux / Rocky Linux

* **Foco:** Centros de dados, infraestruturas corporativas e missões empresariais de larga escala.
* **Gestor de Pacotes:** `dnf` (`.rpm`).
* **Ciclo de Lançamento:** Longo e altamente estável (ciclos de vida de 10 anos).
* **Características:**
  * O **RHEL** é o padrão corporativo pago com certificações de hardware e suporte comercial.
  * **Rocky Linux** e **AlmaLinux** são distribuições comunitárias binariamente compatíveis criadas para substituir o ecossistema do antigo CentOS estável, proporcionando a mesma estabilidade sem custos de licença.

* * *

## 3. Família Arch

### Arch Linux

* **Foco:** Simplicidade interna (princípio *KISS* - *Keep It Simple, Stupid*), controlo manual e personalização.
* **Gestor de Pacotes:** `pacman`.
* **Ciclo de Lançamento:** *Rolling Release* (atualização contínua; sem novas versões periódicas de reinstalação).
* **Características:**
  * O utilizador constrói o sistema de raiz através de linha de comandos, selecionando estritamente os componentes necessários.
  * Software disponibilizado praticamente sem alterações em relação aos programadores originais.
  * Acesso ao **AUR** (*Arch User Repository*), um vasto repositório colaborativo gerido pela comunidade.
  * Dispõe da **ArchWiki**, considerada uma das melhores bases de documentação técnica do ecossistema informático.

### Manjaro

* **Foco:** Acessibilidade ao ecossistema Arch para utilizadores que preferem configuração gráfica.
* **Gestor de Pacotes:** `pacman` e interface gráfica `Pamac`.
* **Ciclo de Lançamento:** *Curated Rolling Release*.
* **Características:**
  * Instalador gráfico amigável e deteção automática de hardware (controladores de vídeo, placas Wi-Fi, etc.).
  * Testa os pacotes do Arch durante breves semanas antes de os distribuir, reduzindo potenciais quebras de compatibilidade em atualizações.

* * *

## 4. Família openSUSE

### openSUSE (Tumbleweed e Leap)

* **Foco:** Ambientes de trabalho avançados, desenvolvimento e administração de sistemas.
* **Gestor de Pacotes:** `zypper` (ficheiros `.rpm`).
* **Ciclos de Lançamento:**
  * **Tumbleweed:** *Rolling release*, continuamente atualizado e validado através da ferramenta de testes automatizados **openQA**.
  * **Leap:** Versão com ciclo regular e base de código partilhada com o SUSE Linux Enterprise (SLE).
* **Características:**
  * Incorpora o **YaST** (*Yet another Setup Tool*), uma das ferramentas de gestão e configuração centralizada mais completas do ecossistema Linux (gestão de rede, partições, serviços e utilizadores).
  * Integração nativa e avançada com o sistema de ficheiros **Btrfs**, permitindo recuperar o sistema facilmente em caso de problemas através de instantâneos automáticos (*snapshots* via Snapper).

* * *

## Quadro Comparativo

| Distribuição | Base | Formato de Pacotes | Ciclo de Atualização | Nível de Perfil | Melhor Caso de Uso |
| --- | --- | --- | --- | --- | --- |
| **Linux Mint** | Ubuntu | `.deb` / Flatpak | Fixo (LTS) | Iniciante | Utilizadores quotidianos vindos do Windows |
| **Ubuntu** | Debian | `.deb` / Snap | Fixo (6m / LTS) | Iniciante / Intermédio | Uso geral, compatibilidade de drivers e cloud |
| **Pop!_OS** | Ubuntu | `.deb` / Flatpak | Fixo (LTS) | Iniciante / Intermédio | Portáteis com GPU híbrida e videojogos |
| **Fedora** | Independente | `.rpm` / Flatpak | Fixo (~6 meses) | Intermédio | Programadores e entusiastas de novidades |
| **Debian** | Independente | `.deb` | Fixo (~2 anos) | Intermédio / Avançado | Servidores, estabilidade absoluta e IoT |
| **Arch Linux** | Independente | `pacman` / AUR | *Rolling Release* | Avançado | Controlo total, aprendizagem e personalização |
| **Manjaro** | Arch | `pacman` / Pamac | *Curated Rolling* | Intermédio | Acesso fácil ao AUR e pacotes recentes |
| **openSUSE** | Independente | `.rpm` (Zypper) | Rolling / Fixo | Intermédio / Avançado | Ferramentas administrativas (YaST) e Btrfs |
