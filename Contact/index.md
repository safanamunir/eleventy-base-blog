---
layout: layouts/post.njk
title: Contact
templateClass: tmpl-post
eleventyNavigation:
  key: Contact
  order: 3
---
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-BmbxuPwQa2lc/FVzBcNJ7UAyJxM6wuqIj61tLrc4wSX0szH/Ev+nYRRuWlolflfl" crossorigin="anonymous">

<div class="container">

<form name="contact" method="POST" data-netlify="true">
  <!-- <input type="hidden" name="form-name" value="contact" /> -->
  


  <div class="mb-3">
    <label class="form-label">Your Name: 
    <input type="text" name="name"  class="form-control" required></label>   
  </div>
  <p>
    <label class="form-label">Your Email: 
    <input  class="form-control" type="email" name="email" required /></label>
  </p>
  <p>
    <label class="form-label"  >Your Role: </label>
    <select class="form-select" name="role[]"  required>
      <option selected value="leader">Leader</option>
      <option value="follower">Follower</option>
    </select>
  </p>
  <p>
    <label class="form-label">Message: </label>
    <textarea class="form-control" rows="3" name="message"></textarea>
  </p>
  <p>
    <button class="btn btn-primary"  type="submit">Send</button>
  </p>

  
</form>
</div>
