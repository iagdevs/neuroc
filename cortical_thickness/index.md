# Cortical Thickness Estimation
John Muschelli  
October 3, 2016  




```r
base_fname = "113-01-T1"
orig = file.path("..", 
                 "brain_extraction",
                 paste0(base_fname, "_SS.nii.gz")
)
stub = file.path("..", "tissue_class_segmentation", 
                base_fname)
seg = paste0(stub, "_Seg.nii.gz")
wm_prob = paste0(stub, "_prob_2.nii.gz")
gm_prob = paste0(stub, "_prob_3.nii.gz")
```



```r
s = antsImageRead(seg)
g = antsImageRead(gm_prob)
w = antsImageRead(wm_prob)
out = kellyKapowski(s = s, g = g, w = w, its = 50, r = 0.025, m = 1.5)
cort = extrantsr::ants2oro(out)
```





```r
ortho2(cort)
```

![](index_files/figure-html/plot_cort-1.png)<!-- -->


```r
hist(c(cort[cort > 0]), breaks = 2000)
```

![](index_files/figure-html/hist_cort-1.png)<!-- -->


```r
ortho2(cort, cort > 0.1)
```

![](index_files/figure-html/thresh_cort-1.png)<!-- -->


```r
ortho2(img, cort)
```

![](index_files/figure-html/overlay_cort-1.png)<!-- -->