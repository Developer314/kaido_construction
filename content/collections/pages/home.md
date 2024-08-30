---
id: home
blueprint: pages
title: Home
template: home
author: 2dffde8f-8095-4a81-8e61-698f35b18138
updated_by: 2dffde8f-8095-4a81-8e61-698f35b18138
updated_at: 1724940375
meta_title: 'Meta Title'
meta_keywords: 'Meta Keywords'
meta_description: 'Meta Description'
content:
  -
    type: set
    attrs:
      id: m0fcyjwx
      values:
        type: home_gallery
        gallery_items:
          -
            id: m0fcxqpb
            image: img/home_gallery/home_gallery_1.jpeg
            title_1: 'Foundation Work'
            title_2: 'Foundation Work and 17. Project Management'
            description: 'The standard chunk of Lorem Ipsum used since the 1500s is reproduced below for those interested. Sections 1.10.32 and 1.10.33 from "de Finibus Bonorum et Malorum".'
            button_1_text: Enquire
            button_1_link: /
            button_1_target: _self
            button_2_text: 'More Details'
            button_2_link: /
            button_2_target: _self
            type: gallery_items
            enabled: true
          -
            id: m0fcxycl
            image: img/home_gallery/home_gallery_2.jpeg
            title_1: 'Foundation Work'
            title_2: 'Foundation Work and 17. Project Management'
            description: 'The standard chunk of Lorem Ipsum used since the 1500s is reproduced below for those interested. Sections 1.10.32 and 1.10.33 from "de Finibus Bonorum et Malorum".'
            button_1_text: Enquire
            button_1_link: /
            button_1_target: _self
            button_2_text: 'More Details'
            button_2_link: /
            button_2_target: _self
            type: gallery_items
            enabled: true
          -
            id: m0fcy3do
            image: img/home_gallery/home_gallery_3.jpeg
            title_1: 'Foundation Work'
            title_2: 'Foundation Work and 17. Project Management'
            description: 'The standard chunk of Lorem Ipsum used since the 1500s is reproduced below for those interested. Sections 1.10.32 and 1.10.33 from "de Finibus Bonorum et Malorum".'
            button_1_text: Enquire
            button_1_link: /
            button_1_target: _self
            button_2_text: 'More Details'
            button_2_link: /
            button_2_target: _self
            type: gallery_items
            enabled: true
        edit_template: false
        custom_template: |-
          <!-- Carousel Start -->
           <div class="container-fluid overflow-hidden px-0">
              <div id="carouselId" class="carousel slide" data-bs-ride="carousel">
                  <ol class="carousel-indicators fadeInUp animate__animated" data-animation="fadeInUp" data-delay="1s" style="animation-delay: 1s;">
                      {{gallery_items}}
                      <li data-bs-target="#carouselId" data-bs-slide-to="{{increment}}" {{if first}} class="active" aria-current="true"{{/if}} aria-label="{{title_1}}"></li>
                      {{/gallery_items}}    
                  </ol>
                  <div class="carousel-inner" role="listbox">
                      {{gallery_items}}
                      <div class="carousel-item {{if first}}active{{/if}}">
                          <img src="{{image}}" class="img-fluid w-100" alt="First slide"/>
                          <div class="carousel-caption">
                              <p class="text-uppercase text-secondary fs-4 mb-0 fadeInUp animate__animated" data-animation="fadeInUp" data-delay="1s" style="animation-delay: 1s;">{{title_1}}</p>
                              <h1 class="display-1 text-capitalize text-white mb-4 fadeInUp animate__animated" data-animation="fadeInUp" data-delay="1.3s" style="animation-delay: 1.3s;">{{title_2}}</h1>
                              <p class="mb-5 fs-5 fadeInUp animate__animated" data-animation="fadeInUp" data-delay="1.5s" style="animation-delay: 1.5s;">{{description}}</p>
                              <div class="d-flex justify-content-center">
                                  <a class="btn btn-primary d-flex py-3 px-5 me-2 flex-shrink-0 fadeInUp animate__animated" data-animation="fadeInUp" data-delay="1.5s" style="animation-delay: 1.7s;" href="{{button_1_link}}" target="{{button_1_target}}">{{button_1_text}}</a>
                                  <a class="btn btn-secondary d-inline-block py-3 px-5 ms-2 flex-shrink-0 fadeInUp animate__animated" data-animation="fadeInUp" data-delay="1.5s" style="animation-delay: 1.7s;" href="{{button_2_link}}" target="{{button_2_target}}">{{button_2_text}}</a>
                              </div>
                          </div>
                      </div>
                      {{/gallery_items}}
                  </div>
                  <button class="carousel-control-prev" type="button" data-bs-target="#carouselId" data-bs-slide="prev">
                      <span class="carousel-control-prev-icon btn-lg-square fadeInLeft animate__animated" aria-hidden="true" data-animation="fadeInLeft" data-delay="1.1s" style="animation-delay: 1.3s;"><i class="fas fa-chevron-left fa-2x"></i></span>
                      <span class="visually-hidden">Previous</span>
                  </button>
                  <button class="carousel-control-next" type="button" data-bs-target="#carouselId" data-bs-slide="next">
                      <span class="carousel-control-next-icon btn-lg-square fadeInRight animate__animated" aria-hidden="true" data-animation="fadeInRight" data-delay="1.1s" style="animation-delay: 1.3s;"><i class="fas fa-chevron-right fa-2x"></i></span>
                      <span class="visually-hidden">Next</span>
                  </button>
              </div>
          </div>
          <!-- Carousel End -->
  -
    type: set
    attrs:
      id: m0dugnph
      values:
        type: about_us
        image: img/about_us.jpeg
        title_1: 'Creating Spaces, Building Relationships'
        title_2: 'Transforming Your Ideas into Reality with Strong Foundation and Expertise'
        description:
          -
            type: paragraph
            attrs:
              textAlign: left
            content:
              -
                type: text
                text: 'Kaido Construction Company is a renowned and trusted name in the construction industry, dedicated to delivering exceptional building experiences. With a passion for excellence and a commitment to quality, we transform visions into reality, crafting spaces that inspire and endure.'
          -
            type: paragraph
            attrs:
              textAlign: left
            content:
              -
                type: text
                text: 'Our journey began with a simple yet profound mission: to build a better future. We believe that every project, regardless of size or scope, deserves meticulous attention to detail, unwavering dedication, and unrelenting passion. This philosophy has guided us in establishing a reputation for reliability, innovation, and unparalleled customer satisfaction.'
          -
            type: paragraph
            attrs:
              textAlign: left
            content:
              -
                type: text
                text: 'What sets us apart is our unwavering commitment to quality, safety, and sustainability. We employ cutting-edge technology, innovative techniques, and sustainable practices to minimize our environmental footprint while maximizing value for our clients. As we continue to grow and evolve, we remain steadfast in our dedication to excellence, integrity, and customer satisfaction. Join us in building a better future, one project at a time.'
        button_text: 'Find Out More'
        button_link: /
        edit_template: true
        custom_template: |-
          <!-- About Start -->
           <div class="container-fluid about py-5"> 
              <div class="container py-5">
                  <div class="row g-5 align-items-center">
                      <div class="col-xl-6 wow fadeInLeft" data-wow-delay="0.1s">
                         
                              <img src="{{ glide:image preset="about_us" }}" class="img-1 img-fluid w-100"  alt="{{title_1}}">
                         
                      </div>
                      <div class="col-xl-6 wow fadeInRight" data-wow-delay="0.1s">
                          <div class="about-item-content">
                              <p class="text-uppercase text-secondary fs-5 mb-0">{{title_1}}</p>
                              <h2 class="display-4 text-capitalize mb-3">{{title_2}}</h2>
                              {{description}}
                              
                              <a class="btn btn-secondary d-inline-block py-3 px-5 me-2 flex-shrink-0 wow fadeInUp" title="{{title_1}}" data-wow-delay="0.1s" href="{{button_link}}">{{button_text}}</a>
                          </div>
                      </div>
                  </div>
              </div>
          </div>
          <!-- About End -->
  -
    type: set
    attrs:
      id: m0dv4hvq
      values:
        type: why_choose_us
        title_1: 'Why Us'
        title_2: 'What Makes Us Unique'
        reasons:
          -
            id: m0dv4ka9
            icon: fa-city
            title: 'Design and Build Expert'
            data: 'It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters'
          -
            id: m0dv4o1p
            icon: fa-funnel-dollar
            title: 'Skilled Craftsman'
            data: 'It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters'
          -
            id: m0dv4si9
            icon: fa-tools
            title: 'Building Science Specialist'
            data: 'It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters'
        edit_template: true
        custom_template: |-
          <!-- Why Us Start -->
            <div class="container-fluid feature bg-light py-5">
              <div class="container py-5">
                  <div class="text-center mx-auto pb-5 wow fadeInUp" data-wow-delay="0.2s" style="max-width: 800px;">
                      <p class="text-uppercase text-secondary fs-5 mb-0">{{title_1}}</p>
                      <h2 class="display-4 text-capitalize mb-3">{{title_2}}</h2>
                  </div>
                  <div class="row g-4">
                     {{reasons}}
                      <div class="col-lg-4 wow fadeInUp" data-wow-delay="0.2s">
                          <div class="feature-item text-center border p-5">
                              <div class="feature-img bg-secondary d-inline-flex p-4">
                                  <i class="fas {{icon}} text-primary fa-5x"></i>
                              </div>
                              <a href="#" class="h4 d-block my-4">{{title}}</a>
                              <p class="mb-0">{{data}}</p>
                          </div>
                      </div>
                     {{/reasons}}
                  </div>
              </div>
          </div>
          <!-- Why Us End -->
  -
    type: set
    attrs:
      id: m0dyjms4
      values:
        type: services
        title_2: 'Crafting Unique Experiences, with Precision and Care & Elevating Expectations, with Creative Flair'
        read_more_text: 'Read More'
        button_text: 'More Services'
        button_link: /services
        edit_template: true
        custom_template: |-
          <!-- Services Start --> 
                  <div class="container-fluid service bg-light {{ if is_homepage }} pb-5 {{else}} py-5 {{ /if }}">
                      <div class="container pb-5">
                          <div class="text-center mx-auto {{ if is_homepage }} pb-5 {{else}} py-5 {{ /if }} wow fadeInUp" data-wow-delay="0.2s" style="max-width: 800px;">
                              <p class="text-uppercase text-secondary fs-5 mb-0">{{title_1}}</p>
                              <h2 class="display-4 text-capitalize mb-3">{{title_2}}</h2>
                          </div>
                          <div class="row g-4">
                              {{collection:services paginate="{{limit}}" as="posts"}}
          {{posts}}
                              <div class="col-lg-4 wow fadeInUp" data-wow-delay="0.2s">
                                  <div class="service-item">
                                      <div class="service-img">
                                          <img src="{{ glide:image preset="service_listing" }}" class="img-fluid w-100" alt="{{title}}">
                                      </div>
                                      <div class="service-content text-center p-4">
                                          <div class="bg-secondary btn-xl-square mx-auto" style="width: 120px; height: 120px;">
                                              <i class="fas {{icon}} text-primary fa-4x"></i>
                                          </div>
                                          <a href="#" class="d-block fs-4 my-4">{{title}}</a>
                                          <p class="text-white mb-4">{{short_description}}</p>
                                          <a class="btn btn-secondary py-2 px-4" href="{{url}}" title="{{title}}">{{read_more_text}}</a>
                                      </div>
                                      <div class="service-tytle">
                                          <div class="d-flex align-items-center ps-4 w-100">
                                              <h4>{{title}}</h4>
                                          </div>
                                          <div class="btn-xl-square bg-secondary p-4" style="width: 80px; height: 80px;">
                                              <i class="fas {{icon}} text-primary fa-2x"></i>
                                          </div>
                                      </div>
                                  </div>
                              </div>
          {{/posts}}
                              {{/collection:services}}
                              {{if button_text}}
                              <div class="col-12 text-center wow fadeInUp" data-wow-delay="0.2s">
                                  <a class="btn btn-secondary py-3 px-5 mt-4" href="{{button_link}}">{{button_text}}</a>
                              </div>
                              {{/if}}
                          </div>
                      </div>
                  </div>
                  <!-- Services End -->
        limit: 6
        title_1: 'Our Services'
  -
    type: set
    attrs:
      id: m0enepg3
      values:
        type: counter
        counters:
          -
            id: m0enerjh
            icon: fa-thumbs-up
            title: 'Completed Projects'
            number: 456
          -
            id: m0eneskf
            icon: fa-users
            title: 'Happy Customers'
            number: 320
          -
            id: m0enetem
            icon: fa-user
            title: 'Qualified Engineers'
            number: 53
          -
            id: m0enf7cq
            icon: fa-heart
            title: 'Year of Experience'
            number: 20
        button_text: 'Join With Us'
        edit_template: false
        custom_template: |-
          <!-- Fact Counter -->
                 <div class="container-fluid counter py-5">
                  <div class="container py-5">
                      <div class="row g-4">
                         {{counters}}
                          <div class="col-lg-6 col-xl-3 wow fadeInUp" data-wow-delay="0.2s">
                              <div class="counter-box">
                                  <div class="counter-item">
                                      <div class="counter-item-style"></div>
                                      <div class="counter-item-inner p-5">
                                          <i class="fas {{icon}} fa-4x text-secondary"></i>
                                          <h4 class="text-dark my-4">{{title}}</h4>
                                          <div class="counter-counting">
                                              <span class="text-secondary fs-2 fw-bold" data-toggle="counter-up">{{number}}</span>
                                              <span class="h1 fw-bold text-secondary">+</span>
                                          </div>
                                      </div>
                                  </div>
                              </div>
                          </div>
                          {{/counters}}
                         
                          <div class="col-12 text-center pt-4 wow fadeInUp" data-wow-delay="0.9s">
                              <a class="counter-btn btn btn-secondary py-3 px-5" href="{{button_link}}" title="{{button_text}}">{{button_text}}</a>
                          </div>

                      </div>
                  </div>
              </div>
              <!-- Fact Counter -->
        button_link: /contact
  -
    type: set
    attrs:
      id: m0erk49m
      values:
        type: projects_listing
        title_1: 'Project Showcase'
        title_2: 'A Showcase of Our Craftsmanship and Expertise'
        read_more_text: 'View Project'
        button_text: 'Explore Projects'
        button_link: /projects
        limit: 4
        edit_template: true
        custom_template: |-
          <!-- Projects Start -->
             <div class="container-fluid project py-5"> 
              <div class="container py-5">
                  <div class="text-center mx-auto pb-5 wow fadeInUp" data-wow-delay="0.2s" style="max-width: 800px;">
                      <p class="text-uppercase text-secondary fs-5 mb-0">{{title_1}}</p>
                      <h2 class="display-4 text-capitalize mb-3">{{title_2}}</h2>
                  </div>
                  <div class="row g-5">
                      {{collection:projects paginate="{{limit}}" as="posts"}}
          {{posts}}
                      <div class="col-lg-6 wow fadeInUp" data-wow-delay="0.2s">
                          <div class="project-item">
                              <div class="row g-4">
                                  <div class="col-md-4">
                                      <div class="project-img">
                                         
                                          <img src="{{ glide:image preset="projects_listing" }}" class="img-fluid w-100 pt-3 ps-3" alt="{{title}}">
                                      </div>
                                  </div>
                                  <div class="col-md-8">
                                      <div class="project-content mb-4">
                                          <p class="fs-5 text-secondary mb-2">{{title}}</p>
                                          <a href="#" class="h4">{{title_2}}</a>
                                          <p class="mb-0 mt-3">{{short_description}}</p>
                                      </div>
                                      <a class="btn btn-primary py-2 px-4" href="{{url}}" title="{{title}}">{{read_more_text}}</a>
                                  </div>
                              </div>
                          </div>
                      </div>
                      {{/posts}}
                      {{/collection:projects}}  
                      {{if button_text}}
                      <div class="col-12 text-center wow fadeInUp" data-wow-delay="0.2s">
                          <a class="btn btn-secondary py-3 px-5" href="{{button_link}}">{{button_text}}</a>
                      </div>
                      {{/if}}
                  </div>
              </div>
          </div>
          <!-- Projects End -->
  -
    type: set
    attrs:
      id: m0evd3cu
      values:
        type: team_members
        title_1: 'Our Team'
        title_2: 'Highly Skilled and Experienced Professionals Working Together as a Team'
        edit_template: true
        custom_template: |-
          <!-- Team Start -->
               <div class="container-fluid team {{ if is_homepage }} pb-5 {{else}} py-5 {{ /if }}">
                  <div class="container {{ if is_homepage }} pb-5 {{else}} py-5 {{ /if }}">
                      <div class="text-center mx-auto pb-5 wow fadeInUp" data-wow-delay="0.2s" style="max-width: 800px;">
                          <p class="text-uppercase text-secondary fs-5 mb-0">{{title_1}}</p>
                          <h2 class="display-4 text-capitalize mb-3">{{title_2}}</h2>
                      </div>
                      <div class="row g-4">
                         
          {{ foreach:team_members:members }}
                          {{if key < limit}}
                          <div class="col-lg-3 wow fadeInUp" data-wow-delay="0.2s">
                              <div class="team-item border border-primary p-1">
                                  <div class="team-border-style-1"></div>
                                  <div class="team-border-style-2"></div>
                                  <div class="team-border-style-3"></div>
                                  <div class="team-border-style-4"></div>
                                  <div class="team-img">
                                      <img src="{{ glide:value.image preset="team_member" }}" class="img-fluid w-100" alt="{{value.name}}">
                                      <div class="team-icon d-flex justify-content-around">
                                          {{value.social_links}}
                                          <a class="btn btn-secondary btn-md-square text-white mx-3" href="{{url}}" target="_blank" title="{{value.name}}"><i class="fab {{icon}}"></i></a>
                                          {{/value.social_links}}
                                      </div>
                                  </div>
                                  <div class="text-center border border-top-0 bg-white py-3">
                                      <h4 class="mb-0">{{value.name}}</h4>
                                      <p class="mb-0">{{value.designation}}</p>
                                  </div>
                              </div>
                          </div>
                          {{/if}}
                         {{ /foreach:team_members:members }}
                          {{if button_text}}
                          <div class="col-12 text-center wow fadeInUp" data-wow-delay="0.2s">
                              <a class="btn btn-secondary py-3 px-5" href="{{button_link}}">{{button_text}}</a>
                          </div>
                          {{/if}}
                      </div>
                  </div>
              </div>
              <!-- Team End -->
        limit: 4
        button_text: 'Explore Team'
        button_link: /team
  -
    type: set
    attrs:
      id: m0f05dt2
      values:
        type: blog_listing
        title_1: 'News & Blog'
        title_2: 'Our latest news post and articles'
        limit: 3
        button_text: 'More news'
        button_link: /blog
        edit_template: true
        custom_template: |-
          <!-- Blog Start -->
            <div class="container-fluid blog pb-5">  
              <div class="container pb-5">
                  <div class="text-center mx-auto  {{ if is_homepage }} pb-5 {{else}} py-5 {{ /if }} wow fadeInUp" data-wow-delay="0.2s" style="max-width: 800px;">
                      <p class="text-uppercase text-secondary  {{ if is_homepage }} pb-5 {{else}} py-5 {{ /if }} mb-0">{{title_1}}</p>
                      <h2 class="display-4 text-capitalize mb-3">{{title_2}}</h2>
                  </div>
                  {{ collection:blog limit="3" paginate="true" as="posts" sort="date_created:desc" }}
                  <div class="row g-4">
                     
                      
                      {{posts}}
                      <div class="col-lg-4 wow fadeInUp" data-wow-delay="0.2s">
                          <div class="blog-item h-100">
                              <div class="blog-img">
                                  <img src="{{ glide:image preset="blog_thumb" }}" class="img-fluid w-100" alt="{{title}}">
                              </div>
                              <div class="blog-content p-4">
                                  <div class="d-flex justify-content-between mb-3">
                                      <p class="mb-0"><i class="fa fa-calendar-check text-secondary me-1"></i>{{date_created}}</p>
                                      <p class="mb-0"><i class="fa fa-user text-secondary me-1"></i> {{author}}</p>
                                  </div>
                                  <a href="#" class="h4 d-block mb-4">{{title}}</a>
                                  <a class="btn btn-secondary py-2 px-4" href="{{url}}" title="{{title}}">Read More</a>
                              </div>
                          </div>
                      </div>
                      {{/posts}}
                  </div>

                 {{if !is_homepage}}

                   <!-- Blog Pagination Section -->
            

               
                        <div class="col-12 text-center wow fadeInUp" data-wow-delay="0.2s">
                  
              

                      
                           {{ paginate }}
                           {{ if prev_page }}
                        <a href="{{ prev_page }}" class="btn btn-secondary py-3 px-5 mt-4"><i class="bi bi-chevron-left"></i></a>
                        {{/if}}
                       {{ if next_page }}
                        <a href="{{ next_page }}" class="btn btn-secondary py-3 px-5 mt-4"><i class="bi bi-chevron-right"></i></a>
                        {{/if}}
                        
                        {{ /paginate }}
                        </div> 
              
                  <!-- /Blog Pagination Section -->

                {{else}}

                <div class="col-12 text-center wow fadeInUp" data-wow-delay="0.2s">
                  <a class="btn btn-secondary py-3 px-5 mt-4" href="{{button_link}}">{{button_text}}</a>
               </div>

                {{/if}}

                {{/collection:blog}}

                

              </div>
          </div>
          <!-- Blog End -->
  -
    type: set
    attrs:
      id: m0f1z3oy
      values:
        type: testimonial
        title_1: Testimonials
        title_2: 'Our clients reviews.'
        edit_template: true
        custom_template: |-
          <!-- Testimonial Start -->
          <div class="container-fluid testimonial {{ if is_homepage }} pb-5 {{else}} py-5 {{ /if }}">
              <div class="container {{ if is_homepage }} pb-5 {{else}} py-5 {{ /if }}">
                  <div class="text-center mx-auto pb-5 wow fadeInUp" data-wow-delay="0.2s" style="max-width: 800px;">
                      <p class="text-uppercase text-secondary fs-5 mb-0">{{title_1}}</p>
                      <h2 class="display-4 text-capitalize mb-3">{{title_2}}</h2>
                  </div>
                  <div class="owl-carousel testimonial-carousel wow fadeInUp" data-wow-delay="0.4s">
                      {{testimonials:testimonials}}
                      <div class="testimonial-item bg-light p-4">
                          <div class="position-relative">
                              <i class="fa fa-quote-right fa-2x text-primary position-absolute" style="bottom: 30px; right: 0;"></i>
                              <div class="mb-4 pb-4 border-bottom border-secondary">
                                  <p class="mb-0">{{testimonial}}</p>
                              </div>
                              <div class="d-flex align-items-center flex-nowrap">
                                  <div class="me-4">
                                      <img src="{{ glide:image preset="testimonial" }}" class="img-fluid w-100" style="width: 100px; height: 100px;" alt="{{client_name}}">
                                  </div>
                                  <div class="d-block">
                                      <h4 class="text-dark">{{client_name}}</h4>
                                      <p class="m-0 pb-3">{{profession}}</p>
                                      <div class="d-flex text-secondary pe-5">
                                          <i class="fas fa-star"></i>
                                          <i class="fas fa-star"></i>
                                          <i class="fas fa-star"></i>
                                          <i class="fas fa-star"></i>
                                          <i class="fas fa-star text-muted"></i>
                                      </div>
                                  </div>
                              </div>
                          </div>
                      </div>
                      {{/testimonials:testimonials}}
                      
                  </div>
              </div>
          </div>
          <!-- Testimonial End -->
           
  -
    type: paragraph
---
