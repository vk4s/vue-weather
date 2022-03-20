<template>
    <main>
        <div class="search-box">
            <input type="text" id="search-bar" class="search-bar" placeholder="location..." />
        </div>

        <div class="weather-wrap">
            <div class="location-box">
                <div class="location">London, UK</div>
                <div class="date">Monday 20, January 2022</div>
            </div>

            <div class="weather-box">
                <div class="temp">9&deg;C</div>
                <div class="weather">Rain</div>
            </div>
        </div>
    </main>
</template>

<script>
export default {
    name: "app",
    data() {
        return {};
    },
};
</script>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: "montserat", sans-serif;
    display: flex;
    justify-content: center;
    background: linear-gradient(165deg, #bae0ff, #1c4a7e);
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
}

#app {
    background-image: url("./assets/cold.bmp");
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    transition: 0.5s;
    overflow: hidden;
    display: flex;
}

main {
    height: 100vh;
    width: 500px;
    background: linear-gradient(to bottom, rgb(0, 0, 0, 0.25), rgb(0, 0, 0, 0.75));
    padding: 20px;
}

/* .search-box {
    width: 100%;
} */

.search-box .search-bar {
    display: block;
    width: 100%;
    padding: 15px;
    margin: auto;

    color: #313131;
    font-size: 20px;

    appearance: none;
    border: none;
    outline: none;
    background: none;

    background-color: rgba(255, 255, 255, 0.25);
    border-radius: 10px;
    box-shadow: 1px 1px 5px rgb(0, 0, 0, 0.25);
    transition: 0.5s;
}

.search-box .search-bar:focus {
    background-color: rgba(255, 255, 255, 0.75);
    box-shadow: 1px 1px 15px rgb(0, 0, 0, 0.25);
}

.weather-wrap {
    margin-top: 20px;
}

.location-box .location {
    color: white;
    font-size: 32px;
    font-weight: 500;
    text-align: center;
    text-shadow: 1px 3px rgba(0, 0, 0, 0.25);
}

.location-box .date {
    color: white;
    font-size: 20px;
    font-weight: 100;
    font-style: italic;
    text-align: center;
}

.weather-box {
    text-align: center;
}

.weather-box .temp {
    display: inline-block;
    padding: 10px 25px;
    color: white;
    font-size: 100px;
    font-weight: 900px;

    text-shadow: 3px 6px rgba(0, 0, 0, 0.25);
    background-color: rgba(255, 255, 255, 0.25);
    border-radius: 15px;
    margin: 25px 0px;

    box-shadow: 3px 6px rgba(0, 0, 0, 0.25);
}

.weather-box .weather {
    color: white;
    font-size: 48px;
    font-weight: 700;
    font-style: italic;
    text-shadow: 3px 6px rgba(0, 0, 0, 0.25);
}
</style>
