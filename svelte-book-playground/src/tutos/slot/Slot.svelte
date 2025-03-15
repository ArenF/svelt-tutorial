<div class="box">
    <!-- 부모 컴포넌트에서 자유롭게 콘텐츠(DOM Element or Component)를 배치할 수 있다. -->
    <slot />
</div>

<style>
    .box {
        border: 1px solid lightgray;
        padding: 1em;
    }
</style>