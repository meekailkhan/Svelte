<script>
    let formValues = {
        name : "",
        profileInfo : "",
        country : "",
        jobLocation : [],
        remoteWork : false,
        skillSet : [],
        yearsOfExperience : ''
    };

    function submitHandler(e){
        e.preventDefault()
        console.log(formValues)
    }
</script>

<div>
    <p>{JSON.stringify(formValues,null,3)}</p>  
    <form on:submit={submitHandler} action="">
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
        <div>
            <input type="checkbox" name="" id="remote" bind:checked={formValues.remoteWork}>
            <label for="remote">Are you able to work remote</label>
        </div>
        <div>
            <label for="">Skill Set</label>
            <input type="checkbox" name="" id="html" value="html" bind:group={formValues.skillSet}>
            <label for="html">HTML</label>
            <input type="checkbox" name="" id="css" value="css" bind:group={formValues.skillSet}>
            <label for="css">CSS</label>
            <input type="checkbox" name="" id="javascript" value="javascript" bind:group={formValues.skillSet}>
            <label for="javascript">JavaScript</label>
        </div>
        <div>
            <label for="">Year's Of Experince</label>
            <input type="radio" name="" id="0-2" value="0-2" bind:group={formValues.yearsOfExperience}>
            <label for="0-2">0-2</label>
            <input type="radio" name="" id="2-4" value="2-4" bind:group={formValues.yearsOfExperience}>
            <label for="2-4">2-4</label>
            <input type="radio" name="" id="4-6" value="4-6" bind:group={formValues.yearsOfExperience}>
            <label for="4-6">4-6</label>
            <input type="radio" name="" id="6-8" value="6-8" bind:group={formValues.yearsOfExperience}>
            <label for="8-10">8-10</label>
            <input type="radio" name="" id="8-10" value="8-10" bind:group={formValues.yearsOfExperience}>
            <label for="8-10">8-10</label>
            <input type="radio" name="" id="10+" value="10+" bind:group={formValues.yearsOfExperience}>
            <label for="10+">10+</label>

        </div>
        <div>
            <button type="submit">Submit</button>
        </div>
    </form>
</div>