<script>
    import Scroller from "../lib/Scroller.svelte";
    import ArticleText from "../lib/ArticleText.svelte";
    import headshot from '../images/headshot.jpg';

document.getElementById('enterBtn').addEventListener('click', () => {
    document.getElementById('headshot').scrollIntoView({
      behavior: 'smooth'
    });
  });
</script>
<section id="headshot">
<div class= "main1">
    <Scroller layout="right">
        {#snippet sticky()}
            <img class="headshot" src={headshot} alt="Orchid Tablet"/>

        {/snippet}

        {#snippet scrolly()}
        <ArticleText >
                <h1 class = "sectHeader"> About me</h1>
                
        </ArticleText>

            <ArticleText >
                <p> </p>
                <h2 style="font-size: 18px;">
                    I am an incoming freshman at UC Berkeley as a Computer Science Major, and I plan to minor in policy. I am from Pueblo, a smaller town in southern Colorado, and a first-generation Nigerian-American. I have always had an interest in technology and healthcare; however, I am especially interested in the role of technology in making medical advancements more equitable.
                </h2>
            </ArticleText>
        <!-- <ArticleText>It's yours to create.</ArticleText> -->
        {/snippet}
    </Scroller>
</div>
</section>
<style>
    .headshot {
        width: 400px;
        height: 550px;
        border-radius: 10px;
        margin: 0px auto;
    }



.sectHeader{
    text-align: center;
    font-family: Arial, Helvetica, sans-serif;
}


</style>
