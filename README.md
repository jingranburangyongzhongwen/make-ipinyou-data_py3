# make-ipinyou-data_py3

**English | [简体中文](README.cn.md)**

This project is to formalise the iPinYou RTB data into a standard format for further researches by Python3. I'll give a concise and clear instruction.

## Step 0

Get the dataset from Baidu WebDrive: [http://pan.baidu.com/s/1kTwX2mF](http://pan.baidu.com/s/1kTwX2mF). 

A dozen hours later you'll get the folder `ipinyou.contest.dataset`. Suppose the path to this folder is `~/ipinyou.contest.dataset`

## Step 1

Get `make-ipinyou-data` from [wnzhang/make-ipinyou-data](https://github.com/wnzhang/make-ipinyou-data).

## Step 2

Update the soft link for the folder `ipinyou.contest.dataset` in `original-data`.

```shell
lkf@ubuntu:~/make-ipinyou-data/original-data$ ln -sfn ~/ipinyou.contest.dataset ipinyou.contest.dataset
```

## Step 3

Replace the folder `python` by this repository's. Make sure all Python files have permission 775 or 777:

```shell
lkf@ubuntu:~/make-ipinyou-data/python$ chmod 777 *
```

## Step 4

Under `make-ipinyou-data` folder, just run `make all`. It takes about 30 minutes. Then you will get:

```shell
859M    ./3358
482M    ./2259
1.3G    ./3427
1.4G    ./3386
56K    ./python
5.4G    ./all
1.6G    ./1458
396M    ./2261
804K    ./.git
1.1G    ./3476
4.0K    ./original-data
135M    ./2997
776M    ./2821
14G    .
```

For more details of the dataset, you can refer to [wnzhang/make-ipinyou-data](https://github.com/wnzhang/make-ipinyou-data).