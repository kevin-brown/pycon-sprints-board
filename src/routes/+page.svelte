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

<div class="space-y-4 lg:mx-auto lg:max-w-400">
  {#each Object.entries(openSpaceData.days) as [date, dayData]}
  {@const roomNames = Object.keys(Object.values(dayData.times)[0].rooms).toSorted((a, b) => a.split("/")[0].localeCompare(b.split("/")[0]))}
  <table class="block lg:table lg:table-auto lg:border border-black">
    <thead class="block lg:table-header-group">
      <tr class="block lg:table-row">
        <th colspan={roomNames.length + 1} class="block lg:table-cell">{date}</th>
      </tr>
      <tr class="block lg:table-row">
        <th class="hidden lg:table-cell"></th>
        {#each roomNames as room}
        <th class="lg:border odd:bg-gray-200 border-black p-1 hidden lg:table-cell">{room}</th>
        {/each}
      </tr>
    </thead>
    <tbody class="block lg:table-row-group space-y-1">
      {#each Object.entries(dayData.times) as [time, timeData]}
      <tr class="block lg:table-row">
        <th class="block border-b lg:border border-black p-1 lg:table-cell">{time}</th>
        {#each roomNames as roomName}
        {@const activity = timeData.rooms[roomName]}
        <td class="block odd:bg-gray-200 border-b lg:border border-black p-1 lg:table-cell before:content-[attr(data-room)] before:pe-1 before:font-bold lg:before:content-none" class:hidden={!activity?.name} data-room={roomName + ':'}>
          {activity?.name}
        </td>
        {/each}
      </tr>
      {/each}
    </tbody>
  </table>
  {/each}
</div>
