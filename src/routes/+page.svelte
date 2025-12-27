<script>
    import PlatenSpeler from "$lib/components/css-art/PlatenSpeler.svelte";
</script>

<div class="page-container">
    <PlatenSpeler/>

</div>


<style>
 
    .page-container{
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        grid-template-rows: repeat(2, 1fr);
        height: 100vh;
    }

    @media (max-width: 600px) {
        .page-container{
            grid-template-columns: 1fr;
            grid-template-rows: repeat(2, 1fr);
        }
    }
</style>
