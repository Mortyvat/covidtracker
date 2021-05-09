<template>
    <div class="grid md:grid-cols-2 gap-4">
        <div class="shadow-md bg-blue-100 p-10 text-center rounded">
            <h3 class="text-3xl text-blue-900 font-bold mb-4">Případy</h3>
            <div class="text-2xl mb-4">
                <span class="font-bold">Nové:</span>
                {{stats.NewConfirmed}}
            </div><div class="text-2xl mb-4">
                <span class="font-bold">Celkem:</span>
                {{stats.TotalConfirmed}}
            </div>
        </div>
        <div class="shadow-md bg-red-100 p-10 text-center rounded">
            <h3 class="text-3xl text-blue-900 font-bold mb-4">Úmrtí</h3>
            <div class="text-2xl mb-4">
                <span class="font-bold">Nové:</span>
                {{stats.NewDeaths}}
            </div><div class="text-2xl mb-4">
                <span class="font-bold">Celkem:</span>
                {{stats.TotalDeaths}}
            </div>
        </div>
    </div>
</template>

<script>
export default{
    name: 'DataBoxes',
    props: ['stats']
}
</script>
