<script>
    import authorPic from "$assets/author3.jpg";
</script>

<section class="landing-page-section">
    <h2 class="mb-l">Meet the Founder</h2>
    <div class="author-container">
        <div class="author-text">
            <p>
                Andrew is part of the club's Data Analytics Department, contributing to the development of advanced metrics and analytical tools to enhance team performance. Notably, he co-authored a study introducing the Expected Pass Turnovers (xPT) model, which evaluates possession retention from player-passing events in football. This model analyzes event and positional data from matches to assess the probability of pass turnovers, providing valuable insights for performance analysis  

            </p>
            <p>
                Andrew has contributed to research in sports science, including the development of the xPT model for analyzing turnovers from passing events in football. 


            </p>
        </div>
        <img src={authorPic} alt="Andrew Peters" />
    </div>
</section>

<style>

.author-container {
    display: flex;
    justify-content: space-between;
}

.author-container img {
    width: 40%;
    border: 6px solid black;
    box-shadow: 0 4px 24px rgba(0, 0, 0, 0.5);
}

.author-text {
    width: 55%;
}
</style>