<template>
  <div id="app">
    <header>
      <h1>Visita Corea del Sur</h1>
    </header>

    <nav class="nav">
        <div class="logo-header">
            <a><img src="./logo.png" alt="" class="logo"></a>
        </div>
        <div class="nav-menu">
            <input type="checkbox" id="check">    
            <label for="check" class="checkbtn">
                <i class="menu-icon"><img src="./menu.png" alt=""></i>
            </label>
            <ul class="naveg">
                <li><a href="#intro">Inicio</a></li>
                <li><a href="#Dest">Destinos</a></li>
                <li><a href="#Event">Eventos</a></li>
                <li><a href="#Act">Actividades</a></li>
                <li><a href="#Food">Gastronomía</a></li>
                <li><a href="#transporte">Como llegar</a></li>
                <li><a href="#cont">Contacto</a></li>
            </ul>
        </div>
      </nav>

    <main>

      <a name="intro"></a>
      <section>
        <h2 class="subt">¿Por qué visitar Corea?</h2>
        <div>
          <p class="int">¡Corea del Sur es un destino turístico que deslumbra con su mezcla única de encanto tradicional y modernidad vibrante! Sumérgete en una experiencia inolvidable mientras exploras este país cautivador que equilibra a la perfección su rica historia con un paisaje contemporáneo emocionante.</p>
          <br>
          <b>Diversidad Geográfica:</b><p class="int">Desde las bulliciosas metrópolis de Seúl y Busan hasta los paisajes impresionantes de la isla de Jeju, Corea del Sur ofrece una diversidad geográfica que sorprende en cada rincón. Descubre la energía palpable de las calles de Seúl, donde rascacielos modernos coexisten con antiguos palacios y templos. En la isla de Jeju, maravíllate con paisajes volcánicos, cascadas espectaculares y playas de arena negra, todo enmarcado por el imponente Monte Hallasan.</p>
          <br>
          <b>Cultura e Historia Milenaria:</b><p class="int">Sumérgete en la rica herencia cultural de Corea a través de sus monumentos históricos, como el Palacio Gyeongbokgung y el Templo Bulguksa, ambos declarados Patrimonio de la Humanidad por la UNESCO. Participa en festivales tradicionales, disfruta de la exquisita gastronomía coreana, y vive la calidez de la hospitalidad local mientras exploras mercados callejeros llenos de vida y color.</p>
          <br>
          <b>Aventuras al Aire Libre:</b><p class="int">Para los amantes de la aventura, Corea del Sur ofrece una variedad de actividades emocionantes. Surfea en las playas de Yangyang en Gangwon-do, donde las olas son ideales para principiantes y expertos por igual. Explora la belleza submarina con kayak transparente en las cristalinas aguas de Jeju, o embárcate en un emocionante recorrido en kayak por el puerto de Janghohang en Gangwon-do.</p>
          <br>
          <b>Gastronomía Exquisita:</b><p class="int">Deléitate con la deliciosa gastronomía coreana, desde platos clásicos como el bulgogi y el kimchi hasta las especialidades locales de cada región. Descubre la cultura del té en los pintorescos campos de plantaciones de té y experimenta la autenticidad de la cocina callejera en los animados mercados locales.</p>
          <br>
          <b>Hospitalidad Inigualable:</b><p class="int">En Corea del Sur, la hospitalidad es una parte integral de la experiencia de viaje. Descubre la calidez y la amabilidad de la gente local, dispuesta a compartir sus tradiciones y a guiarte en una travesía inolvidable.</p>
          <br>
          <b>Conclusión:</b><p class="int">En resumen, Corea del Sur te invita a un viaje único donde cada momento es una oportunidad para explorar, aprender y disfrutar. Desde la fusión de la antigua esencia asiática hasta la vibrante modernidad, este país cautivador tiene algo para cada tipo de viajero. ¡Prepárate para sumergirte en la maravilla que es Corea del Sur y crear recuerdos que perdurarán toda la vida!</p>

        </div>
      </section>

      <a name="Dest"></a>
      <section>
        <h2 class="subt">Destinos Populares</h2>
        <DestinationList :destinations="popularDestinations" />
      </section>

      <div>
        <p><b>¿Ya elegiste a donde quieres ir?</b></p><div class="separador">Si es asi ahora toca planificar las fechas para que disfrutes de una mejor experinecia dependiendo de como deseas que sea el ambiente, si quieres ir cuando no haya mucha afluencia de personas o en algun festival o evento, por eso te mostrare algunos eventos que existen en este hermoso país.</div>
      </div>

      <a name="Event"></a>
      <section>
        <h2 class="subt">Eventos</h2>
        <EventList :events="recentEvents" />
      </section>

      <div>
        <div class="separador">Ahora veamos algunas actividades que puedes realizar para disfrutar lo máximo tu estadia en Corea.</div>
      </div>

      <a name="Act"></a>
      <section>
        <h2 class="subt">Actividades de viaje</h2>
        <ActivitiesList :activities="activityList" />
      </section>

    <a name="Food"></a>
      <section>
        <h2 class="subt">Gastronomía</h2>
        <FoodList :foods="foodsList" />
      </section>

      <a name="transporte"></a>
      <section>
        <h2 class="subt">Como llegar</h2>
        <p>Desde nuestro país una de las maneras mas sencillas de llegar a Corea es por vía aerea</p><br>
        <p>Una de las maneras es ir del departamento en donde estes (en Bolivia) hasta Miami y de Miami a Corea del Sur, y para eso te sugerimos estas aereolineas</p>
        <ul>
          <li><a href="https://www.boa.bo/BoAWebSite/">De cualquier departamento de Bolivia a Miami</a></li>
          <li><a href="https://www.aa.com/homePage.do?locale=es_AR">De Miami a Corea del Sur</a></li>
        </ul>
        <p>O si gusta usted puede buscar la mejor manera para llegar al lugar en:</p>
        <ul>
          <li><a href="https://www.rome2rio.com/es/">Rome2rio</a></li>
        </ul> 
      </section>
    
      <a name="cont"></a>
      <section>
        <h2 class="subt">Contactenos</h2>
        <p>Si tiene alguna duda o desea saber algo mas puede contactarnos al <br>
          <br>
          <i><img src="./whats.png" alt="" class="conta"> 73740793</i>
        </p>
      </section>


    </main>

    <footer>
      <p>&copy; 2023 Turismo en Corea</p>
    </footer>
  </div>
