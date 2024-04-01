<script>
    import profile from "$lib/assets/profile.jpeg"
</script>

<div class="wrap">
    <img alt="profile" class="shape" src={profile}>
</div>

<style>
    * {
        margin: 0;
        padding: 0;
    }

    .wrap {
        background: #000;
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .shape {
        width: 400px;
        height: 400px;
        background: linear-gradient(64.00916346799386deg, rgba(243, 72, 104,1) 23.44140625%,rgba(242, 71, 104,1) 23.44140625%,rgba(158, 0, 236,1) 79.84765625%);
        animation: wave 4.0s ease-in-out infinite;
        &:nth-of-type(2) {
            width: 800px;
            height: 800px;
            position: absolute;
            top: -200px;
            left: -400px;
            opacity: .1;
            z-index: -1;
        }
        &:nth-of-type(3) {
            width: 300px;
            height: 300px;
            position: absolute;
            bottom: -30px;
            right: 0;
            opacity: .1;
            z-index: -1;
        }
    }
    @keyframes wave {
        0%, 100% {
            border-radius: 70% 30% 72% 28% / 27% 61% 39% 73%;
        }
        50% {
            border-radius: 77% 23% 54% 46% / 40% 38% 62% 60%;
        }
    }

</style>