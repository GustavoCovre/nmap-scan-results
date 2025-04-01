# Nmap Scan Results

Este repositório contém os resultados de um escaneamento de rede realizado com a ferramenta **Nmap** na minha rede local. O objetivo deste escaneamento foi verificar as portas abertas e tentar identificar o sistema operacional de um dispositivo específico.

## Descrição

O escaneamento foi realizado em um dispositivo da minha rede local com o IP **192.168.1.8**. O Nmap foi usado para detectar as versões dos serviços em execução e tentar identificar o sistema operacional.

O escaneamento não encontrou portas abertas e a identificação do sistema operacional não foi possível devido a muitas correspondências de "fingerprints".

### Comando utilizado

O comando utilizado para realizar o escaneamento foi o seguinte:

```bash
nmap -sV -O -oN resultado_nmap.txt 192.168.1.8

    -sV: Detectar versões dos serviços.

    -O: Tentar identificar o sistema operacional.

    -oN: Salvar o resultado no arquivo resultado_nmap.txt.

Resultados

    Host: G-Linux (192.168.1.8)

    Status do Host: Ativo (0.000027 segundos de latência)

    Portas verificadas: 1000 portas (todas fechadas ou ignoradas)

    Sistema Operacional: Não identificado devido a múltiplas correspondências de fingerprints

    Tempo total de escaneamento: 1.60 segundos

Como rodar o escaneamento

Para rodar um escaneamento similar na sua própria rede, você pode usar o seguinte comando (modificando o IP conforme necessário):

nmap -sV -O -oN resultado_nmap.txt <IP_DO_SEU_DISPOSITIVO>

Certifique-se de ter o Nmap instalado na sua máquina. Se não tiver, você pode instalar com o comando:

sudo apt install nmap   # Para sistemas baseados em Debian/Ubuntu

Dicas de segurança

    Certifique-se de que as portas abertas na sua rede estão devidamente protegidas e configuradas.

    Utilize firewalls para bloquear acessos não autorizados.

    Faça escaneamentos periódicos na sua rede para identificar possíveis vulnerabilidades.

Licença

Este repositório é para fins educacionais e de demonstração. Não há nenhuma licença específica, então, use-o por sua conta e risco.
