# IoT Hackday 2023 Is Almost Here!

<script>
// Set the date we're counting down to
var countDownDate = new Date("Oct 07, 2023 8:00:00").getTime();

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

<style type="text/css">
.register-button:link, register-button:visited {
  background-color: green;
  color: white !important;
  font-size: 18pt;
  font-weight: bold;
  padding: 6px 12px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
}

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
## Event Date

<b>Saturday, October 7th, 2023 8 am to 6 pm</b>

The Hackday starts in: <p id="countdown-timer"></p>

<a href="https://www.eventbrite.com/e/code-savvy-iot-hackday-tickets-692503896797" class="register-button" style="color:white">Register on EventBright</a>

After you register on the EventBrite site we will notify you about matching participants with teams and registering your team.  Please sign up now so we can send you notifications about our team planning events.

## Themes for 2023

* Women in IoT
* IoT and STEM in School Curriculum
* Sustainability Projects
* Low-cost IoT MicroPython devices such as the [$6 Raspberry Pi Pico W](https://www.raspberrypi.com/news/raspberry-pi-pico-w-your-6-iot-platform/).
* Integration of low-cost [LED Fairy Lights](https://www.amazon.com/ALOVECO-Changing-Christmas-Halloween-Decorative/dp/B08TBF3DJJ) into costumes and devices

## Location

We are happy to be hosted at the same location as in our prior years.

* Minnetronix
* Energy Park in St. Paul MN
* 1635 Energy Park Dr, St Paul, MN 55108

![](img/minnetronix.png)
