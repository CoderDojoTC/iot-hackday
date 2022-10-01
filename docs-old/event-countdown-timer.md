# Event Countdown Timer Test

This should display a timer that counts down to the event on October 22nd, 2022.

<script>
// Set the date we're counting down to
var countDownDate = new Date("Oct 22, 2022 8:00:00").getTime();

// Update the count down every 1 second
var x = setInterval(function() {

  // Get today's date and time
  var now = new Date().getTime();

  // Find the distance between now and the count down date
  var distance = countDownDate - now;

  // Time calculations for days, hours, minutes and seconds
  var days = Math.floor(distance / (1000 * 60 * 60 * 24));
  var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
  var seconds = Math.floor((distance % (1000 * 60)) / 1000);

  // Display the result in the element with id="demo"
  document.getElementById("countdown-timer").innerHTML = days + " days " + hours + " hours "
  + minutes + " minutes and " + seconds + " seconds ";

  // If the count down is finished, write some text
  if (distance < 0) {
    clearInterval(x);
    document.getElementById("countdown-timer").innerHTML = "EXPIRED";
  }
}, 1000);
</script>

<style type="text/CSS">
#countdown-timer {
    border: solid black 2px;
    font-size: 24pt;
    font-weight: bold;
    background-color: silver;
    color: black;
    padding: 6px 12px;
    text-align: center;
    display: inline-block;
}
</style>

Event starts in: <p id="countdown-timer"></p>
