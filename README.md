# workflow-example
├── Jenkinsfile
├── README.md
├── index.html
├── test_webhook
└── testfile


/Jenkinsfile:
--------------------------------------------------------------------------------
 1 | node {
 2 |   stage('SCM') {
 3 |     checkout scm
 4 |   }
 5 |   stage('SonarQube Analysis') {
 6 |     def scannerHome = tool 'SonarScanner';
 7 |     withSonarQubeEnv() {
 8 |       sh "${scannerHome}/bin/sonar-scanner"
 9 |     }
10 |   }
11 | }
12 | 


--------------------------------------------------------------------------------
/README.md:
--------------------------------------------------------------------------------
1 | # Examination_Project_CICD
2 | This is a Multioption-examination project with CICD
3 | 


--------------------------------------------------------------------------------
/index.html:
--------------------------------------------------------------------------------
  1 | <!DOCTYPE html>
  2 | <html lang="en">
  3 | 
  4 |   <head>
  5 | 
  6 |     <meta charset="UTF-8">
  7 |     <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
  8 |     <meta name="description" content="">
  9 |     <meta name="author" content="">
 10 |     <link rel="preconnect" href="https://fonts.gstatic.com">
 11 |     <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400;500;600;700;800;900&display=swap" rel="stylesheet">
 12 | 
 13 |     <title>examination Center - SEO HTML5 Template</title>
 14 | 
 15 |     <!-- Bootstrap core CSS -->
 16 |     <link href="vendor/bootstrap/css/bootstrap.min.css" rel="stylesheet">
 17 | 
 18 |     <!-- Additional CSS Files -->
 19 |     <link rel="stylesheet" href="assets/css/fontawesome.css">
 20 |     <link rel="stylesheet" href="assets/css/templatemo-space-dynamic.css">
 21 |     <link rel="stylesheet" href="assets/css/animated.css">
 22 |     <link rel="stylesheet" href="assets/css/owl.css">
 23 | <!--
 24 |     
 25 | TemplateMo 562 Space Dynamic
 26 | 
 27 | https://templatemo.com/tm-562-space-dynamic
 28 | 
 29 | -->
 30 |   </head>
 31 | 
 32 | <body>
 33 | 
 34 |   <!-- ***** Preloader Start ***** -->
 35 |   <div id="js-preloader" class="js-preloader">
 36 |     <div class="preloader-inner">
 37 |       <span class="dot"></span>
 38 |       <div class="dots">
 39 |         <span></span>
 40 |         <span></span>
 41 |         <span></span>
 42 |       </div>
 43 |     </div>
 44 |   </div>
 45 |   <!-- ***** Preloader End ***** -->
 46 | 
 47 |   <!-- ***** Header Area Start ***** -->
 48 |   <header class="header-area header-sticky wow slideInDown" data-wow-duration="0.75s" data-wow-delay="0s">
 49 |     <div class="container">
 50 |       <div class="row">
 51 |         <div class="col-12">
 52 |           <nav class="main-nav">
 53 |             <!-- ***** Logo Start ***** -->
 54 |             <a href="index.html" class="logo">
 55 |               <h4>Spac<span>Dyna</span></h4>
 56 |             </a>
 57 |             <!-- ***** Logo End ***** -->
 58 |             <!-- ***** Menu Start ***** -->
 59 |             <ul class="nav">
 60 |               <li class="scroll-to-section"><a href="#top" class="active">Home</a></li>
 61 |               <li class="scroll-to-section"><a href="#about">About Us</a></li>
 62 |               <li class="scroll-to-section"><a href="#services">Services</a></li>
 63 |               <li class="scroll-to-section"><a href="#portfolio">Portfolio</a></li>
 64 |               <li class="scroll-to-section"><a href="#blog">Blog</a></li> 
 65 |               <li class="scroll-to-section"><a href="#contact">Message Us</a></li> 
 66 |               <li class="scroll-to-section"><div class="main-red-button"><a href="#contact">Contact Now</a></div></li> 
 67 |             </ul>        
 68 |             <a class='menu-trigger'>
 69 |                 <span>Menu</span>
 70 |             </a>
 71 |             <!-- ***** Menu End ***** -->
 72 |           </nav>
 73 |         </div>
 74 |       </div>
 75 |     </div>
 76 |   </header>
 77 |   <!-- ***** Header Area End ***** -->
 78 | 
 79 |   <div class="main-banner wow fadeIn" id="top" data-wow-duration="1s" data-wow-delay="0.5s">
 80 |     <div class="container">
 81 |       <div class="row">
 82 |         <div class="col-lg-12">
 83 |           <div class="row">
 84 |             <div class="col-lg-6 align-self-center">
 85 |               <div class="left-content header-text wow fadeInLeft" data-wow-duration="1s" data-wow-delay="1s">
 86 |                 <h6>Welcome to Space Dynamic</h6>
 87 |                 <h2>We Make <em>Digital Ideas</em> &amp; <span>SEO</span> Marketing</h2>
 88 |                 <p>Space Dynamic is a professional looking HTML template using a Bootstrap 5 (beta 2). This CSS template is free for you provided by <a rel="nofollow" href="https://templatemo.com/page/1" target="_parent">TemplateMo</a>.</p>
 89 |                 <form id="search" action="#" method="GET">
 90 |                   <fieldset>
 91 |                     <input type="address" name="address" class="email" placeholder="Your website URL..." autocomplete="on" required>
 92 |                   </fieldset>
 93 |                   <fieldset>
 94 |                     <button type="submit" class="main-button">Analyze Site</button>
 95 |                   </fieldset>
 96 |                 </form>
 97 |               </div>
 98 |             </div>
 99 |             <div class="col-lg-6">
