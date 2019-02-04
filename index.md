---
layout: workshop      # DON'T CHANGE THIS.
root: .               # DON'T CHANGE THIS EITHER.  (THANK YOU.)
carpentry: "dc"    # what kind of Carpentry (must be either "dc" or "swc")
venue: "UKZN Big Data & Informatics / RCCPII"        # brief name of host site without address (e.g., "Euphoric State University")
address: "UKZN, Exact Venue TBC"      # full street address of workshop (e.g., "Room A, 123 Forth Street, Blimingen, Euphoria")
country: "za"      # lowercase two-letter ISO country code such as "fr" (see https://en.wikipedia.org/wiki/ISO_3166-1)
language: "en"     # lowercase two-letter ISO language code such as "fr" (see https://en.wikipedia.org/wiki/ISO_639-1)
latlng: "-29.8674172,30.9785332"       # decimal latitude and longitude of workshop venue (e.g., "41.7901128,-87.6007318" - use http://www.latlong.net/)
humandate: "18 - 20 March 2019"    # human-readable dates for the workshop (e.g., "Feb 17-18, 2020")
humantime: "8:30 am - 17:00 pm (13:00 pm)"    # human-readable times for the workshop (e.g., "9:00 am - 4:30 pm")
startdate: 2019-03-18      # machine-readable start date for the workshop in YYYY-MM-DD format like 2015-01-01
enddate: 2019-03-20        # machine-readable end date for the workshop in YYYY-MM-DD format like 2015-01-02
instructor: ["Malvika Sharan", "Katrin Tirok", "Saymore Chifamba", "Samar Elsheikh"] # boxed, comma-separated list of instructors' names as strings, like ["Kay McNulty", "Betty Jennings", "Betty Snyder"]
helper: ["TBC"]     # boxed, comma-separated list of helpers' names, like ["Marlyn Wescoff", "Fran Bilas", "Ruth Lichterman"]
contact: ["katrintirok@gmail.com"]    # boxed, comma-separated list of contact email addresses for the host, lead instructor, or whoever else is handling questions, like ["marlyn.wescoff@example.org", "fran.bilas@example.org", "ruth.lichterman@example.org"]
etherpad:      http://pad.carpentries.org/2019-03-18-UKZN-ttt       # optional: URL for the workshop Etherpad if there is one
eventbrite:           # optional: alphanumeric key for Eventbrite registration, e.g., "1234567890AB" (if Eventbrite is being used)
---

<!-- See instructions in the comments below for how to edit specific sections of this workshop template. -->


<div>
<table>

	<tr>
	<td align="center" style="background-color:white" style="width:30%"><a href="https://www.ukzn.ac.za"><img style="display:block;" src="./fig/BigDataInformatics.png" alt="UKZN Big Data and Informatics"></a></td>
	<td align="center" style="background-color:white" style="width:30%"><a href="https://tenet-rccpii.github.io/rccpii-2018/"><img style="display:block;" src="./fig/dhet_logo.png" alt="DHET RCCP II"></a></td>
	</tr>
</table>

</div>

<!--
  HEADER

  Edit the values in the block above to be appropriate for your workshop.
  If the value is not 'true', 'false', 'null', or a number, please use
  double quotation marks around the value, unless specified otherwise.
  And run 'tools/check' *before* committing to make sure that changes are good.
-->

<!--
  EVENTBRITE

  This block includes the Eventbrite registration widget if
  'eventbrite' has been set in the header.  You can delete it if you
  are not using Eventbrite, or leave it in, since it will not be
  displayed if the 'eventbrite' field in the header is not set.
-->
{% if page.eventbrite %}
<iframe
  src="https://www.eventbrite.com/tickets-external?eid={{page.eventbrite}}&ref=etckt"
  frameborder="0"
  width="100%"
  height="248px"
  scrolling="auto">
</iframe>
{% endif %}

<h2 id="general">General Information</h2>

<!--
  INTRODUCTION

  Edit the general explanatory paragraph below if you want to change
  the pitch.
-->

