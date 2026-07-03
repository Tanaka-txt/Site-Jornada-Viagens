# Site-Jornada-Viagens
Curso Responsividade Frontend React


```
Unidades de medida CSS

2 tipos de medina

- Fixa = Não se adaptam
  "px", "cm"
  * Rigida quebre, tipografias ilegíveis, experiencia comprometida

- Relativas = Podem se adapatar a algo
  "%", "em", "rem", "vh", "vw"

Proporções ao invés valores fixos
- "%" --> referente ao elemento PAI (larguras fluídas, margen, padding)
- "em" --> medidas gerlemnte de tipografica, relativa ao tamanho de font do elemento Pai (efeito cascata, acumula o tamanho de cada pae) [Pai(30px) * 1.5 = 45px]
- "rem" --> Mais usado em tipografias, relativo ao root do html (padroniza tipografia e espeçamentos)
[
  html {
    font-size: 16px;
  }
  div{
    width: 12.5rem; /* 12.5 * 16 = 200 */
  }
  div p {
    font-size: 1.5rem; /* 16 * 1.5 = 24px */
  }
]

- "vw" e "vh" (View width e View Heigth) --> Usados em banners fullscreen, slides, layouts hero (conteudo visivel antes do scroll) [Pode gerar rolagem extra em MOB!!!!]

ler CSS SECRET
```
---

# CSS Media Queries

Condições que aplicam estilos diferentes em telas diferentes

## Sintaxe:
**@** - indica um at-rule
**media** - significa que a regra vai depender de características da mídia
**screen** - tipo de midia (tela)
**and** - operador lógico, combina condições
**(max-width: 768px)** - condição de largura
**{}** - estilos aplicados na condição

```
@media screen and (max-width: 768px){ /*até 768px essas condições são aplicadas*/
  body{
    background: blue;
  }
}
```

---

# Conceito Importante Antes de iniciar hands-on! ==> Mobile First
-> Primeiro desenvolver pelo mobile

# Progressive Emhamcement --> Melhorias progressivamente 
---