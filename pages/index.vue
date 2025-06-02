<template>
  <div class="dahoai-wrapper container">


    <header>
      <h1>Все необходимые вам <br> инструменты ИИ.</h1>
      <NuxtLink>Начните бесплатно</NuxtLink>
      <span class="header-span"></span>
      <p>Присоединяйтесь к 7383 счастливым <br> пользователям, и их число растёт</p>
      <div class="header-ai">
        <img src="@/assets/ai/image%202.svg" alt="ai">
        <img src="@/assets/ai/image%203.svg" alt="ai">
        <img src="@/assets/ai/image%204.svg" alt="ai">
        <img src="@/assets/ai/image%205.svg" alt="ai">
        <img src="@/assets/ai/image%206.svg" alt="ai">
        <img src="@/assets/ai/image%207.svg" alt="ai">
        <img src="@/assets/ai/image%208.svg" alt="ai">
      </div>
    </header>
    <section class="plan">
      <h2>Экономьте по- <br> крупному с Daho AI</h2>
      <p>Зачем платить за несколько подписок, <br> если можно получить все за 5 долларов в месяц</p>
      <div class="plan-wrapper">
        <NuxtLink class="plan-item">
          <h3>БЕЗ Daho AI: оплата отдельно</h3>
          <p>Если вы подпишетесь на каждую услугу по отдельности, вам придется заплатить как минимум:</p>
          <ul>
            <li>
              ChatGPT <span>20$/мес</span>
            </li>
            <li>
              Gemini <span>20$/мес</span>
            </li>
            <li> Grok <span>20$/мес</span></li>
            <li> Flux <span>20$/мес</span></li>
            <li> Luma <span>20$/мес</span></li>
            <li> Midjourney <span>20$/мес</span></li>


          </ul>
          <span class="plan-item-line"></span>
          <h4>Общая стоимость <spna>100$/мес</spna></h4>
        </NuxtLink><NuxtLink class="plan-item">
        <h3>C Daho AI: все в одном!</h3>
        <p>Daho AI предоставляет вам доступ ко всем этим услугам по одной низкой цене:</p>
        <ul>
          <li>
            ChatGPT <span><img src="@/assets/check.svg" alt="check"></span>
          </li>
          <li>
            Gemini <span><img src="@/assets/check.svg" alt="check"></span>
          </li>
          <li> Grok <span><img src="@/assets/check.svg" alt="check"></span></li>
          <li> Flux <span><img src="@/assets/check.svg" alt="check"></span></li>
          <li> Luma <span><img src="@/assets/check.svg" alt="check"></span></li>
          <li> Midjourney <span><img src="@/assets/check.svg" alt="check"></span></li>


        </ul>
        <span class="plan-item-line"></span>
        <h4>Общая стоимость <spna>5$/мес</spna></h4>
      </NuxtLink>
      </div>
     <h4 class="plan-bottom-title">Выбор очевиден: платить 100$ США в месяц в другом месте или всего 5$ США в месяц с Daho AI</h4>
    <div class="plan-bottom">
      <h3>100$/мес в других местах</h3>
      <h4>5$/мес
        c Daho AI</h4>
      <h4>Экономьте 95$ в месяц и получите более 100 инструментов ИИ</h4>
    </div>
    </section>
    <section class="features">
      <h2>Все инструменты искусственного интеллекта, которые вам когда-либо понадобятся</h2>
      <p>Одна платформа для всех ваших потребностей в ИИ — текст, изображения, аудио, видео и многое другое</p>
      <div class="features-item">
        <h3> <img src="@/assets/text.svg" alt="text"> Генерация текста</h3>
        <p>Создаём разнообразный текстовый контент: статьи, рекламу и креативные материалы. Каждый текст помогает привлечь внимание, донести информацию и выделить ваш бренд.</p>
        <div class="features-item-content">
          <div class="features-item-content-btn">
            <span></span>
            <span></span>
            <span></span>
          </div>
          <div class="features-item-content-bottom">
            <img src="@/assets/f1.svg" alt="f1">
          </div>
        </div>
      </div>
      <div class="features-item">
        <h3> <img src="@/assets/img.svg" alt="text"> Генерация изображений</h3>
        <p>ИИ может создавать изображения по текстовым описаниям.</p>
        <img class="features-item-img" src="@/assets/max.svg" alt="macbook">
      </div>
      <div class="features-item features-item-last">
        <div class="features-item-last-wrapper">
          <h3> <img src="@/assets/code.svg" alt="text"> Генерация кода и пояснение</h3>
          <p>ИИ может генерировать, объяснять и отлаживать код на различных языках программирования, таких как Python, Java, C++, JavaScript и других. Это облегчает процесс разработки, позволяет быстро находить и исправлять ошибки.</p>
        </div>

        <img class="features-item-img" src="@/assets/phone.svg" alt="macbook">
      </div>
      <NuxtLink class="features-link">
        Все инструменты
      </NuxtLink>
    </section>
    <section class="coment">
      <h3>Нам доверяют более 3000 людей</h3>

      <swiper
          ref="mySwiper"
          class="coment-wrapper"
          :modules="[Autoplay]"
          :slides-per-view="3"
          :space-between="30"
          :loop="true"
          :autoplay="{ delay: 3000, disableOnInteraction: false }"
          :breakpoints="{
    0: { slidesPerView: 1 },
    768: { slidesPerView: 2 },
    1024: { slidesPerView: 3 }
  }"
          @swiper="onSwiperInit"
          @slideChange="onSlideChange"
      >
        <swiper-slide v-for="(item, index) in comments" :key="index">
          <div class="coment-item">
            <div class="coment-item-top">
              <img src="@/assets/user.svg" alt="user" />
              <h3>
                {{ item.name }}
                <span><img src="@/assets/star.svg" alt="star" /> {{ item.rating }}</span>
              </h3>
            </div>
            <p>{{ item.text }}</p>
          </div>
        </swiper-slide>
      </swiper>

      <div class="coment-bottom">
        <h3>Более простое решение</h3>
        <p>Больше не нужно платить за 9+ разных приложений! Daho AI перенесет все это домой.</p>
        <NuxtLink>Начните сейчас</NuxtLink>
      </div>

    </section>

  </div>
