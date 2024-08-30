---
id: e70119d5-f07c-4426-a488-68f8b0abf180
blueprint: page
title: Blog
author: 2dffde8f-8095-4a81-8e61-698f35b18138
template: default
meta_title: 'Meta Title'
meta_keywords: 'Meta Keywords'
meta_description: 'Meta Description'
updated_by: 2dffde8f-8095-4a81-8e61-698f35b18138
updated_at: 1724919570
parent: home
content:
  -
    type: set
    attrs:
      id: m0f0fku7
      values:
        type: inside_banner
        title: 'Our Blog And News'
        image: img/blog/blog_1.jpeg
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
      id: m0f0g1xb
      values:
        type: blog_listing
        title_1: 'News & Blog'
        title_2: 'Our latest news post and articles'
        limit: 6
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
    type: paragraph
---
