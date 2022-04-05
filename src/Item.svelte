<article class="item">
    <h2>
        <slot name="name">
            <span class="missing">Unknown name</span>
        </slot>
    </h2>

    <div class="comment">
        <slot name="comment" />
    </div>

    <div class="rating">
        <slot name="rating">
            <span class="missing">0</span>
        </slot>
    </div>
</article>

<style>
    .item {
        width: 100%;
        border: 1px solid #aaa;
        border-radius: 2px;
        box-shadow: 2px 2px 8px rgba(0, 0, 0, 0.1);
        padding: 1em;
    }

    h2 {
        padding: 0 0 0.2em 0;
        margin: 0 0 1em 0;
        border-bottom: 1px solid #ff3e00;
    }

    .comment,
    .rating {
        padding: 0 0 0 1.5em;
        background: 0 50% no-repeat;
        background-size: 1em 1em;
        margin: 0 0 0.5em 0;
        line-height: 1.2;
    }

    .missing {
        color: #999;
    }
</style>
