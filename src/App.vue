<script setup>
// import HelloWorld from './components/HelloWorld.vue'
// import TheWelcome from './components/TheWelcome.vue'

</script>

<template>
  <header class="header _flex-center-btwn ">
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <!-- <HelloWorld msg="You did it!" /> -->
      <div class="menu-item">Всего задач: 123</div>
    </div>
  </header>

  <main>
    <div class="new-task-wrap _flex-center">
      <input class="inp-txt f-el" type="text" name="" id="">
      <button class="btn f-el">Создать задачу</button>
    </div>
    <h1>Все задачи</h1>
    <div class="all-task-wrap">

      <div class="task-elem _flex-center">
        <div class="task-number">1</div>
        <div class="task-title">Создать таск менеджер на Вью </div>
        <div class="task-status">Новая</div>
        <div class="task-controls _flex-center">
          <button class="btn f-el">Редактировать</button>
          <button class="btn f-el">Удалить</button>
        </div>
      </div>

      <div class="task-elem _flex-center">
        <div class="task-number">2</div>
        <div class="task-title">Lorem ipsum dolor, sit amet consectetur </div>
        <div class="task-status">Новая</div>
        <div class="task-controls _flex-center">
          <button class="btn f-el">Редактировать</button>
          <button class="btn f-el">Удалить</button>
        </div>
      </div>

      <div class="task-elem _flex-center">
        <div class="task-number">3</div>
        <div class="task-title">Lorem ipsum dolor</div>
        <div class="task-status">Новая</div>
        <div class="task-controls _flex-center">
          <button class="btn f-el">Редактировать</button>
          <button class="btn f-el">Удалить</button>
        </div>
      </div>

    </div>
    <!-- <TheWelcome /> -->
  </main>
</template>

<style scoped>
.header {
  line-height: 1.5;
/* border-bottom: 1px solid var(--vt-c-white-mute); */
}

.logo {
  display: block;
  height: 50px;
  width: auto;
  margin: 0 auto 2rem;
}

.inp-txt {
  flex-grow: 1;
  margin-right: 1rem;
  border: 2px solid var(--vt-c-text-dark-2);
  background: transparent;
  color: var(--vt-c-text-dark-2);
  outline: none;
}
.btn {
  border: 2px solid var(--vt-c-text-dark-2);
  background: var(--vt-c-text-dark-2);
  color: var(--vt-c-indigo);
  font-weight: 700;
  transition: all ease .3s;
}
.btn:hover {
  background: var(--vt-c-divider-dark-1);
  color: var(--vt-c-text-dark-2);
  font-weight: 700;
  transition: all ease .3s;
}
.f-el {
  padding: .7rem;
  border-radius: .7rem;
}
h1 {
  margin: 2rem 0 1rem;
  color: var(--vt-c-white);
  font-weight: 700;
  font-size: 2.5rem;
}
.task-elem {
  width: 100%;
  gap: 2rem;
  padding: .5rem 0;
}
.task-number {
  font-size: 1.3rem;
  font-weight: 700;
}
.task-title {
  flex-grow: 1;
  font-size: 1.3rem;
  color: var(--vt-c-white);
}
.task-controls {
  gap: 1rem;
}
@media (min-width: 1024px) {
  .header {
    padding-bottom: var(--section-padding-y);
    /* display: flex;
    place-items: center;
    padding-right: calc(var(--section-padding-y); */
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
