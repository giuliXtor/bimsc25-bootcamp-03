<template>
    <div id="navBar" class="flexRow spaceBetween alignCenter">
        <div class="flexRow">
            <i class="mdi mdi-food-fork-drink" style="font-size: 25px; padding-right: 10px"></i>
            <h3 style="margin:0">Giulia's Cafe</h3>
        </div>

        <div class="flexRow">
            <span id="about">About</span>
            <span id="content">Contact</span>
        </div>
    </div>
    <div class="flexRow" style="height: calc(100vh - var(--navBarHeight));">
        <div id="sidebar" class="flexColumn">
            <span class="mealTime" id="breakfast">Breakfast</span>
            <span class="mealTime" id="lunch">Lunch</span>
            <span class="mealTime" id="dinner">Dinner</span>
        </div>
        <div id="main">
            <div id="breakfastFoods" class="flexRow wrap">
                <div class="menuItem">
                    <img src="./assets/breakfastImages/bagel.jpg" width="100%" height="133px">
                    <h4>Bagel</h4>
                    <p>Bagel with cream cheese</p>
                </div>
                <div class="menuItem">
                    <img src="./assets/breakfastImages/omelet.jpg" width="100%">
                    <h4>Omelet</h4>
                    <p>4 egg omelet with cheese</p>
                </div>
                <div class="menuItem">
                    <img src="./assets/breakfastImages/pancakes.jpg" width="100%">
                    <h4>Pancakes</h4>
                    <p>Pancakes with syrup</p>
                </div>
            </div>
            
            <div id="lunchFoods" class="flexRow wrap">
                <div class="menuItem">
                    <img src="./assets/lunchImages/soup.jpg" width="100%">
                    <h4>Soup</h4>
                    <p>Tomato</p>
                </div>
                <div class="menuItem">
                    <img src="./assets/lunchImages/sandwhich.jpg" width="100%">
                    <h4>Sandwhich</h4>
                    <p>Chicken and Avocado</p>
                </div>
            </div>
            
        </div>
    </div>
</template>





<style scoped>
:root {
    --navBarHeight: 30px;
    --sideBarHeight: 200px
}

#navBar {
    background-color: rgb(233, 203, 253);
    height: var(--navBarHeight);
    padding: 20px
}

#sidebar {
    background-color: rgb(102, 102, 139);
    width: var(--sideBarHeight);
    padding: 10px
}

#main {
    background-color: rgb(145, 208, 219);
    width: calc(100vw - var(--sideBarHeight));
    padding: 10px
}

.flexRow {
    display: flex;
}

#about {
    margin-right: 10px;
}

.menuItem {
    width: 200px;
    height: 250px;
    margin: 4px;
}

.flexColumn {
    display: flex;
    flex-direction: column;
}

.box {
    height: 100px;
    width: 100px;
    background-color:azure;
    border: 1px solid black;
    margin: 4px;
}

.spaceBetween {
    justify-content: space-between;
}

.spaceAround {
    justify-content: space-around;
}

.wrap {
    flex-wrap: wrap;
}

.justifyCenter {
    justify-content: center;
}

.alignCenter {
    align-items: center;
}

.flexStart {
    justify-content: flex-start;
}

.flexEnd {
    justify-content: flex-end;
}

body {
    margin: 0px;
}

.mealTime {
    margin: 10px;
    color: white
}
</style>
