---
author: AnggiWaSa
category: webdev
date: 2019-01-17 01:30:29
description: Lebih lanjut mengenai z-index
layout: post
tags: css
title: CSS | z-index
---

`z-index` properti CSS menetapkan z-order dari posisi elemen dan keturunannya atau item fleksibel. Elemen yang tumpang tindih dengan indeks z yang lebih besar mencakup elemen yang lebih kecil.

Untuk kotak yang diposisikan (yaitu, satu dengan positionselain dari static), z-indexproperti menentukan:
1.  Tingkat tumpukan kotak dalam konteks penumpukan saat ini .
2. Apakah kotak menetapkan konteks penumpukan lokal.

### Contoh Bagian
#### Bagian HTML
```markup
	<div class="dashed-box">Dashed box
	  <span class="gold-box">Gold box</span>
	  <span class="green-box">Green box</span>
	</div>
```
#### Bagian CSS
```css
	.dashed-box { 
	  position: relative;
	  z-index: 1;
	  border: dashed;
	  height: 8em;
	  margin-bottom: 1em;
	  margin-top: 2em;
	}
	.gold-box { 
	  position: absolute;
	  z-index: 3; /* put .gold-box above .green-box and .dashed-box */
	  background: gold;
	  width: 80%;
	  left: 60px;
	  top: 3em;
	}
	.green-box { 
	  position: absolute;
	  z-index: 2; /* put .green-box above .dashed-box */
	  background: lightgreen;
	  width: 20%;
	  left: 65%;
	  top: -25px;
	  height: 7em;
	  opacity: 0.9;
	}
```
#### Hasil

