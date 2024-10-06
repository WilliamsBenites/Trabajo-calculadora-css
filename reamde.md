```<!-- <div class="container">
<div class="container-items">
<div class="item">1</div>
<div class="item">2</div>
<div class="item">3</div>
<div class="item">4</div>
<div class="item">5</div>
<div class="item">6</div>
<div class="item">7</div>
<div class="item">8</div>
<div class="item">9</div>
<div class="item">10</div>
</div>
</div>
```
    ```<hr> -->
    ```

```<div class="container">
<div class="Box">
<div class="item-a">Header</div>
<div class="item-b">Main</div>
<div class="item-c">Carrousel</div>
<div class="item-d">footer</div>
</div>
</div>
```

# CSS DEL EJEMPLO GRID

html,body {
    width: 100%;
    height: 100%;
    margin: 0;
    padding: 0;
}
 
.container {
    height: inherit;
    width: inherit;
    border: 1px solid;
}
 
.container-items {
    border: 1px solid red;
    height: inherit;
    display: grid;
    grid-template-columns: repeat(2,100px);
    grid-template-rows: repeat(5,100px);
    gap: 5px 50px; /* Fila , columna */
    justify-content: center;
    align-content: center;
}
.item {
    display: flex;
    justify-content: center;
    align-items: center;
    border: 1px solid blue;
}
 
 
/* Grid area */
 
.item-a {
    grid-area: header;
    border: 1px solid;
}
 
.item-b {
    grid-area: main;
    border: 1px solid;
}
 
.item-c {
    grid-area: carrousel;
    border: 1px solid;
}
 
.item-d {
    grid-area: footer;
    border: 1px solid;
}
 
.Box {
    border: 1px solid red;
    height: inherit;
    display: grid;
    grid-template-columns: repeat(4,200px);
    grid-template-rows: auto;
    grid-template-areas:
        "header header header header"
        "main main . carrousel"
        "footer footer footer footer";
    justify-content: center;
}

# Otro ejemplo (FLEX)
```<section class="container">
    <article class="carrousel">
        <header class="carrousel-header">
            <h1 class="carrousel-title">Carrusel de tarjetas</h1>
        <div class="buttons-group">
        <button class="btn btn-left"> < </button>
        <button class="btn btn-right"> > </button>
    </div>
</header>
<div class="carrousel-cards">
    <div class="card">
        <div class="card-header">
            <h2>Title</h2>
        </div>
    <div class="card-body">
         <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Itaque voluptate consequatur laborum tempore fugit possimus nihil labore? Molestiae possimus maiores culpa odio. Quisquam culpa, amet distinctio cupiditate doloribus alias tempore?
        </p>
    <div class="button-action">
<button class="btn btn-primary">Acción</button>
</div>
</div>
</div>
```
## EN CSS(FLEX)
html, body {
    width: 100%;
    height: 100%;
    margin: 0;
    padding: 0;
}
 
.container {
    height: inherit;
    display: flex;
    justify-content: center;
    align-items: center;
    /* border: 2px solid red; */
}
 
.carrousel-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.carrousel-title {
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    font-size: 2rem;
}
 
.carrousel-cards {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
    gap: 10px;
}
.card {
    width: 200px;
    border-radius: 10px;
    background-color: cadetblue;
    padding: 10px;
    border: 1px solid;
}
 
 
.btn {
    background-color: transparent;
    border: none;
    margin: 0;
    padding: 0;
}
 
.btn-left, .btn-right {
    background-color: black;
    color: white;
    font-weight: bold;
    padding: 10px;
    border-radius: 100%;
    cursor: pointer;
}
 
.button-action {
    width: 100%;
}
 
.btn-primary {
    width: inherit;
    background-color: dodgerblue;
    color: white;
    padding: 10px;
    border: 1px solid blue;
    border-radius: 10px;
    cursor: pointer;
}