<script>
    import Property from './Property.svelte';
    let buttonLabel = '전송';
    let called_user = {
        name:'yoon',
        id: 'yoon',
        bio: 'good',
    };
</script>

<Property user={called_user} label={buttonLabel}/>