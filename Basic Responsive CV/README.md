# Code Explanation

## Table of Contents
1. [Hands On Explanation](#hands-on-explanation)
2. [HTML](#1.-html)  
   + [Header](#1.1-header)
     - [Link External CSS](#1.1.1-links-external-css)
     - [Link External Fonts](#1.1.2-links-external-fonts)
     - [Include External Javascript](#1.1.3-include-external-javascript)  
   + [Body](#1.2-body)
     - [Top Section](#1.2.1-top-section)
       - [Left Section](#1.2.1-a.-top-left-section)
       - [Right Section](#1.2.1-b.-top-right-section)
     - [Bottom Section](#1.2.2-bottom-section)
       - [Left Section](#1.2.2-a.-bottom-left-section)
         - [Biodata](#biodata)
         - [Education](#education)
         - [Contact](#contact)
       - [Right Section](#1.2.2-b.-bottom-right-section)
         - [Experience](#experience)
     - [Footer](#1.3-footer)
3. [CSS](#2.-css)
   + [Scrollbar](#scrollbar)
   + [Timeline](#timeline)

## Hands On Explanation
1. Create your personal profile (Curriculum Vitae - CV) with the following requirements:
   - Utilize a basic container and grid system.
   - Include a profile picture.
   - Add a carousel for showcasing experience documentation.
   - Incorporate a table for Educational Background, Held Certifications, or Work Experience.
2. Ensure the created layout is responsive (accessible on different screen sizes).
3. Do not use templates available on the Internet.
4. Use a CSS framework such as Bootstrap, Tailwind, or Semantic UI.

## 1. HTML

### 1.1 Header
The <head> section in HTML is a crucial part of a web page. It contains meta-information about the document, as well as links to external resources like stylesheets and scripts. Let's break down the contents of this specific <head>

#### 1.1.1 Link External CSS
```
<link rel="stylesheet" href="style.css">
```
This links to a local stylesheet named style.css.
```
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/css/all.min.css">
```
This links to the Font Awesome icon library for scalable vector icons.
```
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css">
```
This links to the CSS file of the Bootstrap framework.

#### 1.1.2 Link External Fonts
```
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Nunito:wght@500&display=swap" rel="stylesheet">
```
Links to the stylesheet of the font "Nunito" with a weight of 500 from Google's font library

#### 1.1.3 Include External Javascript
```
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
```
Includes a JavaScript file from a content delivery network (CDN) provided by jsDelivr.

</br>

### 1.2 Body
In the body section, I will divide it into two parts, namely top and bottom. Then, I will further divide the top and bottom parts into right and left.

#### 1.2.1 Top Section
At the top section, I want people to get to know me in general first by providing a photo, name, and description.

#### 1.2.1 a. Top Left Section
I will create a photo in this section.
```
<div class="col-md-4 d-flex justify-content-center align-items-center profile-circle profile-container">
  <img src="picture/profilePicture.jpg" alt="profilePicture" class="img-fluid rounded-circle" width="200">
</div>
```
I made a circular-shaped photo because I prefer it.

#### 1.2.1 b. Top Right Section
"I want people to get to know me in general first by providing a photo, name, and description." Because of this, I want to place the description on the right side.
```
<h1 class="title-color"><b>Vidiawan Nabiel Arrasyid</b></h1>
<h4 class="title-color mb-1">Teknik informatika'22</h4>
<div class="pt-4">
  <p>Nama saya Vidiawan Nabiel Arrasyid. Saya memiliki beberapa pengalaman dalam organisasi, kepanitiaan, dan kompetisi. Saya dapat beradaptasi dan berpartisipasi pada kelompok dengan baik.</p>
</div>
```
In this section, I write my name, major, a brief description of my experiences, and an overall description of my character.

#### 1.2.2 Bottom Section
In this section, I will provide more detailed and comprehensive information about education, personal details, experiences, and contact information.

#### 1.2.2 a. Bottom Left Section
In this section, I will write down personal details, educational background, and contact information.

##### Biodata
```
<h2 class="custom-subtitle">Biodata</h2>
<ul class="list-unstyled ms-3">
  <li>
    <b>Tempat/Tanggal Lahir</b><br>
    *****, ** ******* ****<br>
  </li>
  <li>
    <b>Jenis Kelamin</b><br>
    Laki-laki<br>
  </li>
  <li> 
    <b>Domisili</b><br>
    <a href="https://maps.app.goo.gl/1DDPcBeXfCDFENxX6" target="_blank" class="link-style">Sukolilo, Surabaya, Jawa Timur, Indonesia<br></a>
  </li>
</ul>
```
In this section, I write down my place of birth, date of birth, gender, and current residence.

##### Education
In this education section, I've created a table as requested, and I've formatted it to resemble a timeline.
```
<h2 class="custom-subtitle">Pendidikan</h2>
<table class="ms-3 mb-2">
  <tr class="timeline-item">
    <td class="ps-4">
      <b>FIWA</b><br>
      2019-2022<br>
      IPA
    </td>
  </tr>
  <tr class="timeline-item ms-3">
    <td  class="ps-4">
      <b>ITS Surabaya</b><br>
      2022-Sekarang<br>
      Teknik Informatika
    </td>
</tr>
</table>
```
I've filled it with the name of the school/institution, the years I studied there, and the major I took.

##### Contact
In this section, I will provide my contact information that can be used to reach me.
```
<div class="d-none d-md-block contact mb-4">
```
This section will not be displayed on mobile devices and will be moved to the [footer](#1.3-footer).
```
<a href="tel:#" class="custom-contact ms-3 hover-effect"><i class="fas fa-phone me-3"></i>+62 ***-****-***</a><br>
<a href="mailto:#" class="ms-3 hover-effect"><i class="fas fa-envelope me-3"></i>*****</a><br>
<a href="#" class="ms-3 hover-effect"><i class="fab fa-line me-3"></i>*****</a><br>
<a href="#" target="_blank" class="ms-3 hover-effect"><i class="fab fa-instagram me-3"></i>*****</a>
```
For security and comfort, since this repository is public, I will hide the sensitive data.

#### 1.2.2 b. Bottom Right Section
In this section, I will list experiences accompanied by photos using a carousel as requested.
```
<div id="carouselExampleAutoplaying" class="carousel slide carousel-fade px-3 mt-3" data-bs-ride="carousel">
  <div class="carousel-indicators">
    <button type="button" data-bs-target="#carouselExampleAutoplaying" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
    <button type="button" data-bs-target="#carouselExampleAutoplaying" data-bs-slide-to="1" aria-label="Slide 2"></button>
    <button type="button" data-bs-target="#carouselExampleAutoplaying" data-bs-slide-to="2" aria-label="Slide 3"></button>
  </div>
  <div class="carousel-inner custom-carousel-item">
  <div class="carousel-item active">
    <img src="picture/c.jpg" class="d-block w-100" alt="Foto">
    <div class="carousel-caption d-none d-md-block">
      <h5>First slide label</h5>
      <p>Some representative placeholder content for the first slide.</p>
    </div>
  </div>
    <div class="carousel-item">
      <img src="picture/a.jpeg" class="d-block w-100" alt="Foto">
      <div class="carousel-caption d-none d-md-block">
        <h5>Second slide label</h5>
        <p>Some representative placeholder content for the second slide.</p>
      </div>
    </div>
    <div class="carousel-item">
      <img src="picture/b.jpg" class="d-block w-100" alt="Foto">
      <div class="carousel-caption d-none d-md-block">
        <h5>Third slide label</h5>
        <p>Some representative placeholder content for the third slide.</p>
      </div>
    </div>
    </div>
    <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleAutoplaying" data-bs-slide="prev">
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Previous</span>
    </button>
    <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleAutoplaying" data-bs-slide="next">
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Next</span>
    </button>
</div>
```
This section can be added or reduced depending on the number of experiences you want to include.

### 1.3 Footer
In this section, I will provide contact information to replace the [contact section](#contact) that is not displayed on mobile devices.
```
<footer class="footer-section text-center d-md-none mx-2 mt">
```
The footer will not be displayed on screen sizes larger than a mobile device.
```
<p>
  <a href="tel:#" class="contact-link">+62 ***-****-***</a> <br>
  <a href="mailto:#</a>
</p>
<div>
  <a href="#" class="me-3"><i class="fab fa-line"></i> *****</a>
  <a href="#" target="_blank" class="me-3"><i class="fab fa-instagram"></i> *****</a>
</div>
```
For security and comfort, since this repository is public, I will hide the sensitive data.

</br>
</br>

## 2. CSS
I will only explain a few sections of the CSS.

1. Scrollbar
This code is used to customize the scrollbar.
```
::-webkit-scrollbar {
    width : 5px;
}

::-webkit-scrollbar-track {
    background : #f1f1f1;
}

::-webkit-scrollbar-thumb {
    background : #44717F;
    border-radius : 20px;
}

::-webkit-scrollbar-thumb:hover {
    background : #345a65;
}
```

2. Timeline
This is the styling for the timeline I use in the education section.
```
.timeline-item {
    position: relative;
    padding-left: 1.5rem;
    margin-bottom: 1rem;
}

.timeline-item::before {
    content: '';
    position: absolute;
    left: 0;
    top: 0.5rem;
    width: 0.75rem;
    height: 0.75rem;
    background-color: #25434c;
    border-radius: 50%;
    z-index: 1;
}

.timeline-item::after {
    content: '';
    position: absolute;
    left: 0.275rem;  /* Pusat */
    top: 1.25rem;  /* Bawah titik */
    width: 3px;
    height: calc(100% + 0.75rem); /* garis */
    background-color: #25434c; 
    z-index: 0;
}

.timeline-item:last-child::after {
    height: 3rem;
}
```

