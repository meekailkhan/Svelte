<script>
    let normal = '<b>hello world</b>'
    let bold = '<b>again hello world</b>'
    const hack = '<a href="#" onclick="alert(\'you have been hacked\')">Click here</a>'


</script>

<div>
    <p>{normal}</p>
    <p>{@html bold}</p>
    <h2>{@html hack}</h2>
</div>