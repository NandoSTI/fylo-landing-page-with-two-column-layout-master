# Frontend Mentor - Fylo landing page with two column layout

#### Fylo landing page with two column layout é um desafio do Frontend Mentor com layouts um pouco mais complexos. Esse projeto possui uma seção com área de depoimentos e validação de email com javascript. Obrigado por conferir meu código.

## Índice

- [Captura de tela](#captura-de-tela)
- [Links](#links)
- [Construído com](#construído-com)
- [O que aprendi](#o-que-aprendi)
- [Desenvolvimento contínuo](#desenvolvimento-contínuo)
- [Recursos úteis](#recursos-úteis)
- [Fernando Mendes](#autor)

### Captura de tela

#### Tela Desktop

<img src="./src/images/desktop.gif" alt="Tela desktop exibindo funcionalidades">

#### Tela Ipad

<img src="./src/images/ipad.gif" alt="Tela tablet exibindo funcionalidades">

#### Tela Mobile

<img src="./src/images/mobile.gif" alt="Exibindo responsividade no mobile">

### Links

- Site URL: https://nandosti.github.io/fylo-landing-page-with-two-column-layout-master/

### Construído com

<div style="display: inline_block"><br>
  <img align="center" alt="Js" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg">
  <img align="center" alt="HTML" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
  <img align="center" alt="CSS" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg">       
</div>

## O que aprendi

Nesse projeto envolvendo HTML,CSS e JS, aprendi conceitos importantes: selecionar elementos DOM; selecionar elementos HTML; evento de envio de formulário; evitar o comportamento padrão de envio de formulário; validação de email; uso de expressão regular de validação de email; conceitos de estilização e responsividade. Uma novidade nos meus projetos é o uso do conceito de "Mobile First".

## Trechos de códigos

```
const form = document.querySelector('form');
const email = document.getElementById('email');
const textError = document.querySelector('.text-error');

form.addEventListener('submit', (e) => {
    e.preventDefault();
    let emailValue = email.value;
    if(validateEmail(emailValue)) {
        textError.classList.remove('block');
        email.value = '';
    }else{
        form.classList.add('error');
        textError.classList.add('block');
    }
});

email.addEventListener('input', () => {
    form.classList.remove('error');
    textError.classList.remove('block');
});

function validateEmail (email) {
    var re = /(?:[a-z0-9+!#$%&'*+/=?^_`{|}~-]+(?:\.[a-z0-9!#$%&'*+/=?^_`{|}~-]+)*|"(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21\x23-\x5b\x5d-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])*")@(?:(?:[a-z0-9](?:[a-z0-9-]*[a-z0-9])?\.)+[a-z0-9](?:[a-z0-9-]*[a-z0-9])?|\[(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?|[a-z0-9-]*[a-z0-9]:(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21-\x5a\x53-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])+)\])/

    return re.test(String(email).toLowerCase());
};

```

## Desenvolvimento contínuo

Pretendo continuar focado em construir um conhecimento sólido nessas tecnologias. Ainda há muitos conceitos importantes para serem desenvolvidos. Todos os dias aprendo novos conceitos que são gradativamente adicionados ao meu repertório de ferramentas.

## Recursos úteis
- [Mdn](https://developer.mozilla.org/en-US/) - O Mozilla Developer Network (MDN) desempenha um papel crucial ao fornecer recursos abrangentes e atualizados para desenvolvedores web em todo o mundo.
- [W3School](https://www.w3schools.com/css/default.asp) - Esse site sempre me ajuda a resolver qualquer problema relacionados a códigos de uma maneira fácil e muito rápida.
- [Dev em Dobro](https://www.youtube.com/@DevemDobro) - Este é um canal onde encontro muito material. Tem muito conteúdo relacionado ao desenvolvimento. Recomendo a todos que querem aprender sobre esse e outros conceitos relacionados.

## Autor

[Fernando Mendes](https://www.linkedin.com/in/fernandomendesti/)

