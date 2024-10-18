## OSINT1 Write up: Question and Answer
https://tryhackme.com/r/room/workshoposint

**Question 1:** 
RawSEC aktif dalam mengedalikan acara CTF di seluruh Malaysia. Mereka telah berjaya mengadakan beberapa siri CTF yang telah berlangsung di Utara, Selantan, Sentral dan juga Pantai Timur. Apakah nama CTF paling terbaru diadakan oleh RawSEC dan di manakah acara itu berlangsung?

**Format flag:** 3108{namactf_namatempat}

**Solution:**
- Google search RawSEC
- Head to their Linkedin Page https://www.linkedin.com/company/rawsec-my
- RawSEC are having an event called "Rembulan" at University College TATI
- Flag: 3108{rembulan_UCTATI}

**Question 2:** 
KAMI BANTAH! KAMI BANTAH!

Malayan Union perlu dihapuskan! Kami mahu Raja-Raja kami semula! Mesej bergambar ini untuk menyampaikan berita ini kepada pihak atasan!
https://postimg.cc/7fWKJdsW

**Format flag** : 3108{namatempat}
**Hint:** Johor

**Solution:**
- Based on the Photo and Hint, we know that it is Protest against Malayan Union at Johor
- Asked the following question in ChatGPT: "dimanakah bantahan against Malayan Union diadakan di Johor? Bagi nama lokasi"
- Flag: 3108{Istana_Besar}

**Question 3:**
Where am I ? 
https://drive.google.com/file/d/1aw66UkDVQWr13KBuShpJriacNxZD0ccp/view?usp=sharing

**Format Flag:** CTF{Gallery_Name}
Spaces in the gallery name should be replaced with underscores (_). For example, if the gallery is named National Art Gallery, the flag should be written as: CTF{National_Art_Gallery}.

**Solution:**
- Go to image.google.com to search using photo
- https://www.instagram.com/thelinckl/p/C7F5-EnBrFM/?img_index=5 
- The instagram account shows that it is Ilham Gallery
- Flag: CTF{Ilham Gallery}

**Question 4:**
Could you find the model of the camera used to take the image in question?  (Continued)
This question is a follow-up to the previous one. Please refer to the image provided in Question 3.

**Format Flag:** CTF{Model}
For example, if the model is Samsung Galaxy S21, the flag should be written as: CTF{Samsung_Galaxy_S21}.

**Solutions:**
- Open the downloaded photo with Exif Pilot
- Go to the Exif tab and View the [Model] Row
- Flag: CTF{OPPO_A76}

**Question 5:**
Which date and time was the photo taken?  (Continued)
This question is a follow-up to the previous one. Please refer to the image provided in Question 3.

**Format Flag:** CTF{YYYY-MM-DD_HH:MM:SS}
Note: HH is the hour in 24-hour format, MM is minutes, and SS is seconds.

**Solutions:**
- Open the downloaded photo with Exif Pilot
- Go to the Exif tab and View the [DateTime] Row
- Flag: CTF{2024-04-09_13:52:15}
 
**Question 6:**
Can you find the registration number of the gallery from the image provided in Question 3?  (Continued)

**Flag Format:** CTF{Registration-Number}

**Solutions:**
- Google Search Ilham Gallery
- http://www.ilhamgallery.com/about/
- Flag: CTF{1300502-A}




