<script>
    import CharityList from "../components/CharityList.svelte";

    let title = "Charity";
    setTimeout(function () {
        title = "Donasi";
    }, 2000);

    let charities = ["Charity 1", "Charity 2", "Charity 3"];
</script>

<svelte:head>
    <link
        rel="stylesheet"
        href="https://cdn.rawgit.com/kimeiga/bahunya/css/bahunya-0.1.3.css"
    />
</svelte:head>

<h1>{title}</h1>
<CharityList {charities} />

<style>
    h1 {
        font-size: 3em;
        color: brown;
    }
</style>
