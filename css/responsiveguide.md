dont use px for width, use percentage
max-width: 1200px
margin = rem
fontsize = rem
padding = em
alturas/height = auto

image responsive:
img {
  max-width: 100%;
  height: auto;
  display: block;
}

ever use flex box & flex wrap for automathic responsive

mobile first:

body {
  font-family: sans-serif;
}

.cards {
  display: flex;
  flex-direction: column;
}
then big screens:
@media (min-width: 768px) {
  .cards {
    flex-direction: row;
  }
}

--------
enough
@media (min-width: 768px) {
  /* tablet */
}

@media (min-width: 1024px) {
}
--------
responsive menus:
nav ul {
  display: flex;
  gap: 1rem;
}
@media (max-width: 767px) {
  nav ul {
    flex-direction: column;
  }
}

use maxwidth for center content:
.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 1rem;
}

avoid horizontal scroll:
body {
  overflow-x: hidden;
}


note:
.parent{
    display: flex;
    gap: 1rem;
    flex-wrap: wrap;
}
.children{
    flex: 1 1 auto;
}

