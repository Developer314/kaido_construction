---
id: 9a862549-1fef-487f-8cbc-b2b890eb6713
blueprint: page
title: Team
author: 2dffde8f-8095-4a81-8e61-698f35b18138
template: default
meta_title: 'Meta Title'
meta_keywords: 'Meta Keywords'
meta_description: 'Meta Description'
updated_by: 2dffde8f-8095-4a81-8e61-698f35b18138
updated_at: 1724912761
parent: home
content:
  -
    type: set
    attrs:
      id: m0ew2vf3
      values:
        type: inside_banner
        title: 'Our Expert Team'
        image: img/home_gallery/home_gallery_2.jpeg
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
      id: m0ew3dof
      values:
        type: team_members
        title_1: 'Our Team'
        title_2: 'Highly Skilled and Experienced Professionals Working Together as a Team'
        limit: 20
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
  -
    type: paragraph
---
