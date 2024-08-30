---
id: 373de9b0-e284-4b14-bbdf-d9f11024f2cd
blueprint: page
title: Features
author: 2dffde8f-8095-4a81-8e61-698f35b18138
template: default
meta_title: 'Meta Title'
meta_keywords: 'Meta Keywords'
meta_description: 'Meta Description'
updated_by: 2dffde8f-8095-4a81-8e61-698f35b18138
updated_at: 1724940841
content:
  -
    type: set
    attrs:
      id: m0fd7kzg
      values:
        type: inside_banner
        title: 'Our Features'
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
      id: m0fd7y82
      values:
        type: why_choose_us
        title_1: 'Why Us'
        title_2: 'What Makes Us Unique'
        reasons:
          -
            id: m0fd80kw
            icon: fa-city
            title: 'Design and Build Expert'
            data: 'It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters'
          -
            id: m0fd81xn
            icon: fa-funnel-dollar
            title: 'Design and Build Expert'
            data: 'It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters'
          -
            id: m0fd83rx
            icon: fa-tools
            title: 'Design and Build Expert'
            data: 'It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters'
        edit_template: false
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
      id: m0fd8cma
      values:
        type: contact_us
        title_1: 'Lets Connect'
        title_2: 'Send Your Message'
        description: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book"
        submit_button_text: 'Submit Now'
        form_success_message: 'We have received your message, We will contact you soon...'
        google_map: |-
          <iframe class="h-100 w-100" style="height: 500px;"
                                  src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d387191.33750346623!2d-73.97968099999999!3d40.6974881!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x89c24fa5d33f083b%3A0xc80b8f06e177fe62!2sNew%20York%2C%20NY%2C%20USA!5e0!3m2!1sen!2sbd!4v1694259649153!5m2!1sen!2sbd"
                                  loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
        contacts:
          -
            id: m0fd8h1v
            icon: fa-map-marker-alt
            title: Address
            data: 'Trivandrum, Kerala, India'
          -
            id: m0fd8i2b
            icon: fa-envelope
            title: Address
            data: 'Trivandrum, Kerala, India'
          -
            id: m0fd8ip7
            icon: fa-phone-alt
            title: Address
            data: 'Trivandrum, Kerala, India'
        edit_template: false
        custom_template: |-
          <div class="container-fluid contact bg-light py-5"> 
              <div class="container py-5">
                  <div class="row g-5 mb-5">
                      <div class="col-lg-6 wow fadeInLeft" data-wow-delay="0.2s">
                          <div class="text-center mx-auto pb-5" style="max-width: 800px;">
                              <p class="text-uppercase text-secondary fs-5 mb-0">{{title_1}}</p>
                              <h2 class="display-4 text-capitalize mb-3">{{title_2}}</h2>
                              <p class="mb-0">{{description}}</p>
                          </div>
                          {{ form:contact_us }}
                                 
                          {{ if success }}
                              <div class="text-success">
                                  {{ form_success_message }}
                              </div>
                          {{ else }}
                             {{ if errors }}
                                  <div class="text-danger mb-3">
                                      {{ errors }}
                                          {{ value }}<br>
                                      {{ /errors }}
                                  </div>
                              {{ /if }}
                              <div class="row g-3">
                                  {{fields}}
                                  {{if type=="textarea"}}

                                  <div class="col-12">
                                      <div class="form-floating border border-secondary">
                                          <textarea class="form-control" name="{{handle}}" placeholder="{{placeholder}}" 
                                              style="height: 160px"></textarea>
                                          <label for="message">{{placeholder}}</label>
                                      </div>
                                  </div>

                                  {{elseif handle=="subject"}}
                                  
                                  <div class="col-lg-12 col-xl-6">
                                      <div class="form-floating border border-secondary">
                                          <input type="{{input_type}}" class="form-control" name="{{handle}}" placeholder="{{placeholder}}" >
                                          <label for="name">{{placeholder}}</label>
                                      </div>
                                  </div>
                                  {{else}}
                                  <div class="col-lg-12 col-xl-6">
                                      <div class="form-floating border border-secondary">
                                          <input type="{{input_type}}" class="form-control" name="{{handle}}" placeholder="{{placeholder}}">
                                          <label for="phone">{{placeholder}}</label>
                                      </div>
                                  </div>
                                  {{/if}}
                                  {{/fields}}
                                  
                                  
                                  <div class="col-12">
                                      <button type="submit" class="btn btn-primary w-100 py-3">{{submit_button_text}}</button>
                                  </div>
                              </div>
                          {{/if}}
                          {{/form:contact_us }}
                      </div>
                      <div class="col-lg-6 wow fadeInRight" data-wow-delay="0.4s"
                          style="visibility: visible; animation-delay: 0.4s; animation-name: fadeInRight;">
                          <div class="contact-map h-100 w-100">
                              {{google_map}}
                          </div>
                      </div>
                  </div>
                  <div class="row g-5">
                      {{contacts}}
                      <div class="col-xl-4 wow fadeInUp" data-wow-delay="0.2s">
                          <div class="d-inline-flex bg-white w-100 border border-secondary p-4">
                              <i class="fas {{icon}} fa-2x text-secondary me-4"></i>
                              <div>
                                  <h4>{{title}}</h4>
                                  <p class="mb-0">{{data}}</p>
                              </div>
                          </div>
                      </div>
                     {{/contacts}}
                  </div>
              </div>
          </div>
  -
    type: paragraph
---
