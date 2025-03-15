<script>
    import Slot from './Slot.svelte';
</script>

<!--
아래와 같은 내용입니다.

    <div class="box">
        <h3>Svelte</h3>
        <p>스벨트는 지금까지 없었던 UI 프레임워크</p>
    </div
    
-->

<Slot>
    <h3>Svelte</h3>
    <p>스벨트는 지금까지 없었던 UI 프레임워크</p>
</Slot>