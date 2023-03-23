<script>
    export let number = 1;

    export let answer1 = "";
    export let answer2 = "";
    export let answer3 = "";
    export let answer4 = "";
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
        />
        A: {answer1}
    </label>

    <label for="q{number}b">
        <input type="radio"
        name="q{number}" 
        id="q{number}b" 
        value="b"
        />
        B: {answer2}
    </label>

    <label for="q{number}c">
        <input type="radio"
        name="q{number}" 
        id="q{number}c" 
        value="c"
        />
        C: {answer3}
    </label>

    <label for="q{number}d">
        <input type="radio"
        name="q{number}" 
        id="q{number}d" 
        value="d"
        />
        D: {answer4}
    </label>
</div>