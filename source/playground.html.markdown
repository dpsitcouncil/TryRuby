---
title: "GirlCode | DiPS IT Council"
description: Play around with Ruby programs
---

<div class="row">
    <h2 id="tryruby-title">Playground</h2>
    <div id="tryruby-content"><p>
        In the Playground you can try any Ruby code you like.<br />
        See the
        <a href="https://docs.ruby-lang.org/en/master/" target="_blank">Official Ruby documentation ></a>
      </p>
    </div>
 </div>
 <div class="row">

  <div class="col-md-6">
    <h2 class="code-title">Editor</h2>
    <div id="editor" class="tryruby-code tryruby-code--editor"></div>

    <div class="tryruby-buttons">
      <button
        id="btn_copy_url"
        type="button"
        class="btn btn-secondary"
        aria-controls="editor"
      >
        Copy URL
      </button>
      <select
        id="tryruby-engine"
        class="form-select mx-3 w-50"
        aria-controls="output"
      >
      </select>

      <button
        id="btn_run"
        type="button"
        class="btn btn-primary w-25"
        aria-controls="output"
      >
        Run
      </button>
    </div>

  </div>


  <div class="col-md-6">
    <h2 class="code-title">Output</h2>
    <div id="output" class="tryruby-code tryruby-code--output"></div>
  </div>
</div>
