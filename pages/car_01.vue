
あなた:
<template>
  <div class="container mt-5">
    <h1 class="text-center">車の歴史</h1>
    <div v-for="car in cars" :key="car.name" class="card mb-3">
      <div class="row g-0">
        <div class="col-md-4">
          <img :src="car.image" class="img-fluid rounded-start" alt="車の画像">
        </div>
        <div class="col-md-8">
          <div class="card-body">
            <h2 class="card-title">{{ car.name }}</h2>
            <p class="card-text"><strong>馬力:</strong> {{ car.horsepower }} PS</p>
            <p class="card-text"><strong>エンジン:</strong> {{ car.engine }}</p>
            <p class="card-text"><strong>トルク:</strong> {{ car.torque }} Nm</p>
            <p class="card-text"><strong>重量:</strong> {{ car.weight }} kg</p>
            <p class="card-text"><strong>最高速度:</strong> {{ car.topSpeed }} km/h</p>
            <p class="card-text"><strong>更新内容:</strong> {{ car.update }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      cars: [
        {
          name: "Benz Patent-Motorwagen",
          horsepower: 0.75,
          engine: "単気筒",
          torque: 10,
          weight: 265,
          topSpeed: 16,
          update: "世界初の自動車",
          image: "/img/patent.jpg"
        },
        {
          name: "Bugatti Veyron Super Sport",
          horsepower: 1200,
          engine: "W16 8.0L",
          torque: 1500,
          weight: 1888,
          topSpeed: 431,
          update: "史上初の最高速度 - 時速400km到達",
          image: "/img/veyron.jpg"
        },
        {
          name: "Tesla Model S Plaid",
          horsepower: 1020,
          engine: "3モーター電気",
          torque: 1420,
          weight: 2162,
          topSpeed: 322,
          update: "0-100 km/h 1.99秒 - 加速の記録更新",
          image: "/img/modelS-plaid.jpg"
        },
        {
          name: "Koenigsegg Regera",
          horsepower: 1500,
          engine: "V8 5.0L ハイブリッド",
          torque: 2000,
          weight: 1590,
          topSpeed: 400,
          update: "0-400-0の記録更新 - 31.49秒",
          image: "/img/regera.jpg"
        },
        {
          name: "Koenigsegg Jesko Absolut",
          horsepower: 1600,
          engine: "V8 5.0L",
          torque: 1500,
          weight: 1320,
          topSpeed: 500,
          update: "理論上世界最高速",
          image: "/img/jesko-absolut.webp"
        },
        {
          name: "Rimac Nevera",
          horsepower: 1914,
          engine: "4モーター電気",
          torque: 2360,
          weight: 2150,
          topSpeed: 412,
          update: "0-300 km/h 9.3秒 - 電気自動車の新記録 ",
          image: "/img/Rimac_Nevera.jpg"
        },
        {
          name: "Rolls-Royce Boat Tail",
          horsepower: 563,
          engine: "V12 6.75L",
          torque: 900,
          weight: 3000,
          topSpeed: 250,
          update: "世界で最も高額な車 40億6000万円",
          image: "/img/boattail.png"
        },
        {
          name: "ferrari LaFerrari",
          horsepower: 963,
          engine: "V12 6.3L ハイブリッド",
          torque: 900,
          weight: 1585,
          topSpeed: 350,
          update: "歴史的な三台の一つ",
          image: "/img/laferrari.jpg"
        },
        {
          name: "Porsche 918 Spyder",
          horsepower: 887,
          engine: "V8 4.6L ハイブリッド",
          torque: 1280,
          weight: 1675,
          topSpeed: 345,
          update: "歴史的な三台の一つ",
          image: "/img/918.jpg"
        },
        {
          name: "McLaren P1",
          horsepower: 916,
          engine: "V8 3.8L ハイブリッド",
          torque: 900,
          weight: 1547,
          topSpeed: 350,
          update: "歴史的な三台の一つ",
          image: "/img/p1.jpg"
        }
      ],
    };
  },
};
</script>

<style>
</style>