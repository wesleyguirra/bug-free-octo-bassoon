# Planos de contratação
## Arquivos necessários
> Não é necessário incluir todos os arquivos css apenas o arquivo plano.css que está em components.

## Ícones
Para os ícones foi utilizado imagens, com exceção dos ícones da lista onde foi utilizado [Material icons](https://material.io/icons) já existe um plugin do material icons instalado no drupal, e logo antes do código do ícone tem um comentário com o nome dos ícones
```html
<i class="material-icons"><!-- done -->&#xE876;</i>
```

> A tag com a classe .planos é obrigatória, mas caso queira remove-la deve ser implementado na tag pai de .plano:

```css
@media screen and (min-width: 960px) {
    .tag-pai {
        white-space: nowrap; /* é necessário para manter as caixas de planos uma ao lado da outra */
    }
    .tag-pai .plano {
        display: inline-block;
        width: 50%;
    }
}
```