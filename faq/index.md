---
title: "Frequently Asked Questions (FAQ)"
output: 
  html_document:
    keep_md: true
    theme: cosmo
    includes:
      in_header: header.html   
---


<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css" integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js" integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy" crossorigin="anonymous"></script>


All code for this document is located at [here](https://raw.githubusercontent.com/muschellij2/neuroc/master/faq/index.R).






```{=html}

<div class="accordion" id="accordionExample">
<div class="collapse show" data-parent="#accordionExample">
```



```{=html}

<div class="card-header">
  <h4 class="mb-0">
  <a class="btn btn-primary" role="button" aria-expanded="false" data-toggle="collapse" href="#faq_what_is">What is Neuroconductor?</a>
  </h4>
</div>
<div class="collapse" id="faq_what_is">

<div class="card-body">
```


<!-- ## What is Neuroconductor? -->

Neuroconductor is a GitHub-based repository of R packages generally related to neuroimaging analyses and processing.  The goals for the community are:

1.  Centralize these packages in one place
2.  Provide detailed howtos and tutorials (below) for users to easily set up and start using these packages
3.  Allow for more feedback for feature requests and contributions to these packages

The goals for the package developers are:

1. Provide feedback on packages and features
2. Help developers pass R CMD check with more detailed feedback and pull requests
3. Check packages in a system with 3rd party imaging software (e.g. FSL, Freesurfer, AFNI, etc.) installed

` </div> </div>`{=html}


```{=html}

<div class="card-header">
  <h4 class="mb-0">
  <a class="btn btn-primary" role="button" aria-expanded="false" data-toggle="collapse" href="#faq_what_ops">What operating systems are supported?</a>
  </h4>
</div>
<div class="collapse" id="faq_what_ops">

<div class="card-body">
```


Packages are tested for Unix-based systems, specifically Linux and Mac OSX. 

Although we do not currently support it, [Windows 10 has a Linux subsystem 

Appveyor will check packages on Windows platforms; a small percentage of packages will not be applicable for Windows machine due to intrinsic nature of the non-`R` components of the software.  Therefore, a package submitted to Neuroconductor does not need to pass checks for Windows to be incorporated into the platform.  

However, [Windows 10 currently has a Linux subsystem](https://msdn.microsoft.com/en-us/commandline/wsl/install_guide), which may allow for a working installation of all the dependencies of Neuroconductor.   Although still untested there is a good [tutorial on running FSL on Windows](http://www.nemotos.net/?p=1481) as well as [ANTsR on Windows](https://github.com/stnava/ANTsR/wiki/Installing-ANTsR-in-Windows-10-(along-with-FSL,-Rstudio,-Freesurfer,-etc)).  


As some software in neuroimaging has only implemented versions for *nix-based systems, we will allow users to submit Unix-only R packages, but will encourage them to refactor their code if possible to enable all of Neuroconductor to be cross-platform.


` </div> </div>`{=html}



```{=html}

<div class="card-header">
  <h4 class="mb-0">
  <a class="btn btn-primary" role="button" aria-expanded="false" data-toggle="collapse" href="#faq_who">Who developed Neuroconductor?</a>
  </h4>
</div>
<div class="collapse" id="faq_who">

<div class="card-body">
```


<!-- ## Who developed Neuroconductor? -->

[John Muschelli](http://johnmuschelli.com/), [Jean-Philippe Fortin](https://jfortinbiostats.com/), [Adi Gherman](http://www.jhsph.edu/faculty/directory/profile/3326/adrian-gherman), [Brian Caffo](http://www.bcaffo.com/) and [Ciprian Crainiceanu](http://www.biostat.jhsph.edu/~ccrainic/) all have contributed a significant amount of time to the project.

` </div> </div>`{=html}


```{=html}

<div class="card-header">
  <h4 class="mb-0">
  <a class="btn btn-primary" role="button" aria-expanded="false" data-toggle="collapse" href="#faq_where">Where can I get the code for the tutorial/howto?</a>
  </h4>
</div>
<div class="collapse" id="faq_where">

<div class="card-body">
```


<!-- ## Where can I get the code for the tutorial/howto? -->

All code for the tutorials and installation guides can be located at [https://github.com/muschellij2/neuroc](https://github.com/muschellij2/neuroc).  Pull requests are welcome.   If you would like a specific tutorial or content, please [open an issue](https://github.com/muschellij2/neuroc/issues).  

` </div> </div>`{=html}



```{=html}

<div class="card-header">
  <h4 class="mb-0">
  <a class="btn btn-primary" role="button" aria-expanded="false" data-toggle="collapse" href="#faq_start">Where should I start?</a>
  </h4>
</div>
<div class="collapse" id="faq_start">

<div class="card-body">
```


<!-- ## Where should I start? -->

The workflow is that one would go through [Installation Guides](../index.html), then [Required Readings](../index.html), and then to any specific [Tutorial](../index.html) that a reader would like to learn about. 
` </div> </div>`{=html}



```{=html}

<div class="card-header">
  <h4 class="mb-0">
  <a class="btn btn-primary" role="button" aria-expanded="false" data-toggle="collapse" href="#faq_error">What if something doesn't work?</a>
  </h4>
</div>
<div class="collapse" id="faq_error">

<div class="card-body">
```


Please [open an issue on GitHub](https://github.com/muschellij2/neuroc/issues).  

` </div> </div>`{=html}


`</div> </div>`{=html}
<!-- ## What if something doesn't work? -->

