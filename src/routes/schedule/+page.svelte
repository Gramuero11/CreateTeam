<script>
    let matches = [
      { date: '2024-11-01', opponent: 'Команда A', location: 'Дома' },
      { date: '2024-11-08', opponent: 'Команда B', location: 'На выезде' }
    ];
  </script>
  
  <h1>Расписание матчей</h1>
  <ul>
    {#each matches as match}
      <li>{match.date} — {match.opponent} ({match.location})</li>
    {/each}
  </ul>
  