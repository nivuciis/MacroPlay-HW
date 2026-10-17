# MacroPlay

Teclado de macros aberto com 12 teclas, LED RGB em cada tecla, encoder rotativo e buzzer, baseado em um devkit RP2040 com 16 MB de flash. Funciona com CircuitPython e é configurado por uma página HTML que fica dentro do próprio teclado, sem instalar nenhum programa.

O MacroPlay é pensado para três públicos: quem quer atalhos prontos para os programas que usa, quem programa e quer automações próprias, e pessoas com deficiência motora ou visual que precisam de um teclado adaptável.

## O que ele faz

| Recurso | Para quê |
| --- | --- |
| Teclado, mouse e teclas de mídia (USB HID) | Atalhos, textos prontos, volume, controle do cursor |
| Gamepad HID | Controle para emuladores e jogos |
| USB MIDI | Controlador musical: as 12 teclas formam uma oitava |
| Serial USB | Comunicação com a página de configuração e com scripts no PC |
| 12 LEDs RGB | Cor por tecla, perfil ativo e estados |
| Buzzer (ativo) | Confirmações sonoras por ritmo e duração dos bipes |
| Encoder | Volume, zoom, linha do tempo, troca de perfil |

## Estrutura do repositório

| Pasta | Conteúdo |
| --- | --- |
| [`hardware/`](hardware/) | Esquemático, PCB, BoM e arquivos de fabricação |
| [`firmware/`](firmware/) | `code.py`, `boot.py` e bibliotecas do CircuitPython |
| [`web/`](web/) | Página HTML de configuração |
| [`profiles/`](profiles/) | Perfis prontos em JSON para programas e jogos |
| [`3d/`](3d/) | Case, colmeia de acessibilidade e keycaps táteis |
| [`docs/`](docs/) | Site do projeto (GitHub Pages) e relatórios de teste |

## Começando

1. Instale o CircuitPython na placa (segure BOOT, conecte o USB e arraste o arquivo `.uf2` para a unidade `RPI-RP2`).
2. Baixe a versão mais recente em **Releases** e copie o conteúdo de `firmware/` e `web/` para a unidade `CIRCUITPY`.
3. Abra a página de configuração que aparece na unidade e escolha um perfil ou configure cada tecla.

## Roadmap

O desenvolvimento está dividido em quatro fases, cada uma com um milestone e as issues correspondentes:

1. **Base da plataforma:** formato dos perfis em JSON, modo simples e avançado, layout ABNT2, modo competitivo.
2. **Perfis prontos:** Altium, Blender, Fusion 360, jogos, reuniões, OBS e jogos no próprio teclado.
3. **Acessibilidade e música:** teclas de aderência, filtro de tremor, integração com NVDA, MIDI.
4. **Navegador, IA e comunidade:** emulador no navegador, configurador com IA e galeria de perfis.

Acompanhe o andamento na aba **Milestones** e no quadro em **Projects**.

## Contribuindo

Ideias, perfis novos e resultados de teste são bem-vindos. Abra uma issue usando um dos modelos (**Ideia** ou **Resultado de teste**). Perfis novos entram como pull request na pasta `profiles/`.

Em jogos online, os perfis seguem a regra **uma tecla, uma ação**. Perfis com sequências automáticas ou repetição não são aceitos para jogos competitivos, porque podem causar banimento.

## Licenças

- Hardware (`hardware/`, `3d/`): [CERN-OHL-S v2](LICENSE-HARDWARE)
- Firmware, página web, perfis e documentação: [MIT](LICENSE)