<p>
  The course is aimed at everyone who is
  interested in becoming a better teacher. In particular, this training
  is aimed at those who want to become <a href="{{ site.swc_site }}">Software Carpentry</a>,
  <a href="{{ site.dc_site }}">Data Carpentry</a>, and <a href="{{ site.lc_site }}">Library Carpentry</a>
  instructors, run workshops and contribute to the Carpentry training
  materials. You don't currently have to be an instructor or a
  teacher to attend this workshop, but you do need to be willing and
  committed to becoming one and to improving your teaching techniques.
</p>

<p>
  The workshop is a mix of lectures and hands-on lessons where you
  practice giving a short lesson using approaches learned and
  implement some of the teaching techniques which we will discuss.
  This is training for teaching, not technical training; you do not
  need any particular technical background, and we will not be
  teaching that. This workshop is based on the constantly revised and
  updated
 <a href="{{ site.training_site }}">curriculum</a>.
</p>
<p>
  <a href="{{ site.swc_site }}">Software Carpentry</a>,
  <a href="{{ site.dc_site }}">Data Carpentry</a>, and
  <a href="{{ site.lc_site }}">Library Carpentry</a>'s mission is to
  help scientists, researchers, and librarians get more research done in less time
  and with less pain by teaching them basic lab skills for scientific
  computing.  This hands-on two-day workshop covers the basics of
  educational psychology and instructional design, and looks at how to
  use these ideas in both intensive workshops and regular classes.
</p>

<!--
  LOCATION

  This block displays the address and links to maps showing directions
  if the latitude and longitude of the workshop have been set.  You
  can use http://itouchmap.com/latlong.html to find the lat/long of an
  address.
-->
{% if page.latlng %}
<p id="where">
  <strong>Where:</strong>
  {{page.address}}.
  Get directions with
  <a href="//www.openstreetmap.org/?mlat={{page.latlng | replace:',','&mlon='}}&zoom=16">OpenStreetMap</a>
  or
  <a href="//maps.google.com/maps?q={{page.latlng}}">Google Maps</a>.
</p>
{% endif %}

<p>
  <strong>Requirements:</strong> Participants should bring a laptop
  that is Internet connected and has a functioning browser.  If you
  have it, a device for recording audio and video (mobile phones and
  laptops are OK) is useful as throughout the two days, we are going
  to record one another teaching in pairs or threes.  It does not have
  to be high-quality, but it should be good enough that you can
  understand what someone is saying.
</p>
<p>
  Please note that after this course is over, you will be asked to do
  three short follow-up exercises online in order to finish qualifying
  as an instructor: the details are available at
  <a href="{{ site.training_site }}/checkout/">{{ site.training_site }}/checkout/</a>.
  If you have any questions about the workshop, the reading material,
  or anything else, please get in touch.
</p>
<p align="center">
  <em>
    All participants are required to abide by The Carpentries'
    <a href="{{ site.swc_site }}/conduct/">Code of Conduct</a>.
  </em>
</p>

<p id="accessibility">
  <strong>Accessibility:</strong> We are committed to making this workshop
  accessible to everybody. If we can help making learning easier for
  you please get in touch (using contact details below).
	</p>
<!--
  The workshop organisers have checked that:
</p>
<ul>
  <li>The room is wheelchair / scooter accessible.</li>
  <li>Accessible restrooms are available.</li>
</ul>
<p>
  Materials will be provided in advance of the workshop and
  large-print handouts are available if needed by notifying the
  organizers in advance.  If we can help making learning easier for
  you (e.g. sign-language interpreters, lactation facilities) please
  get in touch (using contact details below) and we will
  attempt to provide them.
</p>
-->


<p id = "applications">
<strong>Applications:</strong> Please register your application by completing the form available at <a href="https://goo.gl/forms/ys7XkRc6u1OHGV6H2">https://goo.gl/forms/ys7XkRc6u1OHGV6H2</a>.
Please note the two-step application process - first register your application by completing the Google Form linked above, then complete the full application available at <a href="https://amy.software-carpentry.org/forms/request_training/">https://amy.software-carpentry.org/forms/request_training/</a> using the group name "UKZN2019".
</p>

