<template>
  <div id="app">
    <Links></Links>
    <section class="hero is-fullheight video-slide">
      <h1>Live Connected, Live Ketchikan</h1>
      <h2>Work, Play &amp; Innovate In The Last Frontier</h2>
      <hooper :autoPlay="true" :playSpeed="2000" :wheelControl="false">
      <slide>
        <video src="./assets/video/Video1.mp4" loop muted autoplay></video>
      </slide>
      <slide>
        <video src="./assets/video/Video2.mp4" loop muted autoplay></video>
      </slide>
      <slide>
        <video src="./assets/video/Video3.mp4" loop muted autoplay></video>
        <!-- <h1 class="slide">Work</h1> -->
      </slide>
      <slide>
        <video src="./assets/video/Video4.mp4" loop muted autoplay></video>
        <!-- <h1 class="slide">Work</h1> -->
      </slide>
            <slide>
        <video src="./assets/video/Video5.mp4" loop muted autoplay></video>
        <!-- <h1 class="slide">Work</h1> -->
      </slide>

      </hooper>
    </section>

    

  <!-- HEADER SECTION -->
  <section class="header-section">
    <div class="container is-fluid">
    <div class="columns">
      <div class="column is-12">
        <h1>You can work remotely, so why not do it from America’s most wildly beautiful community?
        <br>Relocate to Ketchikan, Alaska and experience total connectivity.</h1>
      </div>
    </div>
  </div>
  </section>
  <!-- ICON SECTION -->
  <section class="icon-section">
    <div class="container">
      <div class="columns">
        <!-- CULTURAL ICON -->
        <div class="column is-2">
          <div class="card is-shadowless">
            <div class="card-image">
              <img src="./assets/img/cultural_icon.svg" alt="Cultural Icon">
            </div>
            <div class="card-content">
              <h3>Unique Art Opportunities &amp; Cultural Experiences</h3>
            </div>
          </div>
        </div>
        <!-- ENERGY ICON -->
        <div class="column is-2">
          <div class="card is-shadowless">
            <div class="card-image">
              <img src="./assets/img/energy_icon.svg" alt="Energy Icon">
            </div>
            <div class="card-content">
              <h3>Affordable Renewable Energy</h3>
            </div>
          </div>
        </div>
        <!-- RECREATIONAL ICON -->
        <div class="column is-2">
          <div class="card is-shadowless">
            <div class="card-image">
              <img src="./assets/img/recreational_icon.svg" alt="Recreational Icon">
            </div>
            <div class="card-content">
              <h3>Unparalleled Recreational Activities</h3>
            </div>
          </div>
        </div>
        <!-- INTERNET ICON -->
        <div class="column is-2">
          <div class="card is-shadowless">
            <div class="card-image">
              <img src="./assets/img/internet_icon.svg" alt="Highspeed Internet Icon">
            </div>
            <div class="card-content">
              <h3>Unlimited High-Speed Internet</h3>
            </div>
          </div>
        </div>
        <!-- MEDICAL ICON -->
        <div class="column is-2">
          <div class="card is-shadowless">
            <div class="card-image">
              <img src="./assets/img/medical_icon.svg" alt="Medical Icon">
            </div>
            <div class="card-content">
              <h3>Top-Notch Medical Services & Educational Facilities</h3>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- LIVE CONNECTED VIDEO STORY -->
  <section class="section hero live-video-hero has-text-white">
    <div class="center-box">
      <a href="https://vimeo.com/278261626" data-lity><div class="play-triangle"></div></a>
      <h1>WATCH THE STORY</h1>
    </div>
  </section>
  <!-- KETCHIKAN LIVE CONNECTED SECTION -->
  <section class="live-connected">
    <div class="container is-fluid">
      <div class="columns is-multiline">
        <div class="column is-12">
          <div class="rectangle"></div>
        </div>
        <div class="column is-7" data-aos="fade-right" data-aos-duration="2000" data-delay="400">
          <h1 class="main-header">KETCHIKAN: LIVE CONNECTED</h1>
          <h6 class="sub-header">For remote workers and other tech-based entrepreneurs, Ketchikan represents a unique opportunity to live a connected lifestyle.</h6>
          <p>Living in Ketchikan means living connected:  to stunning natural beauty;
          to lightening-speed internet; to low-cost renewable energy; to unique arts and
          cultural experiences; and to excellent medical and educational facilities.</p>
          <p>Our residents enjoy an affordable and unparalleled quality of life with diverse
          economic opportunities and amazing cultural diversity in one of the world’s
          most beautiful settings for outdoor recreation.</p>
        </div>
        <div class="column is-5" data-aos="zoom-in" data-aos-duration="3000" data-aos-delay="420">
          <img src="./assets/img/ak_map.png" alt="Ketchikan Alaska Location">
        </div>
      </div>
    </div>
  </section>
  <!-- WORK PLAY HERO -->
  <section class="section hero work-play-hero">
    <h1 class="main-header has-text-white">EVERYTHING YOU NEED TO INNOVATE &amp; SUCCEED IN BOTH WORK AND PLAY - <br>LIVES HERE</h1>
  </section>
  <!-- INFUSTRUCTURE SECTION -->
  <section class="infustructure-section">
    <div class="container">
      <div class="columns">
        <div class="column is-12 has-text-white">
          <h1>Ketchikan has all of the infrastructure that tech-savvy workers need, nestled within pristine temperate rainforest and ocean. Be equally connected to the global workplace, and boundless natural beauty of the Tongass National Forest and Alexander Archipelago.</h1>
        </div>
      </div>
    </div>
  </section>
  <section class="why-is-matters">
    <div class="container">
      <div class="columns">
        <div class="column is-4 has-text-white">
          <h5>Why It Matters</h5>
          <p>
            In the <a href="#">2019 State of Remote Work</a> report, OWLlabs
            surveyed 1,202 full-time workers in the United States
            between the ages of 22 and 65. Some key findings
            about remote work include:
          </p>
        </div>
      </div>
      <div class="columns is-multiline" ref="radialProgressBars" style="margin-top: 20px"  data-aos="zoom-in" data-aos-duration="10" data-aos-delay="10">
        <div class="column is-4">
          <div>
            <apexchart type="radialBar" ref="chart1" :options="chartOptions1" :series="seriesP1"></apexchart>
            <div class="pro-number">{{pro1}}%</div>
          </div>
          <div style="text-align:center">
            77% of people said having a flexible job would allow
            them to be healthier (eat better, exercise more, etc).
          </div>
        </div>
        <div class="column is-4">
          <div>
            <apexchart type="radialBar" ref="chart2" :options="chartOptions2" :series="seriesP2"></apexchart>
            <div class="pro-number">{{pro2}}%</div>
          </div>
          <div style="text-align:center">
            86% of people said they would be less
            stressed by having a flexible job.
          </div>
        </div>
        <div class="column is-4">
          <div>
            <apexchart type="radialBar" ref="chart3" :options="chartOptions3" :series="seriesP3"></apexchart>
            <div class="pro-number">{{pro3}}%</div>
          </div>
          <div style="text-align:center">
            97% of workers say a job with flexibility would
            have huge improvement or positive impact on their
            overall quality of life. 
          </div>
        </div>
        
      </div>
    </div>
  </section>
  <!-- SECOND LIVE CONNECTED VIDEO -->
  <section class="section hero live-video-hero2 has-text-white">
    <div class="center-box">
      <a href="https://vimeo.com/278264990" data-lity><div class="play-triangle"></div></a>
      <h1>WATCH THE STORY</h1>
    </div>
  </section>
  <!-- WORK SECTION -->
  <section class="live-connected" id="work">
    <div class="container is-fluid">
      <div class="columns">
        <div class="column is-12">
          <div class="rectangle"></div>
        </div>
      </div>
      <div class="container secondcontainer">
        <div class="columns is-multiline">
          <div class="column is-12">
            <h1 class="main-header">WORK</h1>
          </div>
          <div class="column is-6" data-aos="fade-right" data-aos-duration="1000" data-aos-delay="200">
            <h5>Clean, Affordable Energy</h5>
            <p>Thanks to government investments in clean, renewable hydropower projects, Ketchikan’s residents enjoy the lowest energy costs in Alaska, paying just $0.10 per kWh – rates which are substantially lower than many places in the US, including Seattle.  The vast majority of Ketchikan’s energy comes from hydropower, making it one of the “greenest” cities in America.</p>
          </div>
          <div class="column is-6" data-aos="fade-left" data-aos-duration="1000" data-aos-delay="200">
            <h5>Air & Freight Services</h5>
            <p>Alaska Airlines provides daily jet service to and from Seattle, Juneau, and Anchorage.  Ketchikan is a 2 hour flight from Seattle-Tacoma airport, where you can catch connecting flights to hundreds of locations worldwide. Twice-weekly barge services from the Puget Sound region allows for predictable and reliable shipments of larger items at affordable rates.</p>
          </div>
          <div class="column is-6 lower-units" data-aos="fade-right" data-aos-duration="1200" data-aos-delay="400">
            <h5>World-Class Healthcare Services</h5>
            <p>Ketchikan’s hospital, operated by PeaceHealth, is a modern facility which serves as a medical service hub for the entire southern southeast Alaska region.  It’s ER, ICU, surgery, and birthing suites can handle diverse challenges.  Emergency evacuation services are provided by Guardian Flight, which puts Seattle’s world-leading healthcare facilities in easy reach.</p>
          </div>
          <div class="column is-6 lower-units" data-aos="fade-left" data-aos-duration="1200" data-aos-delay="400">
            <h5>Unlimited High-Speeds</h5>
            <p>Ketchikan residents enjoy flexible, scalable options for lightening-speed broadband, internet, and telecommunications services, made possible through fiber optic connections to the lower 48.</p>
          </div>
        </div>
      </div>
      </div>
  </section>
  <!-- PLAY HERO -->
  <section class="section hero play-hero">
  </section>
  <!-- PLAY SECTION -->
  <section class="live-connected" id="play">
    <div class="container is-fluid">
      <div class="columns">
        <div class="column is-12">
          <div class="rectangle"></div>
        </div>
      </div>
      <div class="container secondcontainer">
        <div class="columns is-multiline">
          <div class="column is-12">
             <h1 class="main-header">PLAY</h1>
          </div>
          <div class="column is-6 is-orange" data-aos="fade-right" data-aos-duration="1000" data-aos-delay="200">
            <h5>Outdoor Activities</h5>
            <p>Stand-up paddleboard through the Alexander Archipelago, take a quick run on the trails, grow out your beard and go on a mountain goat hunt, snorkel for crab and scallops, or kayak out to photograph sea otter rafts. In Ketchikan, adventures are only limited by your imagination.</p>
          </div>
          <div class="column is-6 is-orange" data-aos="fade-left" data-aos-duration="1000" data-aos-delay="200">
            <h5>Food</h5>
            <p>Ketchikan offers diverse dining experiences, varying from locally-sourced seafood and vegetables, to a variety of ethnic foods.  If you’re a coffee drinker, our local roasters have you covered.  Picky eater?  Grocery stores and other services offer specialty food shipments.  And did we mention Alaskan seafood?</p>
          </div>
          <div class="column is-6 lower-units is-orange" data-aos="fade-right" data-aos-duration="1200" data-aos-delay="400">
            <h5>Fishing</h5>
            <p>Ketchikan, known as the “salmon capital of the world,” is widely-viewed as one of the world’s premier sports fishing destinations.  Whether you are chasing trophy halibut, fly-fishing for steelhead and coho off the road system, pulling crab and shrimp pots, or simply trying to fill the freezer, amazing fishing is just minutes away. </p>
          </div>
          <div class="column is-6 lower-units is-orange" data-aos="fade-left" data-aos-duration="1200" data-delay="400">
            <h5>Culture & History</h5>
            <p>Ketchikan is a place where the Alaska Native Tlingit, Haida, and Tsimshian cultures converge. Indigenous art, language, song, dance, and food are an ever-present aspect of our community.  Local museums share the rich history of the pioneer days, replete with fish-pirates, prospectors, and even ladies of the night.</p>
          </div>
          <div class="column is-6 lower-units is-orange" data-aos="fade-right" data-aos-duration="1400" data-delay="400">
            <h5>The Arts</h5>
            <p>Ketchikan has an amazingly diverse arts scene.  From the performing arts, to ongoing gallery shows, to unbeatable opportunities for nature and wilderness photography, and beyond, there is truly something for every taste. The million cruise ship passengers which visit Ketchikan’s downtown each year create sales opportunities for local artists.  It’s no surprise that so many award-winning painters, photographers, and illustrators have put down roots in our town.</p>
          </div>
          <div class="column is-6 lower-units is-orange" data-aos="fade-left" data-aos-duration="1400" data-aos-delay="400">
            <h5>Get Around Quicker</h5>
            <p>Eliminate stressful, lengthy commutes through aggressive urban traffic. Instead, enjoy views of oceans, mountains, and forests on short, beautiful drives along Ketchikan’s scenic roadways</p>
          </div>
        </div>
      </div>
      </div>
  </section>
  <!-- INNOVATE HERO -->
  <section class="section hero innovate-hero">
  </section>
  <!-- INNOVATE SECTION -->
  <section class="live-connected" id="innovate">
    <div class="container is-fluid">
      <div class="columns">
        <div class="column is-12">
          <div class="rectangle"></div>
        </div>
      </div>
      <div class="container secondcontainer">
        <div class="columns is-multiline">
          <div class="column is-12">
            <h1 class="main-header">INNOVATE & SUCCEED</h1>
          </div>
          <div class="column is-6" data-aos="fade-right" data-aos-duration="1000" data-aos-delay="200">
            <h5>Education</h5>
            <p>Ketchikan has a well-funded school system, with modern, well-appointed K-12 facilities.  The University of Alaska Southeast’s local campus offers diverse opportunities for pursuing degrees and accreditations, building new skills, and pursuing lifetime learning.  Ketchikan’s newly-constructed library offers residents access to a wealth of knowledge, in a relaxing and beautiful environment.</p>
          </div>
          <div class="column is-6" data-aos="fade-left" data-aos-duration="1000" data-aos-delay="200">
            <h5>Perks</h5>
            <p>Yes, you really do get paid to live in Alaska — in 2017, every resident received a $1,100 Permanent Fund Dividend.  For children, this offers a great opportunity to begin saving and investing for college.  Also, don’t forget to get an Alaska Airlines credit card so you can earn a free plane ticket for your next vacation. And did we mention all the free Alaskan seafood?</p>
          </div>
          <div class="column is-6 lower-units" data-aos="fade-right" data-aos-duration="1200" data-aos-delay="400">
            <h5>Opportunity</h5>
            <p>The Ketchikan region offers diverse employment opportunities in sectors including construction, the maritime industry, fisheries, government services, and tourism. Local, state, federal, and tribal governments and non-profit organizations are a major employer for skilled professionals, as well, and offer diverse locally-based opportunities for contractors. Government contractor?  Ketchikan is a HubZone region. Or, build a partnership with one of our Alaska Native organizations, which qualify for the SBA’s 8(a) program.</p>

            <p>With one million cruise ship passengers per year, entrepreneurs in the entertainment, retail, tourism, and other sectors have access to a very large potential market. Access to high-speed internet, reliable freight and mail services, and the cheapest electricity in Alaska make Ketchikan the ideal location to launch your start-up.</p>
          </div>
          <div class="column is-6 lower-units" data-aos="fade-left" data-aos-duration="1200" data-aos-delay="400">
            <h5>Affordable Housing</h5>
            <p>As housing prices in major cities continue to soar, Ketchikan offers much more affordable alternatives.  The stereotype of Alaska being too expensive does not hold true here.</p>

          <p>Whether you want to live downtown or out of town, Ketchikan has diverse housing options that make it affordable to live a tremendously high quality of life.  As housing prices in major cities continue to soar, Ketchikan offers highly affordable alternatives.</p>
          </div>
        </div>
        <div class="columns is-multiline bar-charts" ref="barCharts" style="margin-top: 20px" data-aos="fade-right" data-aos-duration="1000" data-aos-delay="200">
          <div class="column is-4" style="text-align: center">
            <div style="text-align: center">{{series1[0].name}}</div>
            <apexchart type="bar" ref="chart4" height="400px" :options="options1" :series="series1"></apexchart>
            <div v-bind:style="{color: options1.plotOptions.bar.colors.ranges[0].color}">The Average 2 Bedroom Rental in Ketchikan is $1285}}</div>
            <div v-bind:style="{color: options1.plotOptions.bar.colors.ranges[1].color}">The Average 2 Bedroom Rental in Seattle is $2867</div>
          </div>
          <div class="column is-4" style="text-align: center">
            <div style="text-align: center">{{series2[0].name}}</div>
            <apexchart type="bar" ref="chart5" height="400px" :options="options2" :series="series2"></apexchart>
            <div v-bind:style="{color: options2.plotOptions.bar.colors.ranges[0].color}">The Average Home Price in Ketchikan is $290000</div>
            <div v-bind:style="{color: options3.plotOptions.bar.colors.ranges[1].color}">The Average Home Price in Seattle is $720000</div>
          </div>
          <div class="column is-4" style="text-align: center">
            <div >{{series3[0].name}}</div>
            <apexchart type="bar" ref="chart6" height="400px" :options="options3" :series="series3"></apexchart>
            <div v-bind:style="{color: options3.plotOptions.bar.colors.ranges[0].color}">The Average Commute time in Ketchikan is 10 Minutes</div>
            <div v-bind:style="{color: options3.plotOptions.bar.colors.ranges[1].color}">The Average Commute Time in Seattle is 48 Minutes</div>
          </div>
        </div>
       </div>
      </div>
  </section>
  <!-- IMPORTANT LINKS HERO -->
  <section class="section hero important-hero">
  </section>
  <!-- INNOVATE SECTION -->
  <section class="live-connected">
    <div class="container is-fluid">
      <div class="columns">
        <div class="column is-12">
          <div class="rectangle"></div>
        </div>
      </div>
      <div class="container secondcontainer">
        <div class="columns is-multiline">
          <div class="column is-12">
            <h1 class="main-header">IMPORTANT LINKS</h1>
          </div>
          <div class="column is-4 is-orange">
            <h5>Local Governments</h5>
            <a href="https://www.ktn-ak.us/" target="_blank"><p style="text-decoration: underline;">Offical Website of The City of Ketchikan</p></a>
          <a href="https://www.borough.ketchikan.ak.us/" target="_blank"><p style="text-decoration: underline;">Offical Website of Ketchikan Gateway Borough</p></a>
          </div>
          <div class="column is-4 is-orange is-visitors">
            <h5>Visiting Information</h5>
          <a href="https://visit-ketchikan.com/" target="_blank"><p style="text-decoration: underline;">Ketchikan Visitors Bureau</p></a>
          <a href="https://www.ketchikanchamber.com/relocation-to-ketchikan-alaska" target="_blank"><p style="text-decoration: underline;">Relocate to Ketchikan</p></a>
          </div>
          <div class="column is-4 is-orange">
            <h5>Business Related</h5>
          <a href="https://www.ketchikanchamber.com/" target="_blank"><p style="text-decoration: underline;">Greater Ketchikan Chamber of Commerce</p></a>
          <a href="https://aksbdc.org/" target="_blank"><p style="text-decoration: underline;">Alaska Small Business Development Center</p></a>
          </div>
        </div>
      </div>
      </div>
  </section>
  <!-- TASK FORCE HERO -->
  <section class="section hero taskforce-hero has-text-white">
    <div class="center-box">
      <a href="https://vimeo.com/278763321" data-lity><div class="play-triangle"></div></a>
      <h1>WATCH THE STORY</h1>
    </div>
  </section>

  <!-- TASK FORCE SECTION -->
  <section class="live-connected">
    <div class="container is-fluid">
      <div class="columns">
        <div class="column is-12">
          <div class="rectangle"></div>
        </div>
      </div>
      <div class="container secondcontainer">
        <div class="columns is-multiline">
          <div class="column is-12">
            <h1 class="main-header">LIVE CONNECTED TASK FORCE</h1>
          </div>
          <div class="column is-6 is-orange">
            <h5>Mission</h5>
            <p>LiveConnected will empower Ketchikan to attract remote workers and other tech-based entrepreneurs as an ideal location to live and work electronically. </p>
            <h5 class="our-team">Our Team</h5>
            <p>The LiveConnected Task Force / Advisory Team is comprised of a dynamic group of Ketchikan residents with demonstrations in marketing, advertising, project management, administration, business, and real estate fields. </p>
          </div>
          <div class="column is-6 is-orange">
            <h5>Investors</h5>
            <p>The Ketchikan Chamber of Commerce is currently seeking investors to advance the LiveConnected project; a dynamic initiative to attract tech-based entrepreneurs and remote workers to relocate to Ketchikan.</p>

            <p>Funding will be used to implement a marketing, advertising, and recruitment campaign with an objective of attracting remote workers and tech-based entrepreneurs to relocate to Ketchikan.</p>

            <p><a href="/assets/documents/liveconnected_whitepaper.pdf" target="_blank" class="white-paper">Download our Funding Request</a></p>
          </div>
         </div>
        </div>
      </div>
  </section>


  <section class="contact-form">
    <div class="container">
      <div class="columns is-multiline">
        <div class="column is-12">
          <h3>LET’S CONNECT</h3>
          <h6>Are you interested in learning more about relocating to Ketchikan?</h6>
        </div>
        </div>
        <form action="https://formspree.io/xvoplgzw" method="POST">
          <div class="columns is-multiline">
          <div class="column is-8">
          <p>Name</p>
          </div>
          <div class="column is-4">
           <p>E-mail</p>
          </div>
          <div class="column is-4">
            <input type="text" name="First Name" placeholder="First">
          </div>
          <div class="column is-4">
            <input type="text" name="Last Name" placeholder="Last">
           </div>
           <div class="column is-4">
            <input type="email" name="_replyto" placeholder="E-mail">
           </div>
           <div class="column is-4">
             <p>How did you hear about us?</p>
           </div>
           <div class="column is-4">
             <p>What state are you currently located?</p>
           </div>
           <div class="column is-4">
             <p>What is your job industry?</p>
           </div>
           <div class="column is-4">
            <select id="hear-about" name="How Did You Hear About Us?">
              <option value="Select" selected="" disable="">Select</option>
              <option value="Google Search">Google Search</option>
              <option value="Facebook Ads">Facebook Ads</option>
              <option value="Word Of Mouth">Word Of Mouth</option>
              <option value="Other">Other</option>
            </select>
           </div>
           <div class="column is-4">
             <input type="text" name="What state are you currently located?" id="state" placeholder="State">
           </div>
           <div class="column is-4">
             <select id="job-industry" name="Job Industry">
            <option value="Select" selected="" disable="">Select</option>
            <option value="Accounting">Accounting</option>
            <option value="Advertising">Advertising</option>
            <option value="Administration">Administration</option>
            <option value="Agriculture">Agriculture</option>
            <option value="Business">Business</option>
            <option value="Construction">Construction</option>
            <option value="Education">Education</option>
            <option value="Engineering">Engineering</option>
            <option value="Finance">Finance</option>
            <option value="Healthcare">Healthcare</option>
            <option value="Investment">Investment</option>
            <option value="Logisitics">Logisitics</option>
            <option value="Management">Management</option>
            <option value="Manufacturing">Manufacturing</option>
            <option value="Natural Resources">Natural Resources</option>
            <option value="Real Estate">Real Estate</option>
            <option value="Research">Research</option>
            <option value="Retail">Retail</option>
            <option value="Sales">Sales</option>
            <option value="Start-Up">Start-Up</option>
            <option value="Transportation">Transportation</option>
            <option value="Technology">Technology</option>
            <option value="Other">Other</option>
            </select>
           </div>
           <div class="column is-8">
              <textarea name="message" placeholder="Type Your Message Here"></textarea>
            </div>
            <div class="column is-2 is-offset-2">
              <button type="submit" class="btn btn-submit">Submit</button>
            </div>
         </div>
       </form>
      </div>

  </section>

  <!-- FOOTER SECTION -->

  <footer class="chamber-footer">
    <div class="container has-text-white">
      <div class="columns">
        <div class="column is-6">
          <h3>Contact</h3>
          <p>For more information on living and working in Ketchikan</p>
          <p class="p-margin">Contact the Greater Ketchikan Chamber of Commerce</p>
          <h6>907-225-3184</h6>
          <a href="mailto: info@ketchikanchamber.com"><h6 class="h-margin">info@ketchikanchamber.com</h6></a>
          <p>Project Lead:</p>
          <p>Chelsea Goucher</p>
        </div>
        <div class="column is-6">
          <div class="columns is-multiline">
            <div class="column is-6">
              <h3>Quick Links</h3>
            <a href="#work"><p class="quick-links">Work Here</p></a>
            <a href="#play"><p class="quick-links">Play Here</p></a>
            <a href="#innovate"><p class="quick-links">Innovate & Succeed</p></a>
            <a href="/assets/documents/liveconnected_comp.pdf" target="_blank"><p class="quick-links">Comparison Sheet</p></a>
            <!-- <a href="#" class="button">DONATE</a> -->
            </div>
            <div class="column is-6 faq-footer">
            <a href="/assets/documents/liveconnected_faq.pdf" target="_blank"><p class="quick-links">FAQ'S</p></a>
              <p class="quick-links">LiveConnected Live Ketchikan Video</p>
              <p class="quick-links">Local Spotlight Video</p>
              <p class="quick-links">Local Spotlight Video</p>
              <!-- <p class="donate-text">You can dontate to the Live Connected Project to aid in Ketchiaksn economic development</p> -->
            </div>
            <div class="column is-12">
              <p class="donate-text">You can dontate to the Live Connected Project to aid in Ketchikan economic development</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>

  <!-- END FOOTER SECTION -->
  <!-- LOWER FOOTER SECTION -->
  <div class="lower-footer">
    <div class="container">
      <div class="columns">
        <div class="column is-12">
          <p class="small-footer">Copyright 2018 Greater Ketchikan Chamber of Commerce | All Rights Reserved
          Photography, Video, Web Design &amp; Development by <a href="http://www.northcreativedesign.com">North Creative Design Co., LLC</a></p>
        </div>
      </div>
    </div>
  </div>
 </div>
