<script lang="ts">
    // eslint-disable-next-line init-declarations
    export let id: number;
    // eslint-disable-next-line init-declarations
    export let index: number;
    // eslint-disable-next-line init-declarations
    export let user: string;
    // eslint-disable-next-line init-declarations
    export let name: string;
    // eslint-disable-next-line init-declarations
    export let score: number;
</script>

<div class="col-span-full grid grid-cols-subgrid items-center gap-3 rounded-md bg-devcamp-gray-900 p-4 shadow-sm">
    <span>{index}</span>
    <img src="https://avatars.githubusercontent.com/u/{id}" alt={name} class="aspect-square size-8 rounded" />
    <div class="flex flex-col justify-center">
        <span class="text-gray-50">{name}</span>
        <span class="text-sm text-gray-300"
            ><a target="_blank" href="https://github.com/{user}" class="hover:underline">{user}</a></span
        >
    </div>
    <span class="font-sans font-bold text-devcamp-red">{score}</span>
</div>
