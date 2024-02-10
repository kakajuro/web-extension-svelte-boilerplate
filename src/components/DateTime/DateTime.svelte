<script lang="ts">
  import { getPalette } from '../../lib/get-palette';
  import type { DayPeriod } from '../../type/index.type';

  export let date: string;
  export let time: string;
  export let period: DayPeriod = 'morning';

  const palette = getPalette(period);
</script>

<h2 class="text-red-600 font-bold">
  {date}
</h2>
<h3 class="text-red-600 font-bold">
  {time}
</h3>

<style>
  .datetime__h2 {
    margin-top: 0;
    margin-bottom: 0;
  }

  .datetime__h3 {
    margin-top: 5px;
    margin-bottom: 0;
  }
</style>
