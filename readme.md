# Principals of Principal Components

See [https://analytic-musings.com/2023/12/31/principles-of-principal-components/](https://analytic-musings.com/2023/12/31/principles-of-principal-components/) for writeup.

I replicate  _Salomon Brother's Principles of Principal Components_ 2000 paper on modern data (yields from 2012-2022), which showed how PCA on the yield curve can be used in bond relative value analysis: to structure curve-neutral butterfly trades free of level and slope bias. 

I first do PCA on the treasury par curve and examine how PC1, PC2 and PC3 capture level, slope and curve, then create butterfly spreads from rolling PCA with 3rd PC loadings as risk weights.

<br>
<br>
<p align='center'>
<img src="pics/10_butterfly.png">
<p align='center'>2s-5s-10s PCA weighted butterfly spreads for 1Y-5Y rolling windows</p align='center'>
</p align='center'>
<br>
<p align='center'>
<img src="pics/8_1yr_spread.png">
<p align='center'>1Y PCA weighted butterfly spreads with regression plots to show level and slope exposure</p align='center'>
</p align='center'>
<br>
<p align='center'>
<img src="pics/6_ssb_ovr.png">
<p align='center'>Original plot from the paper, 4s-10s-27s butterfly from 1997-1998</p align='center'>
</p align='center'>