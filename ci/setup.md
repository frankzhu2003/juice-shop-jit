### Install npm

### Install docker
Optional: only for build docker image

### Signup Snyk
https://snyk.io/

### Install Jenkins
1. Install SNYK Jenkins plugin
> Set up Snyk API token

2. Create Freestyle project
> Execute shell
```
# Clones the repository
cd /Users/frankzhu/git/
rm -R juice-shop
git clone https://github.com/frankzhu2003/juice-shop

# Compiles/builds the application
cd /Users/frankzhu/git/juice-shop
pwd
docker build . -t juice-box1
docker image ls

#Compiles/builds the application
npm install
```

> Invoke Snyk Security task
```
Fail the build, if severity at or above Critical
Target file: juice-shop_home/package.json
```

### The Snyk Security Report 
https://github.com/frankzhu2003/juice-shop/blob/master/ci/snyk_report.html

