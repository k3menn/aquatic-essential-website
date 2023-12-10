<template>
    <div class="carousel">
        <div class="arrows">
            <img class="arrow__left" src="/src/assets/svg/left-arrow.svg" alt="Left Arrow">
            <img class="arrow__right" src="/src/assets/svg/right-arrow.svg" alt="Right Arrow">
        </div>
        <!-- <img src="/src/assets/img/aquatic_1.png" alt="santehnika"> -->
        <div class="carousel-info">
            <div class="carousel-info-text">
                <div class="carousel-info__name">
                    <span>САНТЕХНИКА</span>
                </div>
                <div class="carousel-info__description">
                    <p>Мы предоставляем большой выбор сантехники на любой вкус по выгодным ценам.</p>
                    <p>Предлагаем вам ознакомиться с нашим ассортиментом.</p>
                </div>
                <a href="#" class="carousel-info-button">Ознакомиться</a>
            </div>
        </div>
    </div>
</template>

<style scoped>
.carousel {
    background: url('/src/assets/img/aquatic_1.png'); 
    height: 858px;
    display: flex;
    align-items: center;
    justify-content: flex-end;
}

.arrows {
    position: absolute;
    display: flex;
    justify-content: space-between;
    width: 100%;
}
.arrow__left {
    margin-left: 22px;
}

.arrow__right {
    margin-right: 10px;
}
.arrows img {
    cursor: pointer;
}



.carousel-info {
    /* height: 200px; */
    width: 450px;
    padding: 25px 40px;
    margin-right: 300px;
    position: relative;
    /* z-index: 1; Ensure the .carousel-info appears above the arrows */
    margin-bottom: 400px;
    display: flex;
    flex-direction: column;
    background-color: rgba(73, 71, 71, 0.5); /* Используйте цвет с альфа-каналом (RGBA) для полупрозрачности */
    border-radius: 10px; /* Радиус скругления углов */
    justify-content: center;
    align-items: center;
    color: #000; /* Цвет текста внутри блока */
}

.carousel-info::before {
    content: ''; /* Add content to the pseudo-element */
    
    width: 264px;
    height: 2px;
    background-color: white; /* Border color */
    position: absolute; /* Position absolutely within .carousel-info */
    top: 0; /* Position at the top of .carousel-info */
    left: 128px; /* Align with the left edge of .carousel-info */
    /* z-index: 2; Ensure the border appears above .carousel-info */

}

.carousel-info__name{
    font-family: 'Yeseva One', serif;
    font-size: 64px;
    color: #F9DD9C;
}
/* .carousel-info__name__line{
    margin-top: 0px;
    border-top: 2px solid white;
} */
.carousel-info__description{
    font-family: 'Montserrat', sans-serif;
    font-weight: 400;
    font-size: 20px;
    color: #FFFFFF;
}
.carousel-info-button {
    font-family: 'Montserrat', sans-serif;
    font-weight: 600;
    text-decoration: none;
    font-size: 20px;
    display: inline-block;
    padding: 10px 20px;
    background-color: #DEE0DD;
    color: #000000;
    border: none;
    border-radius: 12px;
}

</style>