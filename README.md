# Como configurar/instalar/usar o `btop` no `Linux Ubuntu`

## Resumo

Neste documento estão contidos os principais comandos e configurações para configurar/instalar/usar o `btop` no `Linux Ubuntu`.

## _Abstract_

_This document contains the main commands and settings to configure/install/use the `btop` on `Linux Ubuntu`._

## Descrição [1][2]

### `btop`

O `btop` é uma ferramenta de monitoramento de recursos de sistema para sistemas `Linux`, incluindo o Ubuntu. A sigla "btop" pode ser interpretada como `"Better TOP"`, uma referência ao comando `top` que também serve para monitorar a atividade do sistema em tempo real. O `btop` oferece uma visão geral do uso da CPU, memória, lista de processos e outros recursos do sistema de forma visual e interativa.

O `btop` é conhecido por seu layout amigável e fácil de usar, fornecendo informações de forma mais organizada e visualmente atraente em comparação com o comando `top`. Ele também permite que você interaja diretamente para matar processos, filtrar listas e muito mais, tudo diretamente da interface.

## 1. Configurar/Instalar o `btop` no `Linux Ubuntu` [1]

Para instalar o `btop` no `Linux Ubuntu`, você pode usar o gerenciador de pacotes `snap`. Siga os passos abaixo:

1. Abra o `Terminal Emulator`. Você pode fazer isso pressionando: `Ctrl + Alt + T`


2. Certifique-se de que seu sistema esteja limpo e atualizado.

    2.1 Limpar o `cache` do gerenciador de pacotes `apt`. Especificamente, ele remove todos os arquivos de pacotes (`.deb`) baixados pelo `apt` e armazenados em `/var/cache/apt/archives/`. Digite o seguinte comando: `sudo apt clean` 
    
    2.2 Remover pacotes `.deb` antigos ou duplicados do cache local. É útil para liberar espaço, pois remove apenas os pacotes que não podem mais ser baixados (ou seja, versões antigas de pacotes que foram atualizados). Digite o seguinte comando: `sudo apt autoclean`

    2.3 Remover pacotes que foram automaticamente instalados para satisfazer as dependências de outros pacotes e que não são mais necessários. Digite o seguinte comando: `sudo apt autoremove -y`

    2.4 Buscar as atualizações disponíveis para os pacotes que estão instalados em seu sistema. Digite o seguinte comando e pressione `Enter`: `sudo apt update`

    2.5 **Corrigir pacotes quebrados**: Isso atualizará a lista de pacotes disponíveis e tentará corrigir pacotes quebrados ou com dependências ausentes: `sudo apt --fix-broken install`

    2.6 Limpar o `cache` do gerenciador de pacotes `apt`. Especificamente, ele remove todos os arquivos de pacotes (`.deb`) baixados pelo `apt` e armazenados em `/var/cache/apt/archives/`. Digite o seguinte comando: `sudo apt clean` 
    
    2.7 Para ver a lista de pacotes a serem atualizados, digite o seguinte comando e pressione `Enter`:  `sudo apt list --upgradable`

    2.8 Realmente atualizar os pacotes instalados para as suas versões mais recentes, com base na última vez que você executou `sudo apt update`. Digite o seguinte comando e pressione `Enter`: `sudo apt full-upgrade -y`
   

3. **Instalar via Snap:** `sudo snap install btop`

4. Depois de instalado, você pode executá-lo simplesmente digitando btop no terminal: `btop`

Isso abrirá a interface do btop, onde você pode monitorar e gerenciar os recursos do sistema.


## 2. Código completo para configurar/instalar

Para instalar o `btop` no `Linux Ubuntu` sem precisar digitar linha por linha, você pode seguir estas etapas:

1. Abra o `Terminal Emulator`. Você pode fazer isso pressionando: `Ctrl + Alt + T`

2. Digite o seguinte comando e pressione `Enter`:

    ```
    sudo apt clean                                                            
    sudo apt autoclean
    sudo apt autoremove -y
    sudo apt update
    sudo apt --fix-broken install
    sudo apt clean
    sudo apt list --upgradable
    sudo apt full-upgrade -y
    sudo snap install btop
    btop
    ```

## Referências

[1] OPENAI. ***O que é o btop?.*** Disponível em: <https://chat.openai.com/c/35bba29e-8c34-40e1-9db1-3369f3c5c476> (texto adaptado). ChatGPT. Acessado em: 25/10/2023 13:08.

[2] OPENAI. ***Vs code: editor popular.*** Disponível em: <https://chat.openai.com/c/b640a25d-f8e3-4922-8a3b-ed74a2657e42> (texto adaptado). ChatGPT. Acessado em: 14/11/2023 09:33.
