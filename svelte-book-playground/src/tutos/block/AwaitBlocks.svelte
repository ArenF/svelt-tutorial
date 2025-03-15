<script>
    let promise = new Promise((resolve, reject) => {
        setTimeout(() => resolve('3초 경과'), 3000);
    })
</script>

{#await promise}
    <p>Promise의 resolve 대기중</p>
{:then message} 
    <p>{message}</p>
{/await}