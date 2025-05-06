# 🦆 Pico Ducky (RP2040) — BadUSB compatível com teclado PT-BR

Este projeto transforma sua placa RP2040 (como o Raspberry Pi Pico) em um dispositivo **BadUSB**, que simula um teclado para executar comandos automaticamente em computadores com sistema configurado em **Português do Brasil** (PT-BR).

> 🔐 Use com responsabilidade. Este projeto é apenas para fins educacionais e testes de segurança autorizados.

---

## 🚀 Instalação

1. **Baixe o CircuitPython compatível com sua placa**  
   🔗 [https://circuitpython.org/downloads](https://circuitpython.org/downloads)

2. **Coloque a placa em modo bootloader**  
   Conecte ao computador segurando o botão **BOOTSEL** até que apareça uma unidade chamada `RPI-RP2`.

3. **Arraste o arquivo `.UF2` baixado para essa unidade**  
   Isso instalará o CircuitPython. Após reiniciar, a placa será exibida como uma nova unidade chamada `CIRCUITPY`.

4. **Copie os arquivos do repositório para a placa**  
   Baixe este repositório e copie **todos os arquivos** para dentro da unidade `CIRCUITPY`.

---

## 📝 Modificando o Payload

- O script que será executado automaticamente está no arquivo:  
  `payload.dd`

- Para mudar o comportamento do BadUSB, edite este arquivo com os comandos desejados (Duckyscript adaptado para PT-BR).

---

## 📄 Exemplo de Payload

```text
DELAY 1000
GUI r
DELAY 500
STRING notepad
ENTER
DELAY 500
STRING Olá! Isso é um teste automatizado.
ENTER
```
📚 Créditos
Este projeto é uma modificação do repositório original:
🔗 [https://github.com/dbisu/pico-ducky](https://github.com/dbisu/pico-ducky)

Modificações realizadas para compatibilidade com o layout de teclado em Português (Brasil).
