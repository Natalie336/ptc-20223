<script>
	
	import Question from "../components/question.svelte";
import Score from "../components/score.svelte";

</script>

<Score />
 

<Question 
	number={1}
	answer1="First answer"
	answer2="Second Answer"
	answer3="Third answer"
	answer4="Fourth answer"
	answer="a"
	>
<div style="text-decoration: underline">
	This is my question?
</div>
</Question>

<Question 
	number={2}
	answer1="First answer"
	answer2="Second answer"
	answer3="Third answer"
	answer4="Fourth answer"
	answer="b"
	>
	<div style="text-decoration: underline">
	This is my question?
	</div>
</Question>

<Question 
	number={3}
	answer1="First answer"
	answer2="Second answer"
	answer3="Third answer"
	answer4="Fourth answer"
	answer="c"
	>
	<div style="text-decoration: underline">
	This is my question?
	</div>
</Question>

<Question 
	number={4}
	answer1="First answer"
	answer2="Second answer"
	answer3="Third answer"
	answer4="Fourth answer"
	answer="d"
	>
	<div style="text-decoration: underline">
	This is my question?
	</div>
</Question>