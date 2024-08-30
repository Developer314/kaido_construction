---
id: a396df08-e7f4-45c0-bb7c-4368b879369d
blueprint: page
title: Testimonial
author: 2dffde8f-8095-4a81-8e61-698f35b18138
template: default
meta_title: 'Meta Title'
meta_keywords: 'Meta Keywords'
meta_description: 'Meta Description'
updated_by: 2dffde8f-8095-4a81-8e61-698f35b18138
updated_at: 1724923499
parent: home
content:
  -
    type: set
    attrs:
      id: m0f2q4hj
      values:
        type: inside_banner
        title: 'Our testimonials'
        image: img/projects/project_1.jpeg
        edit_template: false
        custom_template: |-
          <div class="container-fluid bg-breadcrumb" style="background-image: url({{image}});">
              <div class="container text-center py-5" style="max-width: 900px;">
              <h4 class="text-white display-4 mb-4 wow fadeInDown" data-wow-delay="0.1s" style="visibility: visible; animation-delay: 0.1s; animation-name: fadeInDown;">{{title}}</h4>
              <ol class="breadcrumb d-flex justify-content-center mb-0 wow fadeInDown" data-wow-delay="0.3s" style="visibility: visible; animation-delay: 0.3s; animation-name: fadeInDown;">
              <li class="breadcrumb-item"><a href="/">Home</a></li>
              <li class="breadcrumb-item active text-secondary">{{title}}</li>
              </ol>
              </div>
          </div>
  -
    type: set
    attrs:
      id: m0f2qtjz
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
