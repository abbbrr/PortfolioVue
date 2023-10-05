<script>
    export default{
        name: "Main",
    };
</script>

<template>
	<header>
		<div class = "first_header">
			<h2>Hi, I am <br> Ablaikhan Rauan</h2>
			<p>iOS Developer</p>
		</div>
		<div class = "second_header">
      <img src="/src/assets/abr.PNG" alt="men" >
		</div>
	</header>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=DM+Sans:opsz,wght@9..40,300&family=Open+Sans:wght@300&family=Preahvihear&display=swap');

/* Общие стили для header */
header {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 100px;
}


/* Стили для .first_header */
.first_header h2 {
  color: #FFF;
  font-family: 'Preahvihear', sans-serif;
  font-size: 50px;
  font-style: normal;
  font-weight: 400;
  line-height: 126.664%;
  letter-spacing: 1px;
  overflow-wrap: break-word;
  margin: 0;
}

.first_header p {
  color: #828282;
  font-family: 'Preahvihear', sans-serif;
  font-size: 18px;
  font-style: normal;
  font-weight: 500;
  line-height: normal; 
  margin: 0;
}

.first_header{
  padding: 20px;
}

/* Стили для .second_header */
.second_header img{
  margin: 0 50px;
  padding: 20px;
  width: 280px;
  height: 280px;
  border-radius: 431px;
  background: radial-gradient(50% 50% at 50% 50%, #308a3b 0%, rgba(50, 15, 133, 0.00) 100%);

}

@media (max-width: 1008px) {
  header {
    margin: 130px; /* Увеличил отступ для планшетов и более крупных устройств */
    flex-direction: row; /* Вернул направление flex для планшетов и более крупных устройств */
    justify-content: space-between;
    align-items: center;
  }
  
  .second_header {
    width: 401.265px; /* Уменьшил ширину для планшетов и более крупных устройств */
    height: 401.265px; /* Уменьшил высоту для планшетов и более крупных устройств */
	margin: 50px;
  }
}


@media (max-width: 768px) {
  header {
    margin: 100px; /* Увеличил отступ для планшетов и более крупных устройств */
    flex-direction: column; /* Вернул направление flex для планшетов и более крупных устройств */
    justify-content: space-between;
    align-items: center;
  }
  
  .second_header {
    width: 351.265px; /* Уменьшил ширину для планшетов и более крупных устройств */
    height: 351.265px; /* Уменьшил высоту для планшетов и более крупных устройств */
	  margin: 50px;
  }
}

</style>