</template>

<script>
import DestinationList from './components/DestinationList.vue'
import EventList from './components/EventList.vue'
import ActivitiesList from './components/ActivitiesList.vue'
import FoodList from './components/FoodList.vue';

export default {
  name: 'App',
  components: {
    DestinationList,
    EventList,
    ActivitiesList,
    FoodList,
  },
  data() {
    return {
      popularDestinations: [
        { name: 'Seúl', intro: 'Capital vibrante de Corea del Sur, donde la modernidad se mezcla con la tradición. Desde los rascacielos de Gangnam hasta los palacios antiguos de Gyeongbokgung, Seúl ofrece una experiencia única. Explora mercados animados y sumérgete en la cultura local.', image: './seoul.jpg', description: 'Seúl, la capital dinámica de Corea del Sur, es una mezcla emocionante de modernidad y tradición. Desde los rascacielos futuristas de Gangnam hasta los majestuosos palacios de Gyeongbokgung, la ciudad cuenta la historia viva de Corea. Explora los bulliciosos mercados de Namdaemun y Dongdaemun, donde se entremezclan aromas y colores. Los callejones de Insadong ofrecen un vistazo a la cultura tradicional, mientras que el animado distrito de Hongdae celebra la creatividad moderna. Seúl, con su rica historia y vida urbana vibrante, invita a los visitantes a sumergirse en la esencia misma de Corea del Sur.'},
        { name: 'Busan', intro: 'Ciudad costera encantadora con playas doradas y vibrantes mercados. Desde el sereno Templo Beomeosa hasta la moderna Torre de Busan, la ciudad equilibra la serenidad marina con la vitalidad urbana. Haeundae y Gamcheon Culture Village ofrecen experiencias únicas.', image: './busan.jpg', description: 'La ciudad portuaria de Busan, en el sur de Corea, es una joya costera con un encanto distintivo. Desde las extensas playas de Haeundae hasta la serenidad del Templo Beomeosa, Busan abraza la diversidad. El mercado de pescado Jagalchi ofrece una auténtica experiencia culinaria, mientras que el colorido Gamcheon Culture Village es un deleite para los sentidos. La moderna Torre de Busan se alza en contraste con la naturaleza circundante, creando una fusión armoniosa entre lo antiguo y lo nuevo. Con su vibrante escena cultural y su belleza costera, Busan cautiva a los viajeros en busca de experiencias únicas.' },
        { name: 'Gyeongju', intro: 'Antigua capital del Reino de Silla, Gyeongju es un tesoro histórico con templos antiguos y tumbas reales. Cada rincón respira la esencia de la rica herencia de Corea.', image: './gyeongju.jpg', description: 'Gyeongju, apodada "el museo sin paredes", es un tesoro histórico que atesora los vestigios del antiguo Reino de Silla. Los templos antiguos como Bulguksa y las tumbas reales de la zona revelan la rica herencia cultural. Pasea por el lago Anapji para experimentar la serenidad histórica y explora el Palacio Donggung para sumergirte en la elegancia real. Gyeongju es un destino donde cada piedra cuenta una historia, ofreciendo a los visitantes una ventana a la grandiosa historia de Corea.' },
        { name: 'Andong', intro: 'Sumérgete en la tradición y arquitectura conservada de Corea en Andong. Con aldeas tradicionales hanok y el famoso pueblo Hahoe, ofrece una ventana al pasado.', image: './andong.jpg', description: 'Andong, en el corazón de la provincia de Gyeongsang, es una ciudad que conserva la autenticidad de la cultura coreana. Las aldeas tradicionales hanok y el pueblo Hahoe presentan un viaje en el tiempo, ofreciendo una visión única de la vida rural. El festival de máscaras Hahoe es una celebración vibrante de la tradición, donde los visitantes pueden sumergirse en las artes y la cultura locales. Andong es un destino encantador para aquellos que buscan una experiencia auténtica en medio de la belleza natural.' },
        { name: 'Parque Nacional Seoraksan', intro: 'Para amantes de la naturaleza, el Parque Nacional Seoraksan es un paraíso montañoso. Majestuosas cumbres, arroyos y diversidad de flora y fauna hacen de este lugar un destino imperdible.', image: './seoraksan.jpg', description: 'El Parque Nacional Seoraksan, una maravilla natural en la costa este, invita a los amantes de la naturaleza a explorar sus majestuosas cumbres y exuberantes paisajes. Las rutas de senderismo, como la que conduce al pico Daecheongbong, ofrecen vistas panorámicas inolvidables. Descubre la tranquila Sinheungsa, un templo enclavado en la montaña, y déjate cautivar por la diversidad de flora y fauna. Seoraksan es un santuario natural que inspira admiración y asombro.' },
        { name: 'Jeonju', intro: 'Conocida como la cuna de la comida coreana, Jeonju deleita con su extraordinaria escena gastronómica. Desde el famoso bibimbap hasta puestos callejeros, Jeonju es un festín para los sentidos.', image: './jeonju.jpg', description: 'Conocida como la "cuna de la comida coreana", Jeonju deleita a los paladares con su extraordinaria escena gastronómica. Los callejones de Insadong están llenos de puestos de comida callejera que ofrecen delicias como el famoso bibimbap. Jeonju Hanok Village transporta a los visitantes a la era Joseon, con sus casas tradicionales y talleres de artesanía. La ciudad también alberga el Museo de la Pólvora y una animada escena artística. Jeonju es un festín para los sentidos y un destino imperdible para los amantes de la gastronomía y la cultura.' },
        { name: 'Isla de Jeju', intro: 'Un paraíso en medio del océano, la Isla de Jeju cautiva con paisajes impresionantes, playas de arena negra y la majestuosa Montaña Hallasan. Un retiro sereno y único.', image: './jeju.jpg', description: 'La Isla de Jeju, un paraíso tropical en el sur de Corea, es conocida por sus paisajes impresionantes y su atmósfera única. La Montaña Hallasan, un volcán extinto, domina el centro de la isla y ofrece oportunidades de senderismo incomparables. Las playas de arena negra, como Jungmun Saekdal y Manjanggul Cave, atraen a los amantes del sol y el mar. Jeju es también famosa por sus estatuas de piedra llamadas "dol hareubang". Con su belleza natural y su cultura única, Jeju es un destino relajante y fascinante.' },
        { name: 'Chuncheon', intro: 'Rodeada de hermosos lagos y montañas, Chuncheon es famosa por su encanto escénico y deliciosa comida callejera. Pasea por el mercado de Namsan y prueba el dak-galbi para una experiencia culinaria inolvidable.', image: './chuncheon.jpg', description: 'Chuncheon, en la provincia de Gangwon, es un refugio escénico conocido por su belleza natural y deliciosa comida callejera. El lago Soyang y el río Namiseom ofrecen paisajes serenos ideales para paseos en bote y actividades al aire libre. El dak-galbi, un plato picante de pollo, es una especialidad local que los visitantes no deben perderse. El mercado de Namsan es famoso por sus variedades de alimentos frescos y productos locales. Chuncheon combina la tranquilidad del paisaje con la emoción de los sabores locales.' },
        { name: 'Suwon', intro: 'Hogar de la impresionante Fortaleza de Hwaseong, Suwon equilibra historia con modernidad. Explora callejones empedrados, disfruta de la arquitectura histórica y sumérgete en la animada vida urbana.', image: './suwon.jpg', description: 'Suwon, una ciudad amurallada en la provincia de Gyeonggi, es hogar de la impresionante Fortaleza de Hwaseong. Esta estructura histórica, declarada Patrimonio de la Humanidad por la UNESCO, revela la maestría arquitectónica de la era Joseon. Los callejones empedrados de la ciudad conducen a plazas animadas y mercados tradicionales, mientras que el Pabellón Hwaseong ofrece vistas panorámicas. Suwon es un lugar donde la historia cobra vida entre murallas imponentes y la vitalidad de la vida moderna.' },
      ],
      recentEvents: [
        { title: 'Chuseok', date: '09-28', image: './chuseok.jpg', description: 'El Chuseok, también conocido como Hangawi (“el gran punto medio del otoño”), es una de las tres fiestas tradicionales más importantes de Corea del Sur, junto a Seollal y Dano. Se celebra el decimoquinto día del octavo mes del calendario lunar. Esta festividad abarca, normalmente, tres días. Durante este tiempo, las familias se reúnen y llevan a cabo diferentes costumbres propias de la fecha. Todo está envuelto en un profundo sentimiento de gratitud y abundancia.' },
        { title: 'Festival de linternas de Jinju', date: '10-08', image: './jinju.jpg', description: 'El Festival de linternas de Jinju ilumina la ciudad con más de 70.000 faroles flotantes, que se encienden sobre el río Namgang. El festival tiene su origen en la Batalla de la Fortaleza Jinjuseong de la Guerra de Imjin (1592-1598), ya que las linternas fueron usadas como estrategia militar del ejército de Suseong, para bloquear al ejército japonés que intentaba cruzar el río Namgang. Además, se emplearon como medio de comunicación, con el objetivo de enviar saludos a los familiares fuera del castillo, durante la invasión.' },

      ],
      activityList: [
        { name: 'Pasear en bicicleta', image: './bici.jpg', description: 'El carril para bicicletas del río Han es una de las rutas típicas, que se extiende a lo largo de la orilla del río Han en Seúl. Comenzando en el Parque Nanji Hangang (Camping Nanji), este camino es la ruta para bicicletas más larga que atraviesa el Puente Mapo, el Puente Banpo y el Bosque de Seúl hasta el Puente Gwangjin. A los ciudadanos y turistas de Seúl les encanta porque conecta Seúl con las ciudades satélites y también porque se encuentra bordeando los parques del río Hangang.' },
        { name: 'Auto Camping', image: './auto.jpg', description: 'Hay más de 2.300 campamentos de automóviles en Corea del Sur. Sobre todo, muchos campistas prefieren los campamentos ubicados en los bosques recreativos nacionales debido a su mayor rentabilidad. Las reservas están disponibles a través del sitio web del Servicio de Parques Nacionales de Corea los días 1 y 15 de cada mes. Tenga en cuenta que los campamentos son tan populares que todos se reservan en medio día poco después de que se abran las reservas.' },
        { name: 'Actividades acuáticas', image: './surf.jpg', description: 'Corea del Sur ofrece tres destinos principales para surfear: Yangyang en Gangwon-do, Busan y la isla de Jeju. Además, el kayak transparente es una actividad popular en Jeju, mientras que Janghohang en Gangwon-do es conocido por su paisaje y ofrece kayak y snorkel. Otras actividades marinas como el esnórquel y el submarinismo son populares en lugares como el puerto de Panpo en Jeju, la playa de Bongpo en Goseong y la playa de Namae en Yangyang.' },
        { name: 'Luge', image: './luge.jpg', description: 'Un trineo es una actividad de aventura llena de diversión que consiste en correr por la pista inclinada en un trineo de ruedas sin motor. Se introdujo por primera vez en Tongyeong, Gyeongsangnamdo, en 2017. Skyline Luge Tongyeong se ha convertido en un lugar turístico de visita obligada en la costa sur de Corea del Sur después de causar sensación en los servicios de redes sociales. La isla Ganghwado en Incheon también atrae a turistas con la pista de trineo más larga del este.' },

      ],

      foodsList: [
        { name: 'Bibimbap', image: './bibim.jpg'},
        { name: 'Bulgogi', image: './bulgogi.jpg'},
        { name: 'Japchae', image: './japchae.jpg'},
        { name: 'Kimbap', image: './kimbap.jpg'},
        { name: 'Kimchi', image: './kimchi.jpg'},
        { name: 'Mandu', image: './mandu.jpg'},
        { name: 'Samgyeopsal', image: './samgy.jpg'},
        { name: 'Tteokbokki', image: './tteok.jpg'},
      ]
    };
  },
};
</script>

