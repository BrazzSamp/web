---
título: PlayerPlaySound
descrição: Toca o som especificado para um jogador.
tags: ["player"]
---

## descrição

Toca o som especificado para um jogador.

Para obter uma biblioteca que lista todos os sons, verifique [this](https://github.com/WoutProvost/samp-sound-array).

| Name     | Description                                                  |
| -------- | ------------------------------------------------------------ |
| playerid | O ID do jogador para quem tocar o som                        |
| soundid  | O som a ser reproduzido.                                     |
| Float:x  | Coordenada X para o som a ser reproduzido.                   |
| Float:y  | Coordenada X para o som a ser reproduzido.                   |
| Float:z  | Coordenada X para o som a ser reproduzido.                   |  

## Retornos

1: A função foi executada com sucesso.

0: A função falhou ao executar. Isso significa que o reprodutor não está conectado.
## Exemplos

```c
// psom de soco do jogador (adequado para comandos como /tapa). O som será baixo, pois a fonte está, na verdade, 10 metros acima do reprodutor.
PlayerPlaySound(playerid, 1130, 0.0, 0.0, 10.0);
```

## Notas

:::tip

Use as coordenadas apenas se quiser que o som seja reproduzido em uma determinada posição. Defina todas as coordenadas como 0,0 para apenas reproduzir o som.

:::

## Related Functions

- [PlayCrimeReportForPlayer](PlayCrimeReportForPlayer): Apresentar um relatório de crime para um jogador.
- [PlayAudioStreamForPlayer](PlayAudioStreamForPlayer): Reproduz um fluxo de áudio para um jogador.
- [StopAudioStreamForPlayer](StopAudioStreamForPlayer): Interrompe o fluxo de áudio atual para um jogador.