100 |               <div class="right-image wow fadeInRight" data-wow-duration="1s" data-wow-delay="0.5s">
101 |                 <img src="assets/images/banner-right-image.png" alt="team meeting">
102 |               </div>
103 |             </div>
104 |           </div>
105 |         </div>
106 |       </div>
107 |     </div>
108 |   </div>
109 | 
110 |   <div id="about" class="about-us section">
111 |     <div class="container">
112 |       <div class="row">
113 |         <div class="col-lg-4">
114 |           <div class="left-image wow fadeIn" data-wow-duration="1s" data-wow-delay="0.2s">
115 |             <img src="assets/images/about-left-image.png" alt="person graphic">
116 |           </div>
117 |         </div>
118 |         <div class="col-lg-8 align-self-center">
119 |           <div class="services">
120 |             <div class="row">
121 |               <div class="col-lg-6">
122 |                 <div class="item wow fadeIn" data-wow-duration="1s" data-wow-delay="0.5s">
123 |                   <div class="icon">
124 |                     <img src="assets/images/service-icon-01.png" alt="reporting">
125 |                   </div>
126 |                   <div class="right-text">
127 |                     <h4>Data Analysis</h4>
128 |                     <p>Lorem ipsum dolor sit amet, ctetur aoi adipiscing eliter</p>
129 |                   </div>
130 |                 </div>
131 |               </div>
132 |               <div class="col-lg-6">
133 |                 <div class="item wow fadeIn" data-wow-duration="1s" data-wow-delay="0.7s">
134 |                   <div class="icon">
135 |                     <img src="assets/images/service-icon-02.png" alt="">
136 |                   </div>
137 |                   <div class="right-text">
138 |                     <h4>Data Reporting</h4>
139 |                     <p>Lorem ipsum dolor sit amet, ctetur aoi adipiscing eliter</p>
140 |                   </div>
141 |                 </div>
142 |               </div>
143 |               <div class="col-lg-6">
144 |                 <div class="item wow fadeIn" data-wow-duration="1s" data-wow-delay="0.9s">
145 |                   <div class="icon">
146 |                     <img src="assets/images/service-icon-03.png" alt="">
147 |                   </div>
148 |                   <div class="right-text">
149 |                     <h4>Web Analytics</h4>
150 |                     <p>Lorem ipsum dolor sit amet, ctetur aoi adipiscing eliter</p>
151 |                   </div>
152 |                 </div>
153 |               </div>
154 |               <div class="col-lg-6">
155 |                 <div class="item wow fadeIn" data-wow-duration="1s" data-wow-delay="1.1s">
156 |                   <div class="icon">
157 |                     <img src="assets/images/service-icon-04.png" alt="">
158 |                   </div>
159 |                   <div class="right-text">
160 |                     <h4>SEO Suggestions</h4>
161 |                     <p>Lorem ipsum dolor sit amet, ctetur aoi adipiscing eliter</p>
162 |                   </div>
163 |                 </div>
164 |               </div>
165 |             </div>
166 |           </div>
167 |         </div>
168 |       </div>
169 |     </div>
170 |   </div>
171 | 
172 |   <div id="services" class="our-services section">
173 |     <div class="container">
174 |       <div class="row">
175 |         <div class="col-lg-6 align-self-center  wow fadeInLeft" data-wow-duration="1s" data-wow-delay="0.2s">
176 |           <div class="left-image">
177 |             <img src="assets/images/services-left-image.png" alt="">
178 |           </div>
179 |         </div>
180 |         <div class="col-lg-6 wow fadeInRight" data-wow-duration="1s" data-wow-delay="0.2s">
181 |           <div class="section-heading">
182 |             <h2>Grow your website with our <em>SEO</em> service &amp; <span>Project</span> Ideas</h2>
183 |             <p>Space Dynamic HTML5 template is free to use for your website projects. However, you are not permitted to redistribute the template ZIP file on any CSS template collection websites. Please contact us for more information. Thank you for your kind cooperation.</p>
184 |           </div>
185 |           <div class="row">
186 |             <div class="col-lg-12">
187 |               <div class="first-bar progress-skill-bar">
188 |                 <h4>Website Analysis</h4>
189 |                 <span>84%</span>
190 |                 <div class="filled-bar"></div>
191 |                 <div class="full-bar"></div>
192 |               </div>
193 |             </div>
194 |             <div class="col-lg-12">
195 |               <div class="second-bar progress-skill-bar">
196 |                 <h4>SEO Reports</h4>
197 |                 <span>88%</span>
198 |                 <div class="filled-bar"></div>
199 |                 <div class="full-bar"></div>
200 |               </div>
201 |             </div>
202 |             <div class="col-lg-12">
203 |               <div class="third-bar progress-skill-bar">
204 |                 <h4>Page Optimizations</h4>
205 |                 <span>94%</span>
206 |                 <div class="filled-bar"></div>
207 |                 <div class="full-bar"></div>
208 |               </div>
209 |             </div>
210 |           </div>
211 |         </div>
212 |       </div>
213 |     </div>
214 |   </div>
215 | 
216 |   <div id="portfolio" class="our-portfolio section">
217 |     <div class="container">
218 |       <div class="row">
219 |         <div class="col-lg-6 offset-lg-3">
220 |           <div class="section-heading  wow bounceIn" data-wow-duration="1s" data-wow-delay="0.2s">
221 |             <h2>See What Our Agency <em>Offers</em> &amp; What We <span>Provide</span></h2>
222 |           </div>
223 |         </div>
224 |       </div>
225 |       <div class="row">
226 |         <div class="col-lg-3 col-sm-6">
227 |           <a href="#">
228 |             <div class="item wow bounceInUp" data-wow-duration="1s" data-wow-delay="0.3s">
229 |               <div class="hidden-content">
230 |                 <h4>SEO Analysis</h4>
231 |                 <p>Lorem ipsum dolor sit ameti ctetur aoi adipiscing eto.</p>
232 |               </div>
233 |               <div class="showed-content">
234 |                 <img src="assets/images/portfolio-image.png" alt="">
235 |               </div>
236 |             </div>
237 |           </a>
238 |         </div>
239 |         <div class="col-lg-3 col-sm-6">
240 |           <a href="#">
241 |             <div class="item wow bounceInUp" data-wow-duration="1s" data-wow-delay="0.4s">
242 |               <div class="hidden-content">
243 |                 <h4>Website Reporting</h4>
244 |                 <p>Lorem ipsum dolor sit ameti ctetur aoi adipiscing eto.</p>
245 |               </div>
246 |               <div class="showed-content">
247 |                 <img src="assets/images/portfolio-image.png" alt="">
248 |               </div>
249 |             </div>
250 |           </a>
251 |         </div>
252 |         <div class="col-lg-3 col-sm-6">
253 |           <a href="#">
254 |             <div class="item wow bounceInUp" data-wow-duration="1s" data-wow-delay="0.5s">
255 |               <div class="hidden-content">
256 |                 <h4>Performance Tests</h4>
257 |                 <p>Lorem ipsum dolor sit ameti ctetur aoi adipiscing eto.</p>
258 |               </div>
259 |               <div class="showed-content">
260 |                 <img src="assets/images/portfolio-image.png" alt="">
261 |               </div>
262 |             </div>
263 |           </a>
264 |         </div>
265 |         <div class="col-lg-3 col-sm-6">
266 |           <a href="#">
267 |             <div class="item wow bounceInUp" data-wow-duration="1s" data-wow-delay="0.6s">
268 |               <div class="hidden-content">
269 |                 <h4>Data Analysis</h4>
270 |                 <p>Lorem ipsum dolor sit ameti ctetur aoi adipiscing eto.</p>
271 |               </div>
272 |               <div class="showed-content">
273 |                 <img src="assets/images/portfolio-image.png" alt="">
274 |               </div>
275 |             </div>
276 |           </a>
277 |         </div>
278 |       </div>
279 |     </div>
280 |   </div>
281 | 
282 |   <div id="blog" class="our-blog section">
283 |     <div class="container">
284 |       <div class="row">
285 |         <div class="col-lg-6 wow fadeInDown" data-wow-duration="1s" data-wow-delay="0.25s">
286 |           <div class="section-heading">
287 |             <h2>Check Out What Is <em>Trending</em> In Our Latest <span>News</span></h2>
288 |           </div>
289 |         </div>
290 |         <div class="col-lg-6 wow fadeInDown" data-wow-duration="1s" data-wow-delay="0.25s">
291 |           <div class="top-dec">
292 |             <img src="assets/images/blog-dec.png" alt="">
293 |           </div>
294 |         </div>
295 |       </div>
296 |       <div class="row">
297 |         <div class="col-lg-6 wow fadeInUp" data-wow-duration="1s" data-wow-delay="0.25s">
298 |           <div class="left-image">
299 |             <a href="#"><img src="assets/images/big-blog-thumb.jpg" alt="Workspace Desktop"></a>
300 |             <div class="info">
301 |               <div class="inner-content">
302 |                 <ul>
303 |                   <li><i class="fa fa-calendar"></i> 24 Mar 2021</li>
304 |                   <li><i class="fa fa-users"></i> TemplateMo</li>
305 |                   <li><i class="fa fa-folder"></i> Branding</li>
306 |                 </ul>
307 |                 <a href="#"><h4>SEO Agency &amp; Digital Marketing</h4></a>
308 |                 <p>Lorem ipsum dolor sit amet, consectetur and sed doer ket eismod tempor incididunt ut labore et dolore magna...</p>
309 |                 <div class="main-blue-button">
310 |                   <a href="#">Discover More</a>
311 |                 </div>
312 |               </div>
313 |             </div>
314 |           </div>
315 |         </div>
316 |         <div class="col-lg-6 wow fadeInUp" data-wow-duration="1s" data-wow-delay="0.25s">
317 |           <div class="right-list">
318 |             <ul>
319 |               <li>
320 |                 <div class="left-content align-self-center">
321 |                   <span><i class="fa fa-calendar"></i> 18 Mar 2021</span>
322 |                   <a href="#"><h4>New Websites &amp; Backlinks</h4></a>
323 |                   <p>Lorem ipsum dolor sit amsecteturii and sed doer ket eismod...</p>
324 |                 </div>
325 |                 <div class="right-image">
326 |                   <a href="#"><img src="assets/images/blog-thumb-01.jpg" alt=""></a>
327 |                 </div>
328 |               </li>
329 |               <li>
330 |                 <div class="left-content align-self-center">
331 |                   <span><i class="fa fa-calendar"></i> 14 Mar 2021</span>
332 |                   <a href="#"><h4>SEO Analysis &amp; Content Ideas</h4></a>
333 |                   <p>Lorem ipsum dolor sit amsecteturii and sed doer ket eismod...</p>
334 |                 </div>
335 |                 <div class="right-image">
336 |                   <a href="#"><img src="assets/images/blog-thumb-01.jpg" alt=""></a>
337 |                 </div>
338 |               </li>
339 |               <li>
340 |                 <div class="left-content align-self-center">
341 |                   <span><i class="fa fa-calendar"></i> 06 Mar 2021</span>
342 |                   <a href="#"><h4>SEO Tips &amp; Digital Marketing</h4></a>
343 |                   <p>Lorem ipsum dolor sit amsecteturii and sed doer ket eismod...</p>
344 |                 </div>
345 |                 <div class="right-image">
346 |                   <a href="#"><img src="assets/images/blog-thumb-01.jpg" alt=""></a>
347 |                 </div>
348 |               </li>
349 |             </ul>
350 |           </div>
351 |         </div>
352 |       </div>
353 |     </div>
354 |   </div>
355 | 
356 |   <div id="contact" class="contact-us section">
357 |     <div class="container">
358 |       <div class="row">
359 |         <div class="col-lg-6 align-self-center wow fadeInLeft" data-wow-duration="0.5s" data-wow-delay="0.25s">
360 |           <div class="section-heading">
361 |             <h2>Feel Free To Send Us a Message About Your Website Needs</h2>
362 |             <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed doer ket eismod tempor incididunt ut labore et dolores</p>
363 |             <div class="phone-info">
364 |               <h4>For any enquiry, Call Us: <span><i class="fa fa-phone"></i> <a href="#">010-020-0340</a></span></h4>
365 |             </div>
366 |           </div>
367 |         </div>
368 |         <div class="col-lg-6 wow fadeInRight" data-wow-duration="0.5s" data-wow-delay="0.25s">
369 |           <form id="contact" action="" method="post">
370 |             <div class="row">
371 |               <div class="col-lg-6">
372 |                 <fieldset>
373 |                   <input type="name" name="name" id="name" placeholder="Name" autocomplete="on" required>
374 |                 </fieldset>
375 |               </div>
376 |               <div class="col-lg-6">
377 |                 <fieldset>
378 |                   <input type="surname" name="surname" id="surname" placeholder="Surname" autocomplete="on" required>
379 |                 </fieldset>
380 |               </div>
381 |               <div class="col-lg-12">
382 |                 <fieldset>
383 |                   <input type="text" name="email" id="email" pattern="[^ @]*@[^ @]*" placeholder="Your Email" required="">
384 |                 </fieldset>
385 |               </div>
386 |               <div class="col-lg-12">
387 |                 <fieldset>
388 |                   <textarea name="message" type="text" class="form-control" id="message" placeholder="Message" required=""></textarea>  
389 |                 </fieldset>
390 |               </div>
391 |               <div class="col-lg-12">
392 |                 <fieldset>
393 |                   <button type="submit" id="form-submit" class="main-button ">Send Message</button>
394 |                 </fieldset>
395 |               </div>
396 |             </div>
397 |             <div class="contact-dec">
398 |               <img src="assets/images/contact-decoration.png" alt="">
399 |             </div>
400 |           </form>
401 |         </div>
402 |       </div>
403 |     </div>
404 |   </div>
405 | 
406 |   <footer>
407 |     <div class="container">
408 |       <div class="row">
409 |         <div class="col-lg-12 wow fadeIn" data-wow-duration="1s" data-wow-delay="0.25s">
410 |           <p>© Copyright 2021 Space Dynamic Co. All Rights Reserved. 
411 |           
412 |           <br>Design: <a rel="nofollow" href="https://templatemo.com">TemplateMo</a></p>
413 |         </div>
414 |       </div>
415 |     </div>
416 |   </footer>
417 |   <!-- Scripts -->
418 |   <script src="vendor/jquery/jquery.min.js"></script>
419 |   <script src="vendor/bootstrap/js/bootstrap.bundle.min.js"></script>
420 |   <script src="assets/js/owl-carousel.js"></script>
421 |   <script src="assets/js/animation.js"></script>
422 |   <script src="assets/js/imagesloaded.js"></script>
423 |   <script src="assets/js/templatemo-custom.js"></script>
424 | 
425 | </body>
426 | </html>
427 | 


--------------------------------------------------------------------------------
/test_webhook:
--------------------------------------------------------------------------------
1 | this is test webhook
2 | 


--------------------------------------------------------------------------------
/testfile:
---------------------------------------------------