<p id = "cost">
<strong>Cost:</strong> The workshop is free of charge. Workshop costs are sponsored by UKZN's Capacity Development Programme and the DHET's Rural Campus Connectivity Project II. Participants coming from rural institutions in KwaZulu-Natal or the Eastern Cape can apply for travel sponsorship.
</p>


<p id="contact">
  <strong>Contact</strong>:
  Please email
  {% if page.contact %}
    {% for contact in page.contact %}
      {% if forloop.last and page.contact.size > 1 %}
        or
      {% else %}
        {% unless forloop.first %}
        ,
        {% endunless %}
      {% endif %}
      <a href='mailto:{{contact}}'>{{contact}}</a>
    {% endfor %}
  {% else %}
    to-be-announced
  {% endif %}
  for more information.
</p>

<hr/>

<h2 id="preparation" name="preparation">Preparation</h2>

<p>
  Please read the following before the workshop begins:
</p>
<ol>
  <li><a href="{{ site.training_site }}/papers/science-of-learning-2015.pdf">The Science of Learning</a></li>
</ol>
<p>
  Please also read through <em>one</em> episode of of the Carpentries lessons below   
  carefully, so that you can do some exercises based on it on the
  first day of the class.  An episode is one page of a lesson.
</p>

  <ul>
  <li><a href="{{ site.swc_site }}/lessons">Software Carpentry Lessons</a></li>
  <li><a href="{{ site.dc_site }}/lessons">Data Carpentry Lessons</a></li>
  <li><a href="{{ site.lc_site }}/lessons">Library Carpentry Lessons</a></li>
  </ul>


<hr/>

<h2 id="surveys">Surveys</h2>

<h3 id="pre_workshop_survey">Pre-training survey</h3>

<p>
  Before attending the workshop, please fill out <a href="{{ site.instructor_pre_survey }}{{ site.github.project_title }}">our pre-training survey</a>.
</p>

<h3 id ="post_workshop_survey">Post-training survey</h3>

<p>
  After attending the workshop, please fill out <a href="{{ site.instructor_post_survey }}{{ site.github.project_title }}"> our post-training survey</a>
</p>



<hr/>
<h2 id="schedule" name="schedule">Schedule</h2>

<div class="row">
  <div class="col-md-4">
    <h3>Day 1</h3>
    <table class="table table-striped">
    <tr> <td>08:30</td> <td>Welcome </td> </tr>
    <tr> <td>09:00</td> <td>How Learning Works </td> </tr>
    <tr> <td>10:30</td> <td>Refreshment Break</td> </tr>
    <tr> <td>11:00</td> <td>How Learning Works/ Building Teaching Skill </td> </tr>
    <tr> <td>12:30</td> <td>Lunch </td> </tr>
    <tr> <td>13:30</td> <td>Creating a Positive Learning Environment </td> </tr>
    <tr> <td>15:15</td> <td>Afternoon Break </td> </tr>
    <tr> <td>15:35</td> <td>Building Teaching Skill </td> </tr>
    <tr> <td>16:35</td> <td>Wrap-Up and Homework for Tomorrow </td> </tr>
    <tr> <td>17:00</td> <td>Finish </td> </tr>
    </table>
  </div>
  <div class="col-md-4">
    <h3>Day 2</h3>
    <table class="table table-striped">
    <tr> <td>08:30</td> <td>Welcome Back </td> </tr>
    <tr> <td>08:45</td> <td>Building Teaching Skill </td> </tr>
    <tr> <td>10:30</td> <td>Refreshment Break </td> </tr>
    <tr> <td>11:00</td> <td>Building Teaching Skill </td> </tr>
    <tr> <td>12:30</td> <td>Lunch </td> </tr>
    <tr> <td>13:30</td> <td>The Carpentries</td> </tr>
    <tr> <td>15:15</td> <td>Afternoon Break </td> </tr>
    <tr> <td>15:35</td> <td>The Carpentries </td> </tr>
    <tr> <td>16:35</td> <td>Afternoon Wrap-Up </td> </tr>
    <tr> <td>17:00</td> <td>Finish </td> </tr>
    </table>
  </div>
  <div class="col-md-4">
    <h3>Day 3</h3>
    <table class="table table-striped">
    <tr> <td>08:30</td> <td>Welcome Back </td> </tr>
    <tr> <td>08:45</td> <td>Mentoring within the Carpentries </td> </tr>
    <tr> <td>09:45</td> <td>Lesson Onboarding Sessions </td> </tr>
    <tr> <td>10:30</td> <td>Refreshment Break </td> </tr>
    <tr> <td>11:00</td> <td>Workshop Planning at your university </td> </tr>
    <tr> <td>12:30</td> <td>Lunch </td> </tr>
    <tr> <td>13:00</td> <td>Finish</td> </tr>
    </table>
  </div>
