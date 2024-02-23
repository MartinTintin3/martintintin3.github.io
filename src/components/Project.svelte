<script>
    /** @type {string} */
    export let background_url;
    /** @type {string} */
    export let title;
    /** @type {string} */
    export let description;
    /** @type {string} */
    export let link;
</script>

<div class="project">
    <h2>{title}</h2>
    <p>{description}</p>
    <a href={link}>View project</a>
</div>

<style>
    .project {
        background: url({background_url});
        background-size: cover;
        padding: 20px;
        border-radius: 5px;
        border: 1px solid #000;
    }
</style>