# coming-soon
This is a single page site using HTML, Vanilla Javascript and CSS designed to create a countdown timer. It counts down the seconds, minutes, hours, and days from specific initial values and updates HTML elements with the remaining time. It uses the `setInterval` function to repeatedly execute a function every 1000 milliseconds (1 second) to update the countdown.

Here's a breakdown of how the code works:

1. It selects HTML elements with classes `.seconds .number`, `.minutes .number`, `.hours .number`, and `.days .number` using the `document.querySelector` method and assigns them to variables: `seconds`, `minutes`, `hours`, and `days`.

2. It initializes variables `secValue`, `minValue`, `hourValue`, and `dayValue` with specific initial values (11 seconds, 2 minutes, 2 hours, and 9 days).

3. It sets up a `setInterval` function that executes a callback function every 1000 milliseconds (1 second).

4. Inside the callback function:
   - It decrements `secValue` by 1.
   - It checks if `secValue` reaches 0 and if so, decrements `minValue` by 1 and resets `secValue` to 60 (for seconds).
   - It repeats similar logic for minutes, hours, and days, decrementing values and resetting when necessary.
   - If `dayValue` reaches 0, it clears the interval, effectively stopping the countdown.

5. It updates the text content of the selected HTML elements (`seconds`, `minutes`, `hours`, and `days`) with the updated values, formatting them to have leading zeros if they are less than 10.

This code essentially creates a countdown timer that starts from the specified initial values and counts down until it reaches 0 days, at which point the timer stops.
