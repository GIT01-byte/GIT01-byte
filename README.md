<!-- ТЕМА: РАДИКАЛЬНЫЙ НЕОБРУТАЛИЗМ (КИБЕРПАНК) -->
<style>
  /* 1. Глобальный черный контейнер-рамка, изолирующий виджет от светлой/темной темы GitHub */
  .radical-box {
    background-color: #000000 !important;
    padding: 35px;
    border: 4px solid #ff0055; /* Кислотно-розовая жирная рамка */
    box-shadow: 12px 12px 0px #00f0ff; /* Циановая плоская жесткая тень */
    margin: 20px auto;
    max-width: 1080px;
  }

  /* 2. Радикальный 3D заголовок (имитация Stalinist One) */
  .radical-title {
    font-family: 'Stalinist One', 'Impact', 'Arial Black', sans-serif;
    color: #ff0055;
    text-shadow: 3px 3px 0px #00f0ff;
    text-transform: uppercase;
    font-size: 2.2rem;
    letter-spacing: 3px;
    margin-top: 0;
    margin-bottom: 30px;
    text-align: center;
    display: block;
  }

  /* 3. Настоящий CSS Grid (как в вашем оригинальном CSS) */
  .radical-grid {
    display: grid;
    grid-template-columns: repeat(2, 500px);
    grid-template-rows: repeat(2, 200px);
    gap: 20px;
    justify-content: center;
  }

  /* 4. Радикальные ховер-карточки (физические кнопки) */
  .radical-card {
    border: 3px solid #ff0055;
    background-color: #000000;
    box-shadow: 8px 8px 0px #00f0ff;
    transition: transform 0.15s ease, box-shadow 0.15s ease, border-color 0.15s ease;
    overflow: hidden;
    display: block;
    height: 100%;
  }

  /* Эффект физического вдавливания кнопки при наведении */
  .radical-card:hover {
    transform: translate(4px, 4px);
    box-shadow: 3px 3px 0px #ff0055;
    border-color: #00f0ff;
  }

  /* Позиционирование элементов в сетке */
  .card-streak {
    grid-column: 1;
    grid-row: 1;
  }

  .card-stats {
    grid-column: 1;
    grid-row: 2;
  }

  .card-langs {
    grid-column: 2;
    grid-row: 1 / 3; /* Растягивается на 2 строки в высоту */
  }

  /* Растягивание SVG-графиков внутри карточек без искажений */
  .radical-img {
    width: 100%;
    height: 100%;
    object-fit: fill;
    display: block;
    border: none;
  }

  /* 5. ПОЛНАЯ АДАПТИВНОСТЬ: перестроение сетки на планшетах и мобилках */
  @media (max-width: 1100px) {
    .radical-grid {
      grid-template-columns: 1fr;
      grid-template-rows: auto;
      max-width: 500px;
      margin: 0 auto;
    }
    .card-streak, .card-stats, .card-langs {
      grid-column: 1;
      grid-row: auto;
      height: 200px;
    }
    .card-langs {
      height: 415px; /* сохраняем высоту для списка языков */
    }
    .radical-box {
      padding: 20px;
      box-shadow: 6px 6px 0px #00f0ff;
    }
    .radical-title {
      font-size: 1.6rem;
    }
  }
</style>

<!-- HTML СТРУКТУРА ВНУТРИ ВАШЕГО README -->
<div class="radical-box">
  
  <!-- Заголовок -->
  <span class="radical-title">My GitHub Stats</span>

  <!-- Сетка Grid -->
  <div class="radical-grid">
    
    <!-- Карточка 1: Стрик-статистика -->
    <div class="radical-card card-streak">
      <a href="https://github.com/GIT01-byte">
        <img class="radical-img" src="https://github-readme-streak-stats.herokuapp.com/?user=GIT01-byte&stroke=ff0055&background=000000&ring=00f0ff&fire=ff0055&currStreakNum=ffffff&currStreakLabel=ff0055&sideNums=ffffff&sideLabels=00f0ff&dates=ffffff&hide_border=true" alt="Streak Stats" />
      </a>
    </div>

    <!-- Карточка 2: Топ языков -->
    <div class="radical-card card-langs">
      <a href="https://github.com/GIT01-byte">
        <img class="radical-img" src="https://github-readme-stats.vercel.app/api/top-langs/?username=GIT01-byte&langs_count=5&title_color=ff0055&text_color=ffffff&icon_color=00f0ff&bg_color=000000&hide_border=true&locale=en&custom_title=Top%20Languages&font_family=monospace" alt="Top Languages" />
      </a>
    </div>

    <!-- Карточка 3: Общая статистика коммитов -->
    <div class="radical-card card-stats">
      <a href="https://github.com/GIT01-byte">
        <img class="radical-img" src="https://github-readme-stats.vercel.app/api?username=GIT01-byte&show_icons=true&hide=&count_private=true&title_color=ff0055&text_color=ffffff&icon_color=00f0ff&bg_color=000000&hide_border=true&font_family=monospace" alt="GitHub Stats" />
      </a>
    </div>

  </div>
</div>
