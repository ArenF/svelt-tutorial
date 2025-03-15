<script>
    // js 파일의 export와 헷갈리지 말 것
    // JS - 파일 내의 함수와 객체 등을 다른 파일에서 사용할 수 있도록 지정
    // Svelte - 변수의 값을 컴포넌트의 외부에서 설정할 수 있다는 의미
    // 여기서는 svelte의 뜻을 따라 외부에서 Property_Called.svelte에서 속성에 지정해준 label값을 통해 불러옴.
    
    export let user;
    export let label;

    // 속성이 전달되지 않으면 기본값인 false로 사용된다.
    export let disabled = false;
</script>

<h2>{user.name} (@{user.id})</h2>
<p>{user.bio}</p>

<!-- disabled 의 속성과 변수의 값이 맞으면 아래와 같이 사용 가능하다. -->
<button {disabled}>
    {label}
</button>
<!--
    위의 내용가 같다.
    <script>
    export let disabled_value = false;
    ...
    </script>

    <button disabled={disabled_value}>{label}</button>
-->
