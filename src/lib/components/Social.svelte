<script>
    import { lazyLoad } from '$lib/utils/lazyLoad';
    import github from "$lib/assets/github.svg";
    import mail from "$lib/assets/mail.png";
    import linkedin from "$lib/assets/linkedin.png";
    import x from "$lib/assets/x.svg";
    let socials = [
                {
                    name: 'mail',
                    href: 'https://mail.google.com/mail/u/0/?view=cm&fs=1&tf=1&source=mailto&to=datafloww.in@gmail.com',
                    src: mail
                },
                {
                    name: 'github',
                    href: 'https://github.com/DataFloww',
                    src: github
                },
                {
                    name: 'x',
                    href: 'https://x.com/datafloww',
                    src: x
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
    <div class="flex flex-col items-center w-fit m-auto p-4 rounded-xl cursor-pointer hover:bg-slate-200">
        <img use:lazyLoad={social.src} class="w-7" alt={social.name}>
    </div>
</a>
{/each}
