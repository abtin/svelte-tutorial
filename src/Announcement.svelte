<script>
    let show = true;

    const hideAnnouncement = () => {
        show = false;
    }

    let warning = true;

</script>

{#if show}
    <div class="alert" class:warning={warning}>
        %50 off all fruits. Sign up for more fruits.
        <button on:click={hideAnnouncement}>Hide</button>
    </div>
{/if}

<style>
    .warning {
        background-color: lightpink;
        color: darkred;
    }
</style>