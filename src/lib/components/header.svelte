<script>
    import { onMount } from "svelte";

    onMount(() => {
        const header = document.querySelector("header");
        window.addEventListener("scroll", () => {
            if (window.scrollY > 20) {
                header?.classList.add("scrolled")
            } else {
                header?.classList.remove("scrolled")
            }
        });
    });

    function returnToTop () {
        window.scrollTo({top: 0, behavior:"smooth"})
    }

</script>

<header>
    <h1>The eSafety Guidebook</h1>
    <div class="buttons">

        <button title="Return to Top" class="button-return" on:click={returnToTop}>
            <i class="fa-solid fa-hand-point-up"></i>
        </button>
        
        <button title="Config" class="button-config">
            <i class="fa-solid fa-gear"></i>
        </button>

    </div>
</header>