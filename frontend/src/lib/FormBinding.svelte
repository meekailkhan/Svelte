<script>
    let formValues = {
        name : "",
        profileInfo : "",
        country : "",
        jobLocation : []
    };

</script>

<div>
    <p>{JSON.stringify(formValues,null,3)}</p>  
    <form action="">
        <div>
            <label for="name">Name</label>
            <input type="text" bind:value={formValues.name}>
        </div>
        <div>
            <label for="profileInfo">Profile</label>
            <textarea name="" id="" bind:value={formValues.profileInfo}></textarea>
        </div>
        <div>
            <label for="country">Country</label>
            <select name="" id="country" bind:value={formValues.country}>
                <option value="">Select A Country</option>
                <option value="India">India</option>
                <option value="Saudi">Saudi</option>
                <option value="Switzerland">Switzerland</option>
            </select>
        </div>
        <div>
            <label for="Job Location">Job Location</label>
            <select name="" id="location" bind:value={formValues.jobLocation} multiple>
                <option value="">Select A Job Location</option>
                <option value="India">India</option>
                <option value="Saudi">Saudi</option>
                <option value="Switzerland">Switzerland</option>
            </select>
        </div>
    </form>
</div>