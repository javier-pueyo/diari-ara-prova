# Barra | Component per a Ara.cat

A continuació hi ha una breu explicació de com s'ha construït el component de *Barra*, d'ara endavant anomenat com *barVote*.

El codi es va escriure en anglès, per costum més que res, però no hi hauria problema de fer-ho en català.

M'agradaria aclarir per endavant, que es va comentar en l'anunciat de l'exercici que es lliurés com si fos un *iframe*. Encara que per a mostrar el component d'una forma més agradable es va situar en el centre de la pantalla mitjançant un `contenidor` (En l'apartat [HTML](#html) s'explica en més detall).


## Taula de contingut

- [Aspectes generals](#aspectes-generals)
- [HTML](#html)
- [Estils](#estils)
- [Contacte](#contacte)

## Aspectes generals

El directori d'arxius està format per:

1. **Imatges** `/assets/*img`
2. **SCSS** `/assets/*scss`. En el html s'utilitza el css comprimit: *main.min.css*
3. **HTML**. Solament s'utilitza l'arxiu *index.html*

Com la prova es tractava de html i css vaig fer solament una simulació de com s'afegiria el percentatge dels vots. Es va utilitzar estils inline simulant que mitjançant l'atribut `vote-percent` s'inclou el valor del percentatge i mitjançant javascript es crea dinàmicament els estils `width:51.2%`.
```sh
<div class="barVote__percent--left" vote-percent="51.2" style="width:51.2%">51,2%</div>
```

## HTML

El component comença des del tag:

```sh
<section class="barVote">
```

La classe `contenidor contenidor--center` únicament s'utilitza amb finalitats estètics per a mostrar el component.

## Estils

Es va utilitzar principalment *flexbox* per a un millor control de la grandària dels `div`, en comptes de *grid layout*.

Es va fer ús del *mockup de Figma* per a replicar les propietats de les tipografies, els espais i colors.

Finalment es va treballar el responsive a partir del *breakpoints* que s'esmenta en el *Figma* `774px`.

Els estils principals del component *barVote* troben en el directori `/assets/*components/_*barVote.scss`. La resta d'arxius scss són per a preparar l'entorn (variables globals, mixins, tipografies, etc).

## Contacte

1. **Telèfon**: 609 650 420
2. **Email**: [hola@pueyomir.com](mailto:hola@pueyomir.com)
3. **LinkedIn**: [Veure el meu perfil](https://www.linkedin.com/in/pueyojavier)
