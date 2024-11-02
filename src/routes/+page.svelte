<script>
  // ссылки для боксов
  const boxes = [
    { name: 'Расписание матчей', route: '/schedule' },
    { name: 'Основной состав', route: '/squad/first-team' },
    { name: 'Второй состав', route: '/squad/second-team' },
    { name: 'U21', route: '/squad/u21' },
    { name: 'U19', route: '/squad/u19' },
    { name: 'U17', route: '/squad/u17' },
    { name: 'Академия', route: '/academy' },
    { name: 'Бокс 1', route: '/other-boxes' },
    { name: 'Бокс 2', route: '/other-boxes' }
  ];
</script>

<style>
  .container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
    gap: 1rem;
    padding: 1rem;
  }

  .box {
    padding: 1rem;
    background-color: #ddd;
    border-radius: 8px;
    text-align: center;
    cursor: pointer;
    transition: background-color 0.3s ease;
  }

  .box:hover {
    background-color: #bbb;
  }
</style>

<div class="container">
  {#each boxes as box}
    <a href={box.route} class="box">{box.name}</a>
  {/each}
</div>
