<script>
    let loggedIn = false;

    function toggle() {
        loggedIn = !loggedIn;
    }

    let name = null;
</script>

<!-- if 블록 -->
{#if loggedIn}
    <button on:click={toggle}>로그아웃</button>
{/if}
<!-- 
    인라인으로 표현이 가능하며
    {:else} || {:else if }
    문을 통해서 if, else if, else 문을 모두 사용할 수 있음
    속성값에서는 적용되지 않음
-->
<div>{#if name}{name}{:else}게스트{/if}님!</div>