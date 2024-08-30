---
id: 11f6aac8-74e2-4dce-9404-9930774c6e1d
blueprint: page
title: Projects
author: 2dffde8f-8095-4a81-8e61-698f35b18138
template: default
meta_title: 'Meta Title'
meta_keywords: 'Meta Keywords'
meta_description: 'Meta Description'
updated_by: 2dffde8f-8095-4a81-8e61-698f35b18138
updated_at: 1724906463
parent: home
content:
  -
    type: set
    attrs:
      id: m0esquc6
      values:
        type: inside_banner
        title: 'Our Portfolio'
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
      id: m0esq24i
      values:
        type: projects_listing
        title_1: 'Project Showcase'
        title_2: 'A Showcase of Our Craftsmanship and Expertise'
        read_more_text: 'View Project'
        limit: 25
        edit_template: false
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
    type: paragraph
---
