### Web crawling

In this task, we assume that you can already code with the Python programming
language, and you will learn Web crawling and JSON RESTful services.

If no specific file is required, create a `report.md` and write down you
thoughts in it.

#### JSON format

What are the fields in [top-pypi-packages-30-days.min.json](./top-pypi-packages-30-days.min.json)?

Write a Python program named `read_pypi_json.py`, which:
1. reads the [top-pypi-packages-30-days.min.json](./top-pypi-packages-30-days.min.json),
2. prints the last_update time of the file, and
3. prints the names of top 10 projects.

See [JSON encoder and decoder](https://docs.python.org/3/library/json.html) for
more information.

#### Web crawling with CVE API

CVE (Common Vulnerabilites and Explosures) records publicly known
information-security vulnerabilities and exposures. To search the CVE list
automatically, write a Python program `cve_crawler.py`, which:
1. uses *requests* package and CVE API,
2. reads keywords (per each line) from [repos.txt](./repos.txt), and
3. returns a JSON file named `keyword.json` for each keyword.

See [Python requests](https://docs.python-requests.org/en/latest/),
[CVE API](https://nvd.nist.gov/developers/vulnerabilities), and
[CVE](https://cve.mitre.org/cve/search_cve_list.html) for more information.
