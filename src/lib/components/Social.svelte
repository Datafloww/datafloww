<script>
	import { lazyLoad } from '$lib/utils/lazyLoad';
	import github from '$lib/assets/github.svg';
	import mail from '$lib/assets/mail.png';
	import linkedin from '$lib/assets/linkedin.png';
	import bsky from '$lib/assets/bsky.svg';
	let socials = [
		{
			name: 'mail',
			href: 'https://mail.google.com/mail/u/0/?view=cm&fs=1&tf=1&source=mailto&to=mail@mg.datafloww.me',
			src: mail
		},
		{
			name: 'github',
			href: 'https://github.com/DataFloww',
			src: github
		},
		{
			name: 'bluesky',
			href: 'https://bsky.app/profile/datafloww.bsky.social',
			src: bsky
		},
		{
			name: 'linkedin',
			href: 'https://linkedin.com/company/datafloww',
			src: linkedin
		}
	];
</script>

{#each socials as social}
	<a href={social.href}>
		<div
			class="m-auto flex w-fit cursor-pointer flex-col items-center rounded-xl p-4 hover:bg-slate-200"
		>
			<img use:lazyLoad={social.src} class="w-7" alt={social.name} />
		</div>
	</a>
{/each}
