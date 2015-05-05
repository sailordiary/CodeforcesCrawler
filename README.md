# CodeforcesCrawler
A python script to crawl problems in [Codeforces](http://codeforces.com/)
##How to use
At first,you should install pdftk and wkhtmltopdf<br>
Then edit crawl_html.py,in bottom,you will find this code
run crawl_html.py to crawl html
```
$python crawl_html.py 1 600 50
```
1 is contest id for begin,600 for end,50 is threads
Wait it finish.<br>
Finally,run html2pdf.py
```
$python html2pdf.py 8
```
8 is threads
Wait a moment,you'll get all problem:
#####problem/
all problem in pdf in here
#####contest/
contest in pdf marge by some problem in same contest
#####html/
origin problem in html without unless element
#####src/
some pricture in problem,html file need it
##Other file
#####clear.sh
remove all file in scr/,html/,problem/,contest/
#####Codeforces_files/
css file is html need,I cache it in this directory
#####header.html
html header with local css file,every file involve it in html/
#####html_list.txt
Generated by crawl_html.py and html2pdf.py read it to generate pdf
