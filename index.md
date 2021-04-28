---

layout: col-sidebar
title: OWASP Long Island, NY
region: North America
tags: chapter long-island long island ny new york
level: 4
type: chapter
altfooter: true
meetup-group: owaspli
country: USA
postal-code: 11735


---

Welcome to the Long Island, NY Chapter!

### A List of Donors
<ul class="no-bullets">
	<li>Educational Supporters:<a href="https://www.adelphi.edu/"><img src="/assets/images/AdelphiLogo-150x64.png" alt="Adelphi"/>Adelphi University</a></li>
	<li>Corporate Silver Supporters <a href="https://securedecisions.com/"><img src="/assets/images/200px-Secdec-logo_division.png" alt="Secure Decisions"/>Adelphi University</a></li>
</ul>

### Check our Upcoming Meetup Events:

{% include chapter_events.html group=page.meetup-group %}
<script type='text/javascript'>
  $(function(){
    $(".timeclass").hover(function() {
      utc_str = $(this).text();
      ndx = utc_str.indexOf(':');
      st_hour_str = utc_str.substring(0, ndx);
      st_min_str = utc_str.substring(ndx + 1, ndx + 3);
      utc_dt = luxon.DateTime.utc(2020, 06, 06, parseInt(st_hour_str), parseInt(st_min_str), 0);
      start_dt = utc_dt.setZone(luxon.DateTime.local().zoneName);

      ndx = utc_str.lastIndexOf(':');
      end_hour_str = utc_str.substring(ndx - 2, ndx - 1);
      end_min_str = utc_str.substring(ndx + 1, ndx + 3);
      utc_dt = luxon.DateTime.utc(2020, 06, 06, parseInt(end_hour_str), parseInt(end_min_str), 0);
      end_dt = utc_dt.setZone(luxon.DateTime.local().zoneName);
      popstr = start_dt.toLocaleString(luxon.DateTime.TIME_WITH_SECONDS) + ' to ' + end_dt.toLocaleString(luxon.DateTime.TIME_WITH_SHORT_OFFSET);
      $(this).prop('title', popstr);
    });
  });

  
</script>