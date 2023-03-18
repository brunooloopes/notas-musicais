![logo_do_projeto](assets/logo.png){width="300", .center}
# Notas Musicais


## Como usar?

Você pode chamar as escalas via linha de comando. Por exemplo:

```bash
poetry run escalas
```

Retornando os graus e as notas correspondentes

```
┏━━━┳━━━━┳━━━━━┳━━━━┳━━━┳━━━━┳━━━━━┓
┃ I ┃ II ┃ III ┃ IV ┃ V ┃ VI ┃ VII ┃
┡━━━╇━━━━╇━━━━━╇━━━━╇━━━╇━━━━╇━━━━━┩
│ C │ D  │ E   │ F  │ G │ A  │ B   │
└───┴────┴─────┴────┴───┴────┴─────┘
```

### Alteração na escala

O primeiro parâmetro do CLI é a tônica da escala que deseja exibir. Desta forma, você pode alterar a escala retorna. Por exemplo, a escala de `F#` maior:

```
poetry run escalas F# maior
```

Resultado em:

```
┏━━━━┳━━━━┳━━━━━┳━━━━┳━━━━┳━━━━┳━━━━━┓
┃ I  ┃ II ┃ III ┃ IV ┃ V  ┃ VI ┃ VII ┃
┡━━━━╇━━━━╇━━━━━╇━━━━╇━━━━╇━━━━╇━━━━━┩
│ F# │ G# │ A#  │ B  │ C# │ D# │ F   │
└────┴────┴─────┴────┴────┴────┴─────┘
```

## Alteração na tonalidade da escala

Você pode alterar a tonalidade da escala também! Esse é o seu segundo parâmetro da linha de comando. Por exemplo, a escala de `D#` maior:

```
poetry run escalas D# maior

┏━━━━┳━━━━┳━━━━━┳━━━━┳━━━━┳━━━━┳━━━━━┓
┃ I  ┃ II ┃ III ┃ IV ┃ V  ┃ VI ┃ VII ┃
┡━━━━╇━━━━╇━━━━━╇━━━━╇━━━━╇━━━━╇━━━━━┩
│ D# │ F  │ G   │ G# │ A# │ C  │ D   │
└────┴────┴─────┴────┴────┴────┴─────┘
```

## Mais informações sobre o CLI

Para descobrir outras opções, você pode usar a flag `--help`:

```bash
poetry run escalas --help
                                                                                     
Usage: escalas [OPTIONS] [TONICA] [TONALIDADE]                                      
                                                                                     
╭─ Arguments ───────────────────────────────────────────────────────────────────────╮
│   tonica          [TONICA]      Tônica da escala [default: c]                     │
│   tonalidade      [TONALIDADE]  Tonlidade da escala [default: maior]              │
╰───────────────────────────────────────────────────────────────────────────────────╯
```
