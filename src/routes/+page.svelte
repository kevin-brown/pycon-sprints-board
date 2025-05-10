<script lang="ts">
  type OpenSpaceData = {
    days: {
      [key: string]: DayData,
    }
  }

  type DayData = {
    times: {
      [key: string]: TimeData,
    }
  }

  type TimeData = {
    rooms: {
      [key: string]: ActivityData,
    }
  }

  type ActivityData = {
    name: string,
    mastodon?: string,
  }

  import * as openSpaceJson from "../lib/open-spaces.2024.json"

  let openSpaceData: OpenSpaceData = openSpaceJson
</script>

{#each Object.entries(openSpaceData.days) as [date, dayData]}
{@const roomNames = Object.keys(Object.values(dayData.times)[0].rooms).toSorted((a, b) => a.split("/")[0].localeCompare(b.split("/")[0]))}
<table class="table-auto border border-black">
  <thead>
    <tr>
      <th colspan={roomNames.length + 1}>{date}</th>
    </tr>
    <tr>
      <th></th>
      {#each roomNames as room}
      <th class="border border-black p-1">{room}</th>
      {/each}
    </tr>
  </thead>
  <tbody>
    {#each Object.entries(dayData.times) as [time, timeData]}
    <tr>
      <th class="border border-black p-1">{time}</th>
      {#each roomNames as roomName}
      {@const activity = timeData.rooms[roomName]}
      <td class="border border-black p-1">
        {activity?.name}
      </td>
      {/each}
    </tr>
    {/each}
  </tbody>
</table>
{/each}
