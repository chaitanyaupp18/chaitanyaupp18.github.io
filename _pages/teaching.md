---
layout: page
permalink: /teaching/
title: Teaching & Talks
description: My experience in teaching and public speaking.
nav: true
nav_order: 6
---

<div class="teaching-section">

  <h2 class="section-title mb-4" style="border-bottom: 2px solid var(--global-theme-color); padding-bottom: 10px;">Teaching Experience</h2>

  <div class="row">
    <div class="col-md-6 mb-4">
      <div class="card h-100">
        <div class="card-body d-flex flex-column justify-content-between">
          <div>
            <div class="d-flex align-items-center mb-2">
              <img src="{{ '/assets/img/teaching_icon_1.png' | relative_url }}" style="width: 60px; height: 60px; object-fit: contain; border-radius: 8px; margin-right: 15px; background-color: #f8f9fa; padding: 5px;" alt="Compiler Design">
              <h4 class="card-title mb-0">Compiler Design</h4>
            </div>
            <p class="card-text text-muted">Summer 2025</p>
            <p class="card-text">Served as a Teaching Assistant or Instructor, guiding students through advanced compiler optimization techniques.</p>
          </div>
          <span class="badge badge-secondary align-self-start mt-2">Teaching</span>
        </div>
      </div>
    </div>

    <div class="col-md-6 mb-4">
      <div class="card h-100">
        <div class="card-body d-flex flex-column justify-content-between">
          <div>
            <div class="d-flex align-items-center mb-2">
              <img src="{{ '/assets/img/teaching_icon_1.png' | relative_url }}" style="width: 60px; height: 60px; object-fit: contain; border-radius: 8px; margin-right: 15px; background-color: #f8f9fa; padding: 5px;" alt="Compiler Design">
              <h4 class="card-title mb-0">Compiler Design</h4>
            </div>
            <p class="card-text text-muted">Summer 2024</p>
            <p class="card-text">Assisted in teaching the fundamentals of compiler design, including parsing and intermediate representations.</p>
          </div>
          <span class="badge badge-secondary align-self-start mt-2">Teaching</span>
        </div>
      </div>
    </div>
  </div>

  <div class="row">
    <div class="col-md-6 mb-4">
      <div class="card h-100">
        <div class="card-body d-flex flex-column justify-content-between">
          <div>
            <div class="d-flex align-items-center mb-2">
              <img src="{{ '/assets/img/teaching_icon_2.png' | relative_url }}" style="width: 60px; height: 60px; object-fit: contain; border-radius: 8px; margin-right: 15px; background-color: #f8f9fa; padding: 5px;" alt="Compiler Construction">
              <h4 class="card-title mb-0">Compiler Construction</h4>
            </div>
            <p class="card-text text-muted">Fall 2023</p>
            <p class="card-text">Supported students in building compilers, focusing on code generation and register allocation.</p>
          </div>
          <span class="badge badge-secondary align-self-start mt-2">Teaching</span>
        </div>
      </div>
    </div>
  </div>

  <h2 class="section-title mb-4 mt-4" style="border-bottom: 2px solid var(--global-theme-color); padding-bottom: 10px;">Talks & Presentations</h2>

  <div class="card mb-4">
    <div class="card-body">
      <div class="d-flex align-items-center mb-2">
        <img src="{{ '/assets/img/prefix_talk_thumb.png' | relative_url }}" style="width: 120px; height: auto; object-fit: contain; border-radius: 4px; margin-right: 15px; border: 1px solid #ddd;" alt="PreFix Talk Thumbnail">
        <h4 class="card-title mb-0">Technical Deep-Dive on Heap Layout Optimization</h4>
      </div>
      <p class="card-text text-muted">Google Compiler Optimization Team | 2024</p>
      <p class="card-text">
        Presented a technical deep-dive on heap layout optimization strategies (PreFix) to the Compiler Optimization Team at Google. Discussed how to improve spatial locality and reduce data cache misses.
      </p>
      <div class="d-flex align-items-center mt-2">
        <span class="badge badge-info mr-2">Invited Talk</span>
        <button type="button" class="btn btn-sm btn-outline-primary" data-toggle="modal" data-target="#slidesModal">View Slides</button>
      </div>
    </div>
  </div>

  <!-- Modal -->
  <div class="modal fade" id="slidesModal" tabindex="-1" role="dialog" aria-labelledby="slidesModalLabel" aria-hidden="true">
    <div class="modal-dialog modal-lg modal-dialog-centered" role="document">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title" id="slidesModalLabel">Google Talk Slides (PreFix)</h5>
          <button type="button" class="close" data-dismiss="modal" aria-label="Close">
            <span aria-hidden="true">&times;</span>
          </button>
        </div>
        <div class="modal-body">
          <div class="embed-responsive embed-responsive-16by9">
            <iframe class="embed-responsive-item" src="https://docs.google.com/presentation/d/1yqRdsZyOLezegSZeS68odzcMhSOzDLMDDGXTCeiRNDk/embed?start=false&loop=false&delayms=3000&rm=minimal#slide=id.g33c4ed5785b_0_352" allowfullscreen></iframe>
          </div>
        </div>
      </div>
    </div>
  </div>

</div>
