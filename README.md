# itcss-boilerplate

## ITCSS, Sass and BEM

- The goal of ITCSS is to have a clear and strict structure way to specificate (s)css styles. 
- The direction of the following explained file structure goes from generic (low specificity) to explicit (high specificity).

## using wonderful vendor projects

- https://github.com/necolas/normalize.css
- https://github.com/zessx/sass-flexbox

### structure

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

### links

- http://itcss.io/
- https://speakerdeck.com/dafed/managing-css-projects-with-itcss
- [ITCSS Talk by Harry Roberts](http://youtu.be/1OKZOV-iLj4)