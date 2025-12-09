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
</script>

<header>
    <h1>The eSafety Guidebook</h1>
    <div class="buttons">
        <div class="button-return"><i class="fa-solid fa-hand-point-up"></i></div>
        <div class="button-config"><i class="fa-solid fa-gear"></i></div>
    </div>
</header>