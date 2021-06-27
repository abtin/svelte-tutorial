<script>
    let show = true;

    const hideAnnouncement = () => {
        show = false;
    }
</script>

{#if show}
    <div class="alert">
        %50 off all fruits. Sign up for more fruits.
        <button on:click={hideAnnouncement}>Hide</button>
    </div>
{/if}

<style>

</style>