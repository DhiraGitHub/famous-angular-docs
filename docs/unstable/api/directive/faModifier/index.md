---
layout: "docs_api"
version: "unstable"
versionHref: "/docs/unstable"
path: "api/directive/faModifier/"
title: "fa-modifier"
header_sub_title: "Directive in module famous.angular"
doc: "faModifier"
docType: "directive"
---

<div class="improve-docs">
  <a href='https://github.com/Famous/famous-angular/edit/master/src/scripts/directives/fa-modifier.js#L1'>
    Improve this doc
  </a>
</div>




<h1 class="api-title">

  fa-modifier



</h1>





This directive creates a Famo.us Modifier that will affect all children render nodes.  Its properties can be bound
to numbers (including using Angular's data-binding, though this is discouraged for performance reasons)
or to functions that return numbers.  The latter is  preferred, because the reference to the function is passed
directly on to Famo.us, where only the reference to that function needs to be
watched by Angular instead of needing to $watch the values returned by the function.








  
<h2 id="usage">Usage</h2>
  
```html
<fa-modifier fa-opacity=".25" fa-skew="myScopeSkewVariable" fa-translate="[25, 50, 2]" fa-scale="myScopeFunctionThatReturnsAnArray">
  <!-- Child elements of this fa-modifier will be affected by the values above -->
  <fa-surface>I'm translucent, skewed, rotated, and translated</fa-surface>
</fa-modifier>
```
  
  
<h2 id="api" style="clear:both;">API</h2>

<table class="table" style="margin:0;">
  <thead>
    <tr>
      <th>Attr</th>
      <th>Type</th>
      <th>Details</th>
    </tr>
  </thead>
  <tbody>
    
    <tr>
      <td>
        faRotate
        
        
      </td>
      <td>
        
  <code>Array</code>|<code>function()</code>
      </td>
      <td>
        <p>Array of numbers or function returning an array of numbers to which this Modifier&#39;s rotate should be bound.</p>

        
      </td>
    </tr>
    
    <tr>
      <td>
        faRotateX
        
        
      </td>
      <td>
        
  <code>Number</code>|<code>function()</code>
      </td>
      <td>
        <p>Number or function returning a number to which this Modifier&#39;s rotateX should be bound</p>

        
      </td>
    </tr>
    
    <tr>
      <td>
        faRotateY
        
        
      </td>
      <td>
        
  <code>Number</code>|<code>function()</code>
      </td>
      <td>
        <p>Number or function returning a number to which this Modifier&#39;s rotateY should be bound</p>

        
      </td>
    </tr>
    
    <tr>
      <td>
        faRotateZ
        
        
      </td>
      <td>
        
  <code>Number</code>|<code>function()</code>
      </td>
      <td>
        <p>Number or function returning a number to which this Modifier&#39;s rotateZ should be bound</p>

        
      </td>
    </tr>
    
    <tr>
      <td>
        faScale
        
        
      </td>
      <td>
        
  <code>Array</code>|<code>function()</code>
      </td>
      <td>
        <p>Array of numbers or function returning an array of numbers to which this Modifier&#39;s scale should be bound</p>

        
      </td>
    </tr>
    
    <tr>
      <td>
        faSkew
        
        
      </td>
      <td>
        
  <code>Array</code>|<code>function()</code>
      </td>
      <td>
        <p>Array of numbers or function returning an array of numbers to which this Modifier&#39;s skew should be bound</p>

        
      </td>
    </tr>
    
    <tr>
      <td>
        faTransform
        
        
      </td>
      <td>
        
  <code>Transform</code>
      </td>
      <td>
        <p>Manually created Famo.us Transform object (an array) that can be passed to the modifier</p>

        
      </td>
    </tr>
    
    <tr>
      <td>
        faOpacity
        
        
      </td>
      <td>
        
  <code>Number</code>|<code>function()</code>
      </td>
      <td>
        <p>Number or function returning a number to which this Modifier&#39;s opacity should be bound</p>

        
      </td>
    </tr>
    
    <tr>
      <td>
        faSize
        
        
      </td>
      <td>
        
  <code>Array</code>|<code>function()</code>
      </td>
      <td>
        <p>Array of numbers (e.g. [100, 500] for the x- and y-sizes) or function returning an array of numbers to which this Modifier&#39;s size should be bound</p>

        
      </td>
    </tr>
    
    <tr>
      <td>
        faOrigin
        
        
      </td>
      <td>
        
  <code>Array</code>|<code>function()</code>
      </td>
      <td>
        <p>Array of numbers (e.g. [.5, 0] for the x- and y-origins) or function returning an array of numbers to which this Modifier&#39;s origin should be bound</p>

        
      </td>
    </tr>
    
  </tbody>
</table>

  

  





