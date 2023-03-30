<script>
   import Answer from "./answer.svelte";
   
   export let number = 1;
    export let answer1 = "";
    export let answer2 = "";
    export let answer3 = "";
    export let answer4 = "";

    /** @type { "a" | "b" | "c" | "d" }*/
    export let answer = "a";

    /** @type { "a" | "b" | "c" | "d" }*/
    let selected = "a"

</script>

<div>
    <p>
        {number}. <slot />
    </p>

    <label for="q{number}a">
        <input type="radio"
        name="q{number}" 
        id="q{number}a" 
        value="a"
        bind:group={selected}
        />
        A: {answer1}
    </label>

    <label for="q{number}b">
        <input type="radio"
        name="q{number}" 
        id="q{number}b" 
        value="b"
        bind:group={selected}
        />
        B: {answer2}
    </label>

    <label for="q{number}c">
        <input type="radio"
        name="q{number}" 
        id="q{number}c" 
        value="c"
        bind:group={selected}
        />
        C: {answer3}
    </label>

    <label for="q{number}d">
        <input type="radio"
        name="q{number}" 
        id="q{number}d" 
        value="d"
        bind:group={selected}
        />
        D: {answer4}
    </label>
</div>

<Answer answer={answer == selected} />

