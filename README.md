<!-- 
TOP SINGLE-COLUMN INTRO 
<div style="width:100%; margin-bottom:30px;">

</div>
--!>



<!-- TWO-COLUMN SECTION -->
<table width="100%" border="0" cellspacing="0" cellpadding="0"
       style="border-collapse:collapse; border:none; background-color: transparent;">
<tr style="border:none;">



<!--             -->
<!-- LEFT COLUMN -->
<!--             -->


<!-- LEFT COLUMN -->
<td width="30%" valign="top" style="border:none; padding-right:30px;">

<p align="center">
    <img src="image_carousel/me-cir2.png" width="190"/>
</p> 



<p align="center" style="font-size:14px; line-height:1.8;">
    Assistant Professor <br />
    Department of Physics <br />
    IISc Bangalore, India <br />
    ✉️ <a href="mailto:mukherjee@iisc.ac.in">mukherjee@iisc.ac.in</a><br />
    📞 +91 8022932065
</p>

<br />

  <p align="center">
    <a href="https://scholar.google.co.uk/citations?hl=en&user=M29JjtAAAAAJ" target="_blank">
      <img src="imageN/GoogleScholar.png" width="210"/>
    </a>
  </p>

  <p align="center">
    <a href="https://orcid.org/0000-0003-1942-2521" target="_blank">
      <img src="imageN/ORCID.png" width="210"/>
    </a>
  </p>

  <p align="center">
    <a href="https://www.researchgate.net/profile/Sebabrata-Mukherjee" target="_blank">
      <img src="imageN/ResearchGate1.png" width="210"/>
    </a>
  </p>

</td>




<!--             -->
<!-- RIGHT COLUMN -->
<!--             -->


<td width="75%" valign="top"
    style="border:none; padding-left:30px;">

<p>
<strong>
Welcome to our research group!
We are part of the Department of Physics at IISc Bangalore, India.
We are interested in how optical states propagate along intricately designed photonic networks.
We create such devices in our lab using femtosecond laser pulses and explore novel light-matter
interactions with incredible precision and controllability.
Find more details in the above tabs.
</strong>
</p>

<p>
Contact
<a href="https://sebabrata-mukherjee.github.io/seba.html" target="_blank">
Sebabrata Mukherjee
</a>
if you are interested in pursuing cutting-edge research in photonics,
condensed matter physics, quantum physics, and nonlinear dynamics.
</p>







<h3>Photos </h3>

<!-- Carousel Container -->
<div class="carousel-container" style="position:relative; width:100%; max-width:800px; margin:0 auto; overflow:hidden; border-radius:8px;">



  <!-- Slides -->
   <!--
   <div class="slides" style="display:flex; transition:transform 0.5s ease-in-out; width:400%;">
    <img src="image_carousel/IIScBangalore.jpeg" style="width:25%; flex-shrink:0;" />
    <img src="image_carousel/Char_setup.jpg" style="width:25%; flex-shrink:0;" />
    <img src="image_carousel/TopoAndersonPhase.jpg" style="width:25%; flex-shrink:0;" />
    <img src="image_carousel/sp_2.jpg" style="width:25%; flex-shrink:0;" />
  </div>  -->


<div class="slides" id="slides"
     style="display:flex; transition:transform 0.5s ease-in-out;">
  <img src="image_carousel/IIScBangalore.jpeg" style="width:100%; flex-shrink:0;" />
  <img src="image_carousel/Char_setup.jpg" style="width:100%; flex-shrink:0;" />
  <img src="image_carousel/TopoAndersonPhase.jpg" style="width:100%; flex-shrink:0;" />
  <img src="image_carousel/sp_2.jpg" style="width:100%; flex-shrink:0;" />
</div>




<!-- Navigation Buttons -->
  <button onclick="prevSlide()" style="position:absolute; top:50%; left:10px; transform:translateY(-50%); background-color:#fff; border:none; border-radius:50%; padding:10px; cursor:pointer;">&#10094;</button>
  <button onclick="nextSlide()" style="position:absolute; top:50%; right:10px; transform:translateY(-50%); background-color:#fff; border:none; border-radius:50%; padding:10px; cursor:pointer;">&#10095;</button>

