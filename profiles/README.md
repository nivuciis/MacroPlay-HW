# Perfis

Cada perfil é um arquivo JSON com nome, cor, as 12 teclas e as 3 ações do encoder.

```json
{
  "nome": "Blender",
  "cor": "#F5792A",
  "teclas": {
    "1": { "rotulo": "Frente", "on_press": [{ "tipo": "tecla", "teclas": ["KEYPAD_ONE"] }], "on_release": [] }
  },
  "encoder": {
    "horario":      [{ "tipo": "tecla", "teclas": ["RIGHT_ARROW"] }],
    "anti_horario": [{ "tipo": "tecla", "teclas": ["LEFT_ARROW"] }],
    "clique":       [{ "tipo": "tecla", "teclas": ["SPACE"] }]
  }
}
```

O formato definitivo será fixado ao fim da Fase 1 do roadmap. Até lá, ele pode mudar.

## Regras para perfis de jogos online

Uma tecla, uma ação. Nada de sequências automáticas, repetição ou atrasos em perfis marcados como jogo online.
