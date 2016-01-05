##Coding Challenge- Find Email Address
Create a command line program that will take an internet domain name
(i.e. “jana.com”) and print out a list of the email addresses that were found
on that website.

##Example:

```
> python find_email_addresses.py jana.com
Found these email addresses:
sales@jana.com
press@jana.com
info@jana.com

```
A basic html parser is incable of scraping the content generated dynamically by executing the javascript therefore a browser emulation is required for rendering the internet domain and fetch the document content. The cached content then can be parsed using html parser with beautiful soup, that allows to navigate the document structure and extract the desires text. For this
purpose currently the program uses the firefox webdriver, using selenium  to emulate the browser environment and perform
the browser related tasks such as visitng url and fetching the document text. I am also looking into an implementation which uses headless webdriver such as PhantomJS,which still lacks some support and therefore a future version can use an implementation of the same.

The program is written in Python3 and requires the same to be installed on users machine for execution.

##Additional Libraries

Following additional libraries are required to run the program.

- BeautifulSoup4:  BeautifulSoup allows for scrapping webpages easy. The Library can be installed by using
the following command.If you’re using Ubuntu Linux, you can install Beautiful Soup with the system
package manager:

  $ [sudo] apt-get install python-bs4

  Beautiful Soup 4 can also be installed with easy_install or pip.

  $ easy_install beautifulsoup4
  $ pip install beautifulsoup4

- Splinter is open source and works with python to emulate the browser actions.

  Splinter can be installed by running the following command from terminal on debian or ubuntu linux.

  $ [sudo] pip install splinter

##Execution:
Run the program from terminal by following command:

> python find_email_addresses.py <domain-name>

example: > python find_email_addresses.py jana.com