<style>

body {
  font-family: 'Lucida Sans';
  margin: 0;
  padding: 0;
  background-color: #FFE5EC;
}

#app {
  text-align: center;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

header {
  background-color: #FB6F92;
  color: #000;
}

header h1 {
  margin: 0;
}

h1{
  font-family: Abeganshi;
  font-size: 50px;
  padding: 15px;
}

main {
  flex-grow: 1;
  padding: 20px;
}

section {
  margin-bottom: 40px;
}

h2 {
  color: #333;
}

footer {
  background-color: #FB6F92;
  color: #000;
  padding: 10px 0;
}

.subt{
  font-family: LadyN;
  font-size: 35px;
}

.conta{
  width: 3%;
}


.separador {
  padding: 60px;
  width: 55%;
  text-align: center;
  align-items: center;
  margin: 0 auto;
  text-align: justify;
}

a {
  text-decoration: none;
  color: #C71585;
}

a:hover {
  color: #FF69B4; 
}

.int{
  padding: 5px;
}

.naveg{
  list-style: none;
}

.nav{
    background-color: #FF8FAB;
    color: #fff;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 8px 5px;
    
}
.logo{
    height: 45px;
    padding-left: 10px;
}
.nav-menu ul{
    display: flex;
    align-items: center;
}
.nav-menu li{
    margin-right: 1rem;
}
.nav-menu a{
    color: #fff;
    text-decoration: none;
}

.menu-icon, #check{
    display: none;
}

@media (max-width:768px){
    .checkbtn{
        display: block;
    }

    .menu-icon img{
    width: 20px;
    height: 20px;
}
    .menu-icon{
        display: block;
        top: 105px;
        cursor: pointer;
        padding-right: 15px;
    }
    .nav-menu ul{
        display: block;
        position: fixed;
        top:135px;
        left:-120%;
        background: #FF8FAB;
        width: 100%;
        height: 100vh;
        right: 0;
    }
    .nav-menu ul li{
        padding: 20px;
        justify-content: center;
    }
  
    #check:checked ~ ul{
        left: 0;
        transition: all .25s;
    }
}


@font-face {
  font-family: Abeganshi;
  src: url(Abeganshi.ttf;);
}
@font-face {
  font-family: LadyN;
  src: url(LadyNature.ttf);
}
</style>