</div>


<!--

<div class="row">
  <div class="col-md-6">
    <h3>Day 1</h3>
    <table class="table table-striped">
      <tr> <td>09:00</td> <td>Welcome </td> </tr>
      <tr> <td>09:30</td> <td>How Learning Works: The Importance of Practice </td> </tr>
      <tr> <td>10:20</td> <td>How Learning Works: Expertise and Instruction </td> </tr>
      <tr> <td>11:10</td> <td>Morning Coffee </td> </tr>
      <tr> <td>11:25</td> <td>How Learning Works: Working Memory and Cognitive Load </td> </tr>
      <tr> <td>12:15</td> <td>Building Teaching Skill: Getting Feedback </td> </tr>
      <tr> <td>12:35</td> <td>Lunch </td> </tr>
      <tr> <td>13:35</td> <td>Creating a Positive Learning Environment: Motivation and Demotivation </td> </tr>
      <tr> <td>14:40</td> <td>Creating a Positive Learning Environment: Mindset </td> </tr>
      <tr> <td>15:20</td> <td>Afternoon Coffee </td> </tr>
      <tr> <td>15:35</td> <td>Building Teaching Skill: The Importance of Practice </td> </tr>
      <tr> <td>16:45</td> <td>Wrap-Up and Homework for Tomorrow </td> </tr>
      <tr> <td>17:05</td> <td>Finish </td> </tr>
    </table>
  </div>
  <div class="col-md-6">
    <h3>Day 2</h3>
    <table class="table table-striped">
      <tr> <td>09:00</td> <td>Welcome Back </td> </tr>
      <tr> <td>09:10</td> <td>Building Teaching Skill: Lesson Study </td> </tr>
      <tr> <td>10:05</td> <td>Building Teaching Skill: Live Coding </td> </tr>
      <tr> <td>11:05</td> <td>Morning Coffee </td> </tr>
      <tr> <td>11:20</td> <td>Building Teaching Skill: Performance Revised </td> </tr>
      <tr> <td>12:00</td> <td>Lunch </td> </tr>
      <tr> <td>13:00</td> <td>The Carpentries: Workshop Introductions </td> </tr>
      <tr> <td>14:10</td> <td>The Carpentries: How We Operate </td> </tr>
      <tr> <td>15:15</td> <td>Afternoon Coffee </td> </tr>
      <tr> <td>15:30</td> <td>The Carpentries: Teaching Practices </td> </tr>
      <tr> <td>16:00</td> <td>Afternoon Wrap-Up </td> </tr>
      <tr> <td>16:45</td> <td>Finish </td> </tr>
    </table>
  </div>
</div>

-->

<!--
  ETHERPAD

  At `_misc/etherpad.txt` you will find a template for the etherpad.

  Display the Etherpad for the workshop.  You can set this up in
  advance or on the first day; either way, make sure you push changes
  to GitHub after you have its URL.  To create an Etherpad, go to

      http://pad.software-carpentry.org/YYYY-MM-DD-site

  where 'YYYY-MM-DD-site' is the identifier for your workshop,
  e.g., '2015-06-10-esu'.
-->
{% if page.etherpad %}


<p id="etherpad">
  <strong>Etherpad:</strong> <a href="{{page.etherpad}}">{{page.etherpad}}</a>.
  <br/>
  We will use this Etherpad for chatting, taking notes, and sharing URLs and bits of code.
</p>
{% endif %}

<hr/>
<h2 id="materials" name="materials">Training Materials and detailed schedule</h2>

<p>
  Please see <a href="{{ site.training_site }}">this site</a> for course material.
</p>

<hr/>
