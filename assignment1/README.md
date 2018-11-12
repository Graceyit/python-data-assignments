# JD HUAWEI Mobile Phone Data
## Data Source
HUAWEI's phone information in JD.com: https://list.jd.com/list.html?cat=9987,653,655&ev=exbrand_8557&page=1&sort=sort_rank_asc&trans=1&JL=6_0_0#J_main

## Data fields
* name - string  e.g. 华为mate20 手机 极光色 全网通(6G+64G) 【新品抢购】<br>
* price - float String e.g. 2238.00	<br>
* comment - string e.g. 8万＋<br>
* shop - string e.g. 谷高数码手机专营店 <br>
* type - string e.g. 自营 <br>

## Data Volume
120 rows × 5 columns

## License
CC 4.0

## Obstacles and Solutions 
In the columns of 'comment', there is a word - '万‘ ，so I use df['comment']=df['comment'].str.replace('万','00000') to replace it.
