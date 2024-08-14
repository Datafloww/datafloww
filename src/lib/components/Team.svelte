<script>
	let team = [
		{
			name: 'Taha',
			mail: 'abc'
		},
		{
			name: 'Nitish',
			mail: 'abc'
		},
		{
			name: 'Rishabh',
			mail: 'abc'
		},
		{
			name: 'Misbah',
			mail: 'abc'
		}
	];
</script>

{#each team as member}
	<div class="text-center">
		<div class="avatar placeholder my-2">
			<div class="w-8 rounded-full bg-neutral text-neutral-content">
				<div>{member.name.split('')[0]}</div>
			</div>
		</div>
		<br />
		<span class="h-fit">{member.name}</span>
	</div>
{/each}
