# 도전에 성공한 것들의 Archive
<a href = "https://lovetoken.github.io">lovetoken</a>  
`r Sys.Date()`  



<br><br>

## Rose plot 

### Using ggplot2 package


```r
d <- data.frame(Angle = 0:35*10, Rate = abs(rnorm(36)))

ggplot(d, aes(x = Angle, y = Rate)) +
  coord_polar(theta = "x", start = -pi/36) +
  geom_bar(stat = "identity") +
  scale_x_continuous(breaks = seq(0, 360, 30))
```

<img src="output/figure/unnamed-chunk-1-1.png" width="80%" style="display: block; margin: auto;" />
