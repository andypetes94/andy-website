<script>
    const chapters = [
  {
    number: 1,
    title: "Custom Dashboards",
    strapline: "Understanding Visas, Residency, and Legal Essentials",
    excerpt:
      "Interactive, real-time dashboards tailored to your business needs.",
  },
  {
    number: 2,
    title: "Data Analysis",
    strapline: "From Coastal Villas to Urban Apartments: Where and How to Live",
    excerpt: 
    "Expert analysis that reveals patterns, trends, and actionable insights.",  },
  {
    number: 3,
    title: "Tailored Solutions",
    strapline: "Strategies for Employment and Freelancing in a New Culture",
    excerpt: "Visual reports that simplify complex data for stakeholders at all levels.",
  },
  {
    number: 4,
    title: "Insightful & Impactful",
    strapline: "Cultural Norms, Social Etiquette, and Making New Connections",
    excerpt: "Not just pretty pictures, but visualizations that truly enhance decision-making.",
  },
];

let selectedChapterNumber = $state(1);
let selectedChapter = $derived(
    chapters.find((chapter) => chapter.number === selectedChapterNumber)
);

function selectChapter(chapter){ 
    selectedChapterNumber = chapter.number;
}

</script>


<section class="landing-page-section">
    <h2 class="mb-m">What we offer</h2>
    <div class="chapter-container">
        <ul>
            {#each chapters as chapter}
                <li>
                    <button
                    class="chapter-title"
                    class:selected-chapter-title={selectedChapterNumber === chapter.number}
                    aria-controls="chapter-info-{chapter.number}"
                    aria-expanded="{selectedChapterNumber === chapter.number}"
                    onclick={() => selectChapter(chapter)}
                    >
                    <h3>{chapter.title}</h3>
                    </button>
                </li>
            {/each}
        </ul>
        <div class="chapter-info">
            <h3 class="chapter-strapline italic mb-s">
                {selectedChapter.title}
            </h3>
            <p>
                {selectedChapter.excerpt}
            </p>
        </div>
    </div>
</section>


<style>


    .chapter-container {
        display: flex;
        justify-content: space-between;

    }

    .chapter-container ul {
        width: 55%;
    }

    .chapter-info {
        width: 40%;

    }

    .chapter-title {
        border-bottom: 2px solid gray;
        width: 100%;
        display: block;
        padding: 12px;
        text-align: left;
    }


    .selected-chapter-title {
        background-color: black;
        border: none;
        color: white;
        box-shadow: 
        0 12px 6px rgba(0, 0, 0, 0.1),
        0 1px 3px rgba(0, 0, 0, 0.08);
    }

</style>