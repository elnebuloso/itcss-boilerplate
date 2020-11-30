# itcss-boilerplate

![abandoned](https://img.shields.io/badge/project-abandoned-red)

## ITCSS, Sass and BEM

- The goal of ITCSS is to have a clear and strict structure way to specificate (s)css styles. 
- The direction of the following explained file structure goes from generic (low specificity) to explicit (high specificity).

### using wonderful vendor projects

- https://github.com/necolas/normalize.css
- https://github.com/zessx/sass-flexbox

## compiling examples

```
docker run -v ${PWD}:/app elnebuloso/compass compass compile /app/public
docker run -v ${PWD}:/app elnebuloso/compass compass watch /app/public --poll
```

### ITCSS

#### 01-variables

- ITCSS (settings)

#### 02-mixins

- ITCSS (tools)
- vendor folder contains external projects scss files

#### 03-normalize

- ITCSS (generic)
- vendor folder contains external projects scss files

#### 04-tags

- ITCSS (base)
- styling standard html tags

#### 05-patterns

- ITCSS (objects)

#### 06-components

- ITCSS (components)

#### 07-externals

- ITCSS (no equivalent)
- vendor folder contains external projects scss files

#### 08-override

- ITCSS (trumps)
- Only Place where !important allowed

### BEM

```
/**
 * Block
 */
.c-example {

    /* 1: Add the direct properties of the element */
    property: value;

    /* 2: Add media queries or print styles */
    @media (--breakpoint-10) {
        property: value;
    }

    /* 3: Add selectors of the parent element */
    &:hover {
        property: value;
    }

    /* 4: Add temporary states of the parent element */
    &.is-open {
        property: value;
    }

    /* 5: Add nested elements */
    & strong {
        property: value;
    }
}

/*
 * Modifier
 */
.c-example--modifier {
    property: value;
}

/*
 * Element
 */
.c-example__subcomponent {
    property: value;
}
```

### links

- http://sass-lang.com
- http://compass-style.org/
- http://chriseppstein.github.io/blog/2010/05/17/where-are-your-images/
- http://itcss.io/
- https://speakerdeck.com/dafed/managing-css-projects-with-itcss
- [ITCSS Talk by Harry Roberts](http://youtu.be/1OKZOV-iLj4)
- http://thesassway.com/editorial/sass-vs-scss-which-syntax-is-better