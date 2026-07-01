  1. Grid Kya Hai?
CSS Grid ek 2D layout system hai jo elements ko rows aur columns dono mein ek saath control karne deta hai.
Flexbox  → 1D (ya row YA column)
Grid     → 2D (row AUR column dono ek saath)
Grid Layout:
┌────────┬────────┬────────┐
│  Item1 │  Item2 │  Item3 │  ← Row 1
├────────┼────────┼────────┤
│  Item4 │  Item5 │  Item6 │  ← Row 2
├────────┼────────┼────────┤
│  Item7 │  Item8 │  Item9 │  ← Row 3
└────────┴────────┴────────┘

2. Grid Kaise Use Karein?
Basic Setup
css.container {
  display: grid;
}

grid-template-columns — Columns banana
css.container {
  display: grid;

  /* 3 equal columns */
  grid-template-columns: 200px 200px 200px;

  /* fr unit — flexible ratio */
  grid-template-columns: 1fr 1fr 1fr;

  /* repeat shorthand */
  grid-template-columns: repeat(3, 1fr);

  /* mixed sizes */
  grid-template-columns: 200px 1fr 2fr;
}

grid-template-rows — Rows banana
css.container {
  display: grid;
  grid-template-rows: 100px 200px 100px;  /* 3 rows ki height */
  grid-template-rows: repeat(3, 150px);
  grid-template-rows: auto auto auto;      /* content ke hisaab se */
}

gap — Rows aur Columns ke beech space
css.container {
  display: grid;
  gap: 20px;              /* row aur column dono mein 20px */
  row-gap: 10px;          /* sirf rows ke beech */
  column-gap: 30px;       /* sirf columns ke beech */
}

grid-template-areas — Named Areas (Visual Layout)
css.container {
  display: grid;
  grid-template-columns: 1fr 3fr 1fr;
  grid-template-rows: auto 1fr auto;
  grid-template-areas:
    "header  header  header"
    "sidebar main    aside"
    "footer  footer  footer";
}

.header  { grid-area: header; }
.sidebar { grid-area: sidebar; }
.main    { grid-area: main; }
.aside   { grid-area: aside; }
.footer  { grid-area: footer; }
┌─────────────────────────┐
│         HEADER          │
├────────┬────────┬───────┤
│SIDEBAR │  MAIN  │ ASIDE │
├────────┴────────┴───────┤
│         FOOTER          │
└─────────────────────────┘

Item ko multiple columns/rows mein failana
css.item {
  grid-column: 1 / 3;    /* column 1 se 3 tak */
  grid-row: 1 / 2;       /* row 1 se 2 tak */
  
  /* ya span use karke */
  grid-column: span 2;   /* 2 columns cover karo */
  grid-row: span 3;      /* 3 rows cover karo */
}

Alignment in Grid
css.container {
  /* Sabhi items ko align karo */
  justify-items: center;    /* horizontal (row axis) */
  align-items: center;      /* vertical (column axis) */

  /* Poore grid ko align karo container mein */
  justify-content: center;
  align-content: center;
}

/* Individual item ke liye */
.item {
  justify-self: end;
  align-self: start;
}

3. Flex vs Grid — Difference 📊

Sabse Bada Farak
FlexboxGridDimension1D (ek direction)2D (row + column)ControlItems control karte hainContainer control karta haiBest ForComponents, nav barsFull page layoutsDirectionRow ya ColumnDono ek saath

Detailed Comparison
FeatureFlexboxGridLayout type1D2DAlignmentEk axis peDono axis peItem sizingContent ke hisaab seGrid ke hisaab seGapsgapgap (zyada control)Template areas❌ Nahi✅ HaanBrowser supportBahut acchaBahut acchaOverlapping itemsMushkilAasaanResponsiveflex-wrap seauto-fill/auto-fit se

Kab Kya Use Karein?
Flexbox use karo jab:
css/* Navigation bar */
nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

/* Buttons ek line mein */
.btn-group {
  display: flex;
  gap: 10px;
}

/* Card ke andar content */
.card {
  display: flex;
  flex-direction: column;
}
Grid use karo jab:
css/* Full page layout */
.page {
  display: grid;
  grid-template-areas:
    "header"
    "main"
    "footer";
}

/* Image gallery */
.gallery {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 16px;
}

/* Dashboard */
.dashboard {
  display: grid;
  grid-template-columns: 250px 1fr;
}

Dono Saath Use Karo! ✨
css/* Grid se page layout banao */
.page {
  display: grid;
  grid-template-columns: 1fr 3fr;
}

/* Flexbox se items andar align karo */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

Quick Recap 🧠
Grid   = Table jaisa layout (rows + columns dono)
Flex   = Line jaisa layout (ek direction)

Grid   → Page ka structure banao
Flex   → Us structure ke andar items align karo

Dono ko saath use karna = Best Practice! 💪