</template>
<script setup lang="ts">
import { ref } from 'vue'
import { Swiper, SwiperSlide } from 'swiper/vue'
import 'swiper/css'
import { Autoplay } from 'swiper/modules'
import { useHead } from '#imports'

useHead({
  title: 'Daho AI — Все ИИ-инструменты в одном месте за $5',
  meta: [
    {
      name: 'description',
      content: 'Получите доступ к более чем 100 инструментам искусственного интеллекта — текст, изображения, код, аудио и видео — всего за $5 в месяц. Daho AI заменяет ChatGPT, Midjourney, Gemini, Grok и другие сервисы.',
    },
    {
      name: 'keywords',
      content: 'Daho AI, ИИ платформа, ИИ инструменты, ChatGPT альтернатива, Midjourney, искусственный интеллект, генерация текста, генерация изображений, генерация кода, AI tools',
    },
    {
      name: 'author',
      content: 'Daho AI Team',
    },
    {
      property: 'og:title',
      content: 'Daho AI — Все ИИ-инструменты за $5 в месяц',
    },
    {
      property: 'og:description',
      content: 'Экономьте $95 каждый месяц, используя единую платформу для генерации текста, изображений, кода и многого другого. Присоединяйтесь к 7000+ пользователям!',
    },
    {
      property: 'og:image',
      content: 'https://daho.ai/logo.svg'
    },
    {
      property: 'og:type',
      content: 'website',
    }
  ],
  link: [
    {
      rel: 'icon',
      type: 'image/x-icon',
      href: '/favicon.ico'
    },
    {
      rel: 'canonical',
      href: 'https://daho.ai'
    }
  ]
})

const currentSlide = ref(0)
const totalSlides = ref(0)

const comments = ref([
  {
    name: 'Джейк Рейнольдс',
    rating: '4.5/5',
    text: 'Честно говоря, я был ошеломлён всеми подписками на ИИ... спасибо Daho AI!',
  },
  {
    name: 'Алия Ким',
    rating: '5/5',
    text: 'Daho AI заменил все мои ИИ-сервисы за $5. Это просто чудо.',
  },
  {
    name: 'Мурад Саидов',
    rating: '4.8/5',
    text: 'Удобный интерфейс, всё работает быстро и стабильно. Подписка — 🔥',
  },
  {
    name: 'Мурад Саидов',
    rating: '4.8/5',
    text: 'Удобный интерфейс, всё работает быстро и стабильно. Подписка — 🔥',
  },
  {
    name: 'Мурад Саидов',
    rating: '4.8/5',
    text: 'Удобный интерфейс, всё работает быстро и стабильно. Подписка — 🔥',
  },
  {
    name: 'Мурад Саидов',
    rating: '4.8/5',
    text: 'Удобный интерфейс, всё работает быстро и стабильно. Подписка — 🔥',
  },
])

