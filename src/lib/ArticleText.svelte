<script>
    let { children } = $props();
</script>

<div class="article-text">
    <p>
        {@render children()}
    </p>
</div>

<style>
    .article-text {
        margin: 70% auto;
        width: 70%;
        background-color: black;
        color: white;
        border: solid #8427c9 3px;
        border-radius: 20px;
        padding: 20px;
        box-shadow: 16px 16px #8aa6df;
        font: 300px;
    }
</style>
