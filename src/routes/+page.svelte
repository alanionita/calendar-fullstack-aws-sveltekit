<script lang="ts">
	function returnAllDays() {
		const currentDate = new Date(); // create a new Date object with the current date
		const currentMonth = currentDate.getMonth(); // get the current month (0-11)

		const firstDay = new Date(currentDate.getFullYear(), currentMonth, 1); // get the first day of the current month
		const lastDay = new Date(currentDate.getFullYear(), currentMonth + 1, 0); // get the last day of the current month

		const daysInMonth = []; // create an empty array to store the days in the current month

		for (let day = firstDay.getDate(); day <= lastDay.getDate(); day++) {
			// loop over each day in the current month
			const date = new Date(currentDate.getFullYear(), currentMonth, day); // create a new Date object for the current day
			daysInMonth.push(date); // add the new Date object to the array
		}

		console.log(daysInMonth); // log the array of days in the current month to the console
        return daysInMonth
	}

	const days = returnAllDays();
</script>

<section class="home-grid">
	<h1 class="home-month">Month</h1>
	<ul class="home-days">
		{#each days as day}
			<li class="home-day">{`Day :: ${day}`}</li>
		{/each}
	</ul>
</section>

<style>
	.home-grid {
		display: grid;
		height: 80%;
        grid-template-columns: repeat(12, 1fr);
		gap: 1em;
        padding-top: 1rem;
		background-color: palegoldenrod;
	}
	.home-month {
        height: 100%;
		writing-mode: vertical-lr;
		grid-column-start: 1;
		grid-column-end: span 1;
	}
	.home-days {
		display: flex;
		width: 100%;
		flex-wrap: wrap;
		grid-column-start: 2;
		grid-column-end: span 11;
		list-style: none;
		padding: 0;
        margin: 0;
	}
	.home-day {
		background-color: aquamarine;
		height: var(--ui-grid-card-height);

		width: calc((100% / 7) - 16px);
		margin-right: 1rem;
	}
	.home-day:nth-child(7n) {
		background-color: red;
		margin-right: 0rem;
	}
</style>