const onSwiperInit = (swiper: any) => {
  totalSlides.value = swiper.slides.length - swiper.loopedSlides * 1
  currentSlide.value = swiper.realIndex
}

const onSlideChange = (swiper: any) => {
  currentSlide.value = swiper.realIndex
}
</script>




<style>
*{
  box-sizing: border-box;
}
header {
  width: 100%;
  display: flex;
  flex-direction: column;
  gap: 30px;
  align-items: center;
  min-height: 90vh;
}

header h1 {
  font-size: 64px;
  line-height: 80px;
  text-align: center;
  font-weight: bold;
}
.plan-bottom-title{
  font-size: 32px;
  text-align: center;
}
header a {
  text-decoration: none;
  color: #000;
  font-size: 32px;
  border: 2px solid #000000;
  width: max-content;
  border-radius: 50px;
  padding: 16px 30px;
}

header p {
  color: #000;
  font-size: 32px;
  text-align: center;
}

.header-span {
  width: 50%;

  height: 2px;
  background-color: #000000;
}

.header-ai {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 50px;
}

.header-ai img {
  width: 70px;
  height: 70px;
}
.plan{
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: start;
  margin-top: 50px;
}
.plan h2{
  font-size: 64px;
  font-weight: bold;
  text-align: center;
  line-height: 75px;
}
.plan p{
  font-size: 32px;
  text-align: center;
}
.plan-wrapper{
  width: 100%;
  display: flex;
  align-items: start;
  justify-content: space-between;
}
.plan-item{
  text-decoration: none;
  width: 48%;
  box-sizing: border-box;
  padding: 20px;
  color: #000;
  display: flex;
  flex-direction: column;
  align-items: start;
  justify-content: start;
  border: 2px solid #000;
  gap: 20px;
  border-radius: 30px;
}
.plan-item h3{
  font-size: 32px;
  font-weight: bold;
  text-align: start;
  line-height: 34px;
  margin: 0;
  padding: 0;


}
.plan-item p{
  font-size: 20px;
  font-weight: 400;
  text-align: start;
  margin: 0;
  padding: 0;
}
.plan-item ul{
  display: flex;
  flex-direction: column;
  list-style: none;

  width: 100%;
  padding: 0;
  margin: 0;
  gap: 15px;
}
.plan-item ul li{
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100%;
  font-size: 24px;
}
.plan-item ul li span img{
  width: 25px;
  height: 25px;
}
.plan-item-line{
  width: 100%;
  height: 2px;
  background-color: #000;
}
.plan-item h4{
  font-size: 32px;
  font-weight: bold;
  width: 100%;
  padding: 0;
  margin: 0;
  display: flex;
  align-items: center;
  justify-content: space-between;

}
.plan-item h4 span{
  font-weight: 400;
}
.plan-bottom {
  width: 100%;
  border: 2px solid #000;
  border-radius: 30px;
  padding: 20px;
  box-sizing: border-box;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.plan-bottom h3{

  text-decoration: line-through;
  font-size: 32px;
  font-weight: bold;
  text-align: center;

}
.plan-bottom h4{
  font-size: 32px;
  text-align: center;


}
.features{
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: start;
  margin-top: 120px;
  width: 100%;
  gap: 50px;
}

.features h2{
  font-size: 44px;
  font-weight: bold;
  text-align: center;
  margin: 0;
}
.features p{
  font-size: 32px;
  text-align: center;

}

.features-item{
  width: 100%;
  display: flex;
  flex-direction: column;
  border: 2px solid #000;
  border-radius: 30px;
  padding: 20px;
  box-sizing: border-box;
  align-items: center;

}
.features-item-last{
  flex-direction: row;
}
.features-item-img{
  width: 50%;
  margin-bottom: -20px;
}
.features-item h3{
  font-size: 44px;
  font-weight: bold;
  display: flex;
  align-items: center;
  margin: 0;
  gap: 20px;
}
.features-item p{
  font-size: 32px;
  text-align: center;

}
.features-item-content{
  width: 100%;
  display: flex;
  flex-direction: column;
  border: 2px solid #000;
  border-radius: 20px;
  overflow: hidden;
  padding: 10px;
  box-sizing: border-box;

}
.features-item-content-btn{
  display: flex;
  align-items: center;
  padding: 10px;
  gap: 10px;
}
.features-item-content-btn span{
  width: 20px;
  height: 20px;
  border-radius: 50px;
  background-color: #969696;
}
.features-item-content-bottom{
  width: 100%;
  height: 250px;
  border: 2px solid #000;
  border-radius: 15px;
  overflow: hidden;

}
.features-item-content-bottom img{
  width: 100%;
  height: 100%;
  object-fit: contain;
}

.features-item-last-wrapper{
  display: flex;
  flex-direction: column;
  align-items: start;
  justify-content: start;
}
.features-item-last-wrapper p{
  text-align: start;
}
.features-item-last-wrapper h3{
  text-align: start;
}
.features-link{
  width: 250px;
  font-size: 25px;
  font-weight: bold;
  text-align: center;
  border: 2px solid #000;
  border-radius: 15px;
  padding: 10px;
  transition: all 300ms ease-in-out;
}
.features-link:hover{
  cursor: pointer;
  background: #000;
  color: #fff;
}
.coment{
  width: 100%;
  display: flex;
  flex-direction: column;
}
.coment h3{
  font-size: 44px;
  font-weight: bold;
  text-align: center;

}
.coment-item{
  display: flex;
  font-size: 20px;
  flex-direction: column;
  border: 2px solid #000;
  border-radius: 20px;
  margin-left: 10px;
  padding: 10px;
}
.coment-item h3{
  font-size: 20px;
  display: flex;
  flex-direction: column;
  align-items: start;
}
.coment-item h3 span{
  font-weight: 400;
  font-size: 18px;
  display: flex;
  align-items: center;
  gap: 10px;
}
.coment-item p{
  font-size: 20px;
}
.coment-item h3 span img{
  width: 20px;
  height: 20px;
}
.coment-item-top{
  display: flex;
  align-items: center;
  gap: 20px;
}
.coment-wrapper {
  width: 100%;
  overflow: hidden;
}
.coment-bottom{
  width: 100%;
  border: 2px solid #000;
  border-radius: 30px;
  padding: 20px;
  margin-top: 100px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 20px;
}
.coment-bottom h3{
  font-size: 44px;
  text-align: center;
  margin: 0;

}
.coment-bottom p{
  font-size: 20px;
  text-align: center;

  margin: 0;
}
.coment-bottom a{
  text-decoration: none;
  font-size: 20px;
  border: 2px solid #000;
  border-radius: 15px;
  padding: 10px 15px;
}

@media (max-width: 1025px) {
  header h1{
    font-size: 44px;
    line-height: 64px;
  }
  header a{
    font-size: 23px;
  }
  .header-ai img{
    width: 60px;
    height: 60px;
  }
  .plan h2{
    font-size: 44px;
    line-height: 54px;
  }
  .plan p{
    font-size: 22px;
  }
  .plan-item h3{
    font-size: 25px;
  }
  .plan p{
    font-size: 18px;
  }
  .plan-item ul li{
    font-size: 18px;
  }
  .plan-item h4{
    font-size: 20px;
  }
  .plan-bottom-title {
    font-size: 24px;
  }
  .plan-bottom h4{
    font-size: 22px;
  }
  .plan-bottom h3{
    font-size: 22px;
  }
  .features h2 {
    font-size: 32px;
  }
  .features p{
    font-size: 22px;
  }
  .features-item h3{
    font-size: 20px;
  }
  .features-item-content-btn span{
    width: 15px;
    height: 15px;
  }
  .features-item-last{
    flex-direction: column;
  }
  .features-item h3 img{
    width: 40px;
    height: 40px;
  }
  }
@media (max-width: 769px) {
  header h1{
    font-size: 34px;
    line-height: 44px;
  }
  .coment h3{
    font-size: 32px;
  }
  .coment-item h3{
    font-size: 22px;
  }
  .coment-bottom p{
    font-size: 18px;
  }
  .coment-bottom a{
    font-size: 18px;
  }
  .features-link{
    font-size: 18px;
  }
  .plan-bottom{
    align-items: center;
    justify-content: center;
  }
  .navbar-right a {
    font-size: 16px;
  }
    header a{
    font-size: 18px;
    padding: 10px 21px;
  }
  header{
    align-items: center;
    justify-content: center;
  }
  .header-ai{
    flex-wrap: wrap;
  }
  .plan h2 {
    font-size: 34px;
    line-height: 44px;
    margin: 0;
  }
  .plan-wrapper{
    flex-direction: column;
    gap: 30px;
  }
  .plan-bottom{
    flex-wrap: wrap;
  }
  .plan-item{
    width: 100%;
  }
  header p{
    font-size: 20px;
  }
}
</style>