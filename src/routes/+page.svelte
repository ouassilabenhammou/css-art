<script>
    import PlatenSpeler from "$lib/components/css-art/PlatenSpeler.svelte";
    import WillemII from "$lib/components/css-art/WillemII.svelte";
</script>

<div class="page-container">
    <PlatenSpeler/>
    <div class="single-container">
    <WillemII/>
    </div>
</div>




<style>
    .page-container{
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        grid-template-rows: repeat(2, 1fr);
        height: 100vh;
    }

    .single-container{
        grid-column: span 2;
    }
  
    @media (max-width: 600px) {
        .page-container{
            grid-template-columns: 1fr;
            grid-template-rows: auto;
        }
        .single-container{
            grid-column: span 1;
        }

    }
</style>
