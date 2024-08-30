---
id: 8dc175f6-7cac-463b-9c2c-6f4df740df70
blueprint: page
title: Services
author: 2dffde8f-8095-4a81-8e61-698f35b18138
template: default
meta_title: 'Meta Title'
meta_keywords: 'Meta Keywords'
meta_description: 'Meta Description'
updated_by: 2dffde8f-8095-4a81-8e61-698f35b18138
updated_at: 1724856830
parent: home
content:
  -
    type: set
    attrs:
      id: m0dyxdi5
      values:
        type: inside_banner
        title: 'Banner Text'
        image: img/home_gallery/home_gallery_1.jpeg
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
      id: m0dyxt25
      values:
        type: services
        title_2: 'Crafting Unique Experiences, with Precision and Care & Elevating Expectations, with Creative Flair'
        limit: 50
        read_more_text: 'Read More'
        button_text: 'Contact Us'
        button_link: /contact
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
        title_1: 'Our Services'
  -
    type: paragraph
---
