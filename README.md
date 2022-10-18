# web-scraping-Yellowpage.com-using-beautifulSoup-and-Requests

**Introduction**
There is a vast amount of data available on the internet, most of it is in the unstructured format those data cannot be used directly to build a model .So industries find a way to extract meaningful information from unstructured data. This is where web scraping comes into the picture.

**What is yellowpages.com?**

Yellowpages.com is a United States-based web site operated by Thryv that provides listings for local businesses. In 2013, it was re-branded as YP.com or simply "YP". It currently offers a broad range of marketing tools including online presence, local search, display ads and direct marketing.

**Outline of the Project**

In this project we created more than 10 reusable functins and 3 main function .The steps we followed in this project is as bellow.

**Step:-1** Select the suitable page_url and Install the required Python libraries.

**Step:-2** Assign that page to BeautifulSoup library from request to parse the html page and convert them into html doc format to scraope the information.

**Step:-3** select the suitable tag which contains required informations.

**Step:-4** creating the reusable Functions from parsed htnl doc.Here we extracted the information in two parts,

**For part-1 tags are** parsed from main url pages they are ,

**get_name(doc)**

**get_Phone(doc)**

**get_address(doc)**

**get_online(doc)**

**get_info_web(doc)**


**Part-2 below tags are extracted** from each hotel info_web tag urls 

**6. get_Cuisine(doc1)** 

**7. get_payment(doc1)**

**8. get_neighborhoods(doc1)**


**Step:-5** create a reusable function which returns list of urls to extract tags from multiple pages

**Step:6** Create main function as get_main_page_tags() which loop over the multiple pages and get each part-1 tags ,get information and return them in the data frame format.And assign that function as df_1

**Step:-7** cretae one more main function as get_individual_page_tags() to loop over the each part-2 tags and return them in datarame format.And assign that function as df_2

**Step:-8** create final main function as scrape_yellowpages() to merge all tags exrtacted from above two main functions return them in csv format


Check out jupayter notebook here:  https://jovian.ai/yogeeshtr26/web-scraping-project
