### Install npm

### Install docker

### Install Jenkins
1. Install SNYK Jenkins plugin
> Set up Snyk API token

2. Create Freestyle project
> Execute shell
```
cd /Users/frankzhu/git/
rm -R juice-shop
git clone https://github.com/frankzhu2003/juice-shop

cd /Users/frankzhu/git/juice-shop
pwd
docker build . -t juice-box1
docker image ls
npm install
```

> Invoke Snyk Security task
```
Fail the build, if severity at or above Critical
Target file: juice-shop_home/package.json
```

### The Snyk Security Report
![Juice Shop Logo]((https://github.com/frankzhu2003/juice-shop/blob/master/ci/snyk_report.html)
