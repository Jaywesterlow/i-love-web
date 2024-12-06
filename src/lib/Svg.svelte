<script>
	export let name = '';
</script>

{#if name == 'arrow'}
<svg width="58" height="59" viewBox="0 0 58 59" fill="none" xmlns="http://www.w3.org/2000/svg">
    <mask id="path-1-outside-1_76_367" maskUnits="userSpaceOnUse" x="0" y="0" width="58" height="59" fill="black">
    <rect fill="white" width="58" height="59"/>
    <path d="M3 27.5C3 12.3122 15.3122 0 30.5 0C45.6878 0 58 12.3122 58 27.5C58 42.6878 45.6878 55 30.5 55C15.3122 55 3 42.6878 3 27.5Z"/>
    </mask>
    <path d="M3 0H58H3ZM58 29.5323C58 45.8068 44.8068 59 28.5323 59C12.7743 59 0 46.2257 0 30.4677L6 27.5C6 40.4787 16.969 51 30.5 51C45.6878 51 58 40.4787 58 27.5V29.5323ZM28.5323 59C12.7743 59 0 46.2257 0 30.4677V29.5C0 13.2076 13.2076 0 29.5 0H30.5C16.969 0 6 12.3122 6 27.5C6 40.4787 16.969 51 30.5 51L28.5323 59ZM58 0V55V0Z" fill="url(#paint0_linear_76_367)" mask="url(#path-1-outside-1_76_367)"/>
    <path d="M17.7 39.15C16.7 39.15 15.775 38.9333 14.925 38.5C14.0917 38.0667 13.4083 37.45 12.875 36.65L13.925 35.4C14.4083 36.1 14.9667 36.6333 15.6 37C16.2333 37.3667 16.925 37.55 17.675 37.55C19.8583 37.55 20.95 36.2667 20.95 33.7V20.6H14.55V19H22.775V33.625C22.775 35.4583 22.3417 36.8333 21.475 37.75C20.625 38.6833 19.3667 39.15 17.7 39.15ZM39.42 22.5L33.22 36.5H31.76L25.56 22.5H27.16L32.52 34.66L37.92 22.5H39.42ZM47.3848 22.5L41.1848 36.5H39.7248L33.5248 22.5H35.1248L40.4848 34.66L45.8848 22.5H47.3848Z" fill="white"/>
    <defs>
    <linearGradient id="paint0_linear_76_367" x1="30.5" y1="55" x2="30.5" y2="0" gradientUnits="userSpaceOnUse">
    <stop stop-color="#797979"/>
    <stop offset="0.45" stop-color="white"/>
    </linearGradient>
    </defs>
</svg>

{:else if name == 'return'}
<svg xmlns="http://www.w3.org/2000/svg" height="60px" viewBox="0 -960 960 960" width="60px" fill="#fff"><path d="M360-240 120-480l240-240 56 56-144 144h488v-160h80v240H272l144 144-56 56Z"/></svg>
<!-- {:else if name == ''} -->
{/if}