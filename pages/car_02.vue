<template>
 <div class="container mt-5">
   <h1 class="text-center">歴史的な三台</h1>
   <div v-for="car in cars" :key="car.name" class="card mb-3">
     <div class="row g-0">
       <div class="col-md-4">
         <img :src="car.image" class="img-fluid rounded-start" alt="車の画像" />
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
   <!-- 戻るリンク -->
   <a href="car_01.vue" class="btn btn-secondary mt-3">戻る</a>
 </div>
</template>

<script>
export default {
 data() {
   return {
     cars: [
       {
         name: "ferrari LaFerrari",
         horsepower: 963,
         engine: "V12 6.3L ハイブリッド",
         torque: 900,
         weight: 1585,
         topSpeed: 350,
         update: "歴史的な三台の一つ",
         image: "/img/laferrari.jpg",
       },
       {
         name: "Porsche 918 Spyder",
         horsepower: 887,
         engine: "V8 4.6L ハイブリッド",
         torque: 1280,
         weight: 1675,
         topSpeed: 345,
         update: "歴史的な三台の一つ",
         image: "/img/918.jpg",
       },
       {
         name: "McLaren P1",
         horsepower: 916,
         engine: "V8 3.8L ハイブリッド",
         torque: 900,
         weight: 1547,
         topSpeed: 350,
         update: "歴史的な三台の一つ",
         image: "/img/p1.jpg",
       },
     ],
   };
 },
};
</script>
