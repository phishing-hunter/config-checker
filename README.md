# Config Checker
This is the Docker image repository for validating [PHOps](https://github.com/phishing-hunter/PHOps).  
The algorithm of the engine that performs domain scoring running on [phishing-hunter](https://www.phishing-hunter.com) is available.  
If you need real-time notification of scoring results, please register an account [here](https://www.phishing-hunter.com/login).  

## Run checker
```bash
$ docker run --rm -it -v $PWD:/work -w /work phishinghunter/config-checker:20220922 /app/checker.py suspicious.yaml /csv/target.csv 500 150
```

## Reference
* [phishing_catcher](https://github.com/x0rz/phishing_catcher)
* [yara_zip_module](https://github.com/stoerchl/yara_zip_module)