</div>

<!-- Caption -->
<p id="carousel-caption" align="center" style="margin-top:10px; font-style:italic;">
  (source: google images)
</p>



<script>
const slides = document.getElementById("slides");
const images = slides.children;
let index = 0;

// Clone first slide for seamless looping
const firstClone = images[0].cloneNode(true);
slides.appendChild(firstClone);

const totalSlides = slides.children.length;
const captions = [
  "IISc Bangalore – Main Building",
  "Experiments: Probing Station",
  "Topological Anderson Phase Transition",
  "Topological Edge States of Photonic s-p Orbitals"
];

function updateCaption(i) {
  document.getElementById("carousel-caption").innerText =
    captions[i % captions.length];
}

function moveSlide() {
  index++;
  slides.style.transition = "transform 0.5s ease-in-out";
  slides.style.transform = `translateX(-${index * 100}%)`;
  updateCaption(index);

  // When reaching cloned slide
  if (index === totalSlides - 1) {
    setTimeout(() => {
      slides.style.transition = "none";
      index = 0;
      slides.style.transform = "translateX(0)";
    }, 500);
  }
}

// Auto-slide every 3 seconds
setInterval(moveSlide, 3000);

// Initial caption
updateCaption(0);
</script>


<!--
<script>
let currentIndex = 0;
const slides = document.querySelector('.slides');
const totalSlides = slides.children.length;

// Array of captions for each image
const captions = [
  "IISc Bangalore – Main Building",
  "Experiments: Probing Station",
  "Topological Anderson Phase Transition",
  "Topological Edge States of Photonic s-p Orbitals" 
];

function showSlide(index) {
  slides.style.transform = 'translateX(' + (-index * 100/totalSlides) + '%)';
  document.getElementById('carousel-caption').innerText = captions[index];
}

function nextSlide() {
  currentIndex = (currentIndex + 1) % totalSlides;
  showSlide(currentIndex);
}

function prevSlide() {
  currentIndex = (currentIndex - 1 + totalSlides) % totalSlides;
  showSlide(currentIndex);
}

// Initial caption
showSlide(currentIndex);

// Auto-slide every 3 seconds
setInterval(nextSlide, 3000);
</script>
-->



<!--             -->
<!--             -->

<h3>Recent News</h3>

<div style="max-height:200px; overflow-y:scroll; padding-right:10px; scrollbar-width: thin;">
  <ul>
    <li>Check out our recent work on
      <a href="https://doi.org/10.1103/9jjd-vbp1" target="_blank">Topological Anderson Transition</a>
    </li>
    <li>Check out our recent work on
      <a href="https://doi.org/10.1364/OL.546876" target="_blank">photonic s-p orbitals</a>
    </li>
    <li>Congratulations, Avinash, on winning the Poster Award at Photonics 2024, IIT Kharagpur</li>
    <li>Congratulations, Bhoomija, on winning the Poster Award at WOPI 2024, IIT Bombay</li>
    <li>Check out our recent work on
      <a href="https://doi.org/10.1364/OPTICA.494823" target="_blank">Period-doubled Floquet solitons</a> published in <em>Optica</em>
    </li>
    <li>IOE postdoc Dr. Shailja Sharma is joining our group. Welcome, Shailja!</li>
    <li>Welcome Trideb (Int. PhD) and Avinash (PhD), new members of our group!</li>
    <li>Check out our recent work on
      <a href="https://doi.org/10.1103/PhysRevX.11.041057" target="_blank"><strong>nonlinear</strong> topological edge states</a> published in <em>Physical Review X</em>
    </li>
    <li>Undergraduate student Sanjay S is joining our group. Welcome, Sanjay!</li>
    <li>Ph.D. student Gayathry R is joining our group. Welcome, Gayathry!</li>
  </ul>
</div>







<!-- end of your right column content -->
</td>
</tr>

<!-- SINGLE-COLUMN LOGO AT THE END -->
<tr>
  <td colspan="2" align="center" style="padding-top:30px; border:none; background-color: transparent;">
    <a href="https://iisc.ac.in/" target="_blank">
      <img src="imageN/Funding_logo/logo-all.png" width="600"/>
    </a>
  </td>
</tr>


