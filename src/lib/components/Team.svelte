<script>
    let team = [
        {
            name:"Nitish",
            mail:"abc"
        },
        {
            name:"Taha",
            mail:"abc"
        },
        {
            name:"Rishabh",
            mail:"abc"
        },
        {
            name:"Misbah",
            mail:"abc"
        }
    ]
</script>

{#each team as member}
<div class="text-center">
    <div class="avatar placeholder my-2">
        <div class="bg-neutral text-neutral-content w-8 rounded-full">
          <div>{member.name.split("")[0]}</div>
        </div>
    </div>
    <br>
    <span class="h-fit">{member.name}</span>
</div>
{/each}

