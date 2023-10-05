<script>
export default{
    name: "Header",
};
</script>

<template>
    <header>
        <div class="first_headers">
            <h2>Welcome to my portfolio!</h2>
            <p>I am an iOS developer passionate about this field for over a year. My passion for mobile development, specifically the iOS platform, inspires me to create innovative and user-friendly applications.</p>
        </div>
        <div class="second_headers">

        </div>
    </header>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=DM+Sans:opsz,wght@9..40,300&family=Open+Sans:wght@300&family=Preahvihear&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@300&display=swap');

header{
    justify-content: center;
    margin: 30px;
}
.first_headers h2{
 color: #FFF;
 text-align: center;
  font-family: 'Preahvihear', sans-serif;
 font-size: 48px;
 font-style: normal;
 font-weight: 700;
 line-height: normal;
}
.first_headers {
    width: 745px;
    height: 136px;
    flex-shrink: 0;
}
.first_headers p{
 color: #FFF;
 text-align: center;
  font-family: 'Preahvihear', sans-serif;
//font-family: 'Open Sans', sans-serif;
 font-size: 20px;
 font-style: normal;
 font-weight: 400;
 line-height: normal;
}

</style>