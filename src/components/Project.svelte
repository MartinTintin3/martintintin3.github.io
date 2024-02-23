<script>
    /** @type {string} */
    export let image_url;
    /** @type {string} */
    export let title;
    /** @type {string | undefined} */
    export let description = undefined;
    /** @type {string} */
    export let link;
</script>

<div class="project">
    <img class="project-img" src="{image_url}" alt="{title}">
    <div class="project-info">
        <a href={link} target="_black" class="project-title">{title}</a>
        <div class="project-description">
            {#if description}
                {description}
            {:else}
                <slot />
            {/if}
        </div>
    </div>
</div>

<style>
    .project {
        text-align: center;
        padding: 20px;
        margin-top: 25px;
        margin-bottom: 25px;
        border: 2px solid #000;
        display: inline-flex;
        width: 400px;
    }

    .project .project-img {
        float: left;
        width: 100px;
        height: 100px;
        border: 0.5px solid black;
    }

    .project .project-info {
        text-align: left;
        margin-left: 20px;
        display: flex;
        flex-direction: column;
        justify-content: flex-start;
        gap: 10px;
    }

    .project .project-title {
        font-size: 20px;
        font-weight: bold;
    }
</style>