</template>

<script>
import { Hooper, Slide } from 'hooper';
import 'hooper/dist/hooper.css';
import Links from './components/Links';
import Vue from 'vue'
import VueApexCharts from 'vue-apexcharts'
Vue.component('apexchart', VueApexCharts)

export default {
  name: 'App',
  components: {
    Hooper,
    Slide,
    Links
  },
  data: function() {
    return {
      pro1: 77,
      pro2: 86,
      pro3: 97,
      seriesP1: [77],
      chartOptions1: {
        chart: {
          type: 'radialBar',
          offsetY: -20,
          animations: {
            enabled: true,
            easing: 'linear',
            speed: 5000,
            animateGradually: {
                enabled: true,
                delay: 50
            },
            dynamicAnimation: {
                enabled: true,
                speed: 100
            }
          }
        },
        colors: ['#114253'],
        plotOptions: {
          radialBar: {
            startAngle: -90,
            endAngle: 90,
            track: {
              background: "#e7e7e7",
              strokeWidth: '97%',
              margin: 5, // margin is in pixels
            },
            dataLabels: {
              name: {
                show: false
              },
              value: {
                offsetY: -2,
                fontSize: '22px',
                formatter: function()  {
                  return ''
                }
              }
            }
          }
        },
        labels: ['Average Results'],
      },
      seriesP2: [86],
      chartOptions2: {
        chart: {
          type: 'radialBar',
          offsetY: -20,
          animations: {
            enabled: true,
            easing: 'easeinout',
            speed: 5000,
            animateGradually: {
                enabled: true,
                delay: 550
            },
            dynamicAnimation: {
                enabled: true,
                speed: 850
            }
          }
        },
        colors: ['#69a3a9'],
        plotOptions: {
          radialBar: {
            startAngle: -90,
            endAngle: 90,
            track: {
              background: "#e7e7e7",
              strokeWidth: '97%',
              margin: 5, // margin is in pixels
            },
            dataLabels: {
              name: {
                show: false
              },
              value: {
                offsetY: -2,
                fontSize: '22px',
                formatter: function()  {
                  return ''
                }
              }
            }
          }
        },
        labels: ['Average Results'],
      },
      seriesP3: [97],
      chartOptions3: {
        chart: {
          type: 'radialBar',
          offsetY: -20,
          animations: {
            enabled: true,
            easing: 'easeinout',
            speed: 5000,
            animateGradually: {
                enabled: true,
                delay: 550
            },
            dynamicAnimation: {
                enabled: true,
                speed: 850
            }
          }
        },
        colors: ['#98521b'],
        plotOptions: {
          radialBar: {
            startAngle: -90,
            endAngle: 90,
            track: {
              background: "#e7e7e7",
              strokeWidth: '97%',
              margin: 5, // margin is in pixels
            },
            dataLabels: {
              name: {
                show: false
              },
              value: {
                offsetY: -2,
                fontSize: '22px',
                formatter: function()  {
                  return ''
                }
              }
            }
          }
        },
        labels: ['Average Results'],
      },
      options1: {
        chart: {
          toolbar: {
            show: false
          },
          animations: {
            enabled: true,
            easing: 'easeinout',
            speed: 1000,
            animateGradually: {
                enabled: true,
                delay: 550
            },
            dynamicAnimation: {
                enabled: true,
                speed: 850
            }
          }
        },
        xaxis: {
          categories: ['', ''],
          axisBorder: {
            height: 5
          }
        },
        yaxis: {
          tickAmount: 12,
          max: 3000
        },
        dataLabels: {
          enabled: false
        },
        plotOptions: {
          bar: {
            columnWidth: '30%',
            colors: {
              ranges: [
                {
                  from: 0,
                  to: 1500,
                  color: '#114253'
                },
                {
                  from: 1501,
                  to: 5000,
                  color: '#2d2d2d'
                },
              ],
            },
          }
        }
      },
      options2: {
        chart: {
          toolbar: {
            show: false
          },
          animations: {
            enabled: true,
            easing: 'easeinout',
            speed: 1000,
            animateGradually: {
                enabled: true,
                delay: 550
            },
            dynamicAnimation: {
                enabled: true,
                speed: 850
            }
          }
        },
        xaxis: {
          categories: ['', ''],
          axisBorder: {
            height: 5
          }
        },
        yaxis: {
          tickAmount: 10,
          max: 1000000
        },
        dataLabels: {
          enabled: false
        },
        plotOptions: {
          bar: {
            columnWidth: '30%',
            colors: {
              ranges: [
                {
                  from: 0,
                  to: 400000,
                  color: '#69a3a9'
                },
                {
                  from: 400001,
                  to: 5000000,
                  color: '#2d2d2d'
                },
              ],
            },
          }
        }
      },
      options3: {
        chart: {
          toolbar: {
            show: false
          },
          animations: {
            enabled: true,
            easing: 'easeinout',
            speed: 1000,
            animateGradually: {
                enabled: true,
                delay: 550
            },
            dynamicAnimation: {
                enabled: true,
                speed: 850
            }
          }
        },
        xaxis: {
          categories: ['', ''],
          axisBorder: {
            height: 5
          }
        },
        yaxis: {
          tickAmount: 10,
          max: 50
        },
        dataLabels: {
          enabled: false
        },
        plotOptions: {
          bar: {
            columnWidth: '30%',
            colors: {
              ranges: [
                {
                  from: 0,
                  to: 20,
                  color: '#98521b'
                },
                {
                  from: 21,
                  to: 500,
                  color: '#2d2d2d'
                },
              ],
            },
          }
        }
      },
      series1: [
        {
          name: 'Amounts in $US Dollars',
          data: [0, 0, 0, 1285, 2867, 0, 0, 0],
        },
      ],
      series2: [{
        name: 'Amounts in $US Dollars',
        data: [0,0 ,0, 290000, 720000, 0,0,0],
      }],
      series3: [{
        name: 'Amounts in Minutes',
        data: [0, 0,0, 10, 48, 0, 0,0]
      }],
      oldAttr:"",
      oldAttr1:"",
      timer2: null,
      timer3: null,
      timer1: null
    }    
  },
  methods: {
    onClassChange(classAttrValue) {
      const classList = classAttrValue.split(' ');
      if (classList.includes('bar-charts')) {
        if(this.oldAttr !== classAttrValue){
          this.oldAttr = classAttrValue;
          if (classList.includes('aos-animate')) {
            this.$refs.chart4.updateOptions (this.options1, true, true, true);
            this.$refs.chart5.updateOptions (this.options2, true, true, true);
            this.$refs.chart6.updateOptions (this.options3, true, true, true);
          }
        }
      } else {
        if(this.oldAttr1 !== classAttrValue){
          this.oldAttr1 = classAttrValue;
          if (classList.includes('aos-animate')) {
            this.$refs.chart1.updateOptions (this.chartOptions1, true, true, true);
            this.$refs.chart2.updateOptions (this.chartOptions2, true, true, true);
            this.$refs.chart3.updateOptions (this.chartOptions3, true, true, true);
            this.pro1=0
            this.timer1 = setInterval(()=>{
              this.pro1++;
              if(this.pro1>=this.seriesP1[0]) {
                this.pro1=this.seriesP1[0]
                clearInterval(this.timer1)
              }
            }, 21)
            this.pro2=0
            this.timer2 = setInterval(()=>{
              this.pro2++;
              if(this.pro2>=this.seriesP2[0]) {
                this.pro2=this.seriesP2[0]
                clearInterval(this.timer2)
              }
            }, 21)
            this.pro3=0
            this.timer3 = setInterval(()=>{
              this.pro3++;
              if(this.pro3>=this.seriesP3[0]) {
                this.pro3=this.seriesP3[0]
                clearInterval(this.timer3)
              }
            }, 21)
          } else {
            clearInterval(this.timer1);
            clearInterval(this.timer2);
            clearInterval(this.timer3);
          }
        }
      }
    }    
  },
  mounted() {
    this.observer = new MutationObserver(mutations => {
      for (const m of mutations) {
        const newValue = m.target.getAttribute(m.attributeName);
        this.$nextTick(() => {
          this.onClassChange(newValue, m.oldValue);
        });
      }
    });

    this.observer.observe(this.$refs.radialProgressBars, {
      attributes: true,
      attributeOldValue : true,
      attributeFilter: ['class'],
    });
    
    this.observer.observe(this.$refs.barCharts, {
      attributes: true,
      attributeOldValue : true,
      attributeFilter: ['class'],
    });
  },
  beforeDestroy() {
    this.observer.disconnect();
  }, 
};
</script>

<style lang="css" src=""></style>

<style lang="scss" src="./assets/scss/app.scss"></style>
