<script>
    let firstName = "John";
    let lastName = "Doe";
    $: fullName = `${firstName} ${lastName}`
    
    let item = [
        {
            id : 1,
            name : "Samsung",
            price : 10000
        },
        {
            id : 2,
            name : "Abcdd",
            price : 43434
        },
        {
            id : 3,
            name : "fdfg",
            price : 42343
        }
    ]

    $: total = item.reduce((acc,val)=> acc + val.price,0)

</script>

<div>
    <button on:click={()=>{
        firstName = "abcde"
        lastName = "fghi"
    }}>Change Name</button>
    <h2>{firstName} {lastName}</h2>
    <h2>{fullName}</h2>

    <button on:click={()=>{
        item = [...item,{id:4,name:"abcdedd",price:434334}]
    }}>Add item</button>
    <h2>Total = {total}</h2>
</div>