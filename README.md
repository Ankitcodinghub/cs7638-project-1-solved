# cs7638-project-1-solved
**TO GET THIS SOLUTION VISIT:** [CS7638 Project 1 Solved](https://www.ankitcodinghub.com/product/cs-7638-artificial-intelligence-for-robotics-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;121148&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS7638 Project 1 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Solar System (Particle Filter) Project

Project Description

The goal of this project is to give you practice implementing a particle filter used to localize a man-made satellite in a solar system. After completing an intergalactic mission, it’s time for you to return home. Your satellite is warped through a wormhole and released into your home solar system in perfect circular orbit around the sun. The satellite receives measurements of the magnitude of the collective gravitation pull of the planets in the solar system. Note that this measurement does NOT include the gravitational effects of the sun. Although the gravitational acceleration of other planets can be measured, curiously in your home solar system, the satellite and the planets follow their orbit around the sun and their motion is not affected by other planets.

Your satellite has an on-board model of the solar system that it is being dropped into.

You’ll be riding in the satellite which will exit the wormhole somewhere within the solar system, possibly as far off as +/- 4 AU in both X and Y, and it will be ejected into circular counter-clockwise orbit around the sun, which is located at (0,0).

The planets in the solar system are also orbiting counter-clockwise around the sun in circular or elliptical orbits.

You also have at most 300 days to locate yourself and the satellite before food and resources run out.

The gravimeter sensor [sense function] gives you a (noisy) magnitude of the sum across each planet of the gravitational acceleration on the satellite by that planet, +/- some Gaussian noise.

v = Xn G∗2Mp,

p=1 rp

where v is the gravity magnitude, n is the number of planets, G is the gravitational constant, Mp is the mass of planet p, and r is the vector from the satellite to the planet.

The solar_system.py file contains the model for the sun and planets, helper functions to initialize planets in orbit, move them in orbit, or sense the gravimeter measurement from a certain location in the solar system.

The solar_locator.py file contains two functions that you must implement, and is the only file you should submit to GradeScope.

Part A

After warping back to your home solar system, you must localize where you are. The first function is called estimate_next_pos, and must determine the next location of the satellite given its gravimeter measurement. If your estimate is less than 0.01 AU from the target satellite’s actual (x,y) position, you will succeed and the test case will end.

Note that your function is called once per day (time step), and each time your function is called, you will receive one additional data point. It is likely you will need to integrate the information from multiple calls to this function before you will be able to correctly estimate your satellite’s position. The “OTHER” variable is passed into your function and can be used to store data which you would like to have returned back to your function the next time it is called (the next day).

• Initialization

– How many particles do you need such that some cover the target satellite?

• Importance Weights

– How does the sigma parameter affect the probability density function of a gaussian distribution and the weights of the particles?

– Considering the gravimeter measurement has an inverse r-squared relationship to distance, how might using a fixed sigma vs a sigma relative to the gravimeter measurement affect your results?

• Resample

– How many particles should you keep at each timestep and what are the pros/cons to having more/less particles?

• Fuzz

– How much positional fuzzing should you have?

– What percentage of your particles should you fuzz?

• Mimic the motion of the target satellite

• Estimate

Part B

Now that you’re back in your home solar system you must send SOS messages back to your home planet, the last planet in the solar system, so that they know to come pick you up. The second function is called next_angle. The goal of this function is to set the angle to send a radio message from the satellite to your home planet. Each message you send contains part of your location and trajectory. It takes 10 messages to fully transmit this data. When your home planet receives your messages they will send a team out to retrieve you and your satellite. The test will end once your home planet has received 10 messages.

Your two functions will have the same input (gravimeter), but the next_angle function will return an absolute angle from the satellite to the home planet in radians in addition to the predicted location.

Submitting your Assignment

Please refer to the “Online Grading” section of the Syllabus

Calculating your score

You will receive seven points for each successful test case, even though there are 20 test cases in total (10 in part A, 10 in part B). This means that you only need to successfully complete 15 of the 20 test cases to receive a full score on this assignment. Your maximum score will be capped at 101, although if you are able to solve more than 15 test cases you can brag about it.

Testing Your Code

NOTE: The test cases in this project are subject to change.

We have provided you a sample of 10 test cases where the first two test cases are easier than the actual test cases you will be graded with because they have no measurement noise.

These test cases are designed to allow you to test an aspect of the simulation. Test cases 3-10 are more representative of the test cases that will be used to grade your project.

To run the provided test cases on the terminal: python testing_suite_full.py We will grade your code with 10 different “secret” test cases that are similar, but not an exact match to any of the publicly provided test cases. These “secret” test cases are generated using the generate_params_planet.py file that we have provided to you. You are encouraged to make use of this file to generate additional test cases to test your code.

We have provided a testing suite similar to the one we’ll be using for grading the project, which you can use to ensure your code is working correctly. These testing suites are NOT complete as given to you, and you will need to develop other test cases to fully validate your code. We encourage you to share your test cases (only) with other students on Ed.

Frequently Asked Questions (F.A.Q.) • Q How can I simplify this problem to make thinking about it easier?

– A Take a look at this video that uses a particle filter to solve a 1D problem that has a lot of similarities to this one: Particle Filter explained without equations https://www.youtube.com/watch?v=aUkBa1zMKv4

• Q Are you SURE this can be solved using a particle filter?

– A Yes. See https://mediaspace.gatech.edu/media/t/1_c1f99rxe

• Q What is fuzzing?

– A Fuzzing is the process of perturbing (a percentage of) the particles with the intention of diversifying your hypotheses (covering a wider search area). Fuzzing is also known as dithering or roughening (sometimes called jittering). It is discussed in these papers: Sample Impoverishment, PF: Tutorial, Roughening Methods

• Q Why is my local score different from my Gradescope score?

• Q Why do I get different results locally when the visualization is on vs off?
