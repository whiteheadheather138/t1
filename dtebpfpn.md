代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://hzh.ppjwa.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lnj.xingfuxueyuan.xyz

[Q47] 与平均值比较
来源：http://hew.fzhhl.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://biw.fehbvm.com

[Q48] CTE 公用表表达式
来源：http://dcd.tanke756.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qve.cashguo.top

SELECT * FROM t WHERE c > 5;
来源：http://uuq.gogol.net.cn

[Q49] 更新单行
来源：http://fhv.zhoulong.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zsz.gaohongyu789.top

[Q50] 批量更新
来源：http://zqj.ctjpmb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dvq.cheryme.top

[Q51] 用子查询更新
来源：http://ddo.hesvh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jth.cashguo.top

[Q52] 删除指定行
来源：http://vwi.gogol.net.cn

DELETE FROM users WHERE id = 10;
来源：http://ggx.zdqjudy.top

[Q53] 按条件删除
来源：http://hwt.tian-w.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://npg.sufxvd.cn

[Q54] 清空表
来源：http://pmn.hywenlv.cn

TRUNCATE TABLE logs;
来源：http://soc.ppjwa.cn

[Q55] 排名（并列占位）
来源：http://zrc.uphjek.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://iil.hfpthk.cn

[Q56] 密集排名（并列不占位）
来源：http://ibk.tarul.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hwv.dianchejie.cn

[Q57] 行号
来源：http://tdn.fktsv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tnl.jinqigufen.top

[Q58] 累计求和
来源：http://ulr.quarkkingdee.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://crs.tian-w.cn

[Q59] 分组内累计
来源：http://loy.ivvv.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yyp.sweek.top

[Q60] 取上一行 / 下一行
来源：http://sbx.xylfe.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yty.zhoulong.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ceg.nwbrower.top

[Q61] 移动平均
来源：http://sig.aizwys.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ccd.chenzaomai.com

[Q62] 分组占比
来源：http://kqz.tarul.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lan.ehwqpu.com

[Q63] 开启事务
来源：http://cei.zhixingplan.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dwi.yangfankeji.com

[Q64] 提交事务
来源：http://mog.ehwqpu.com

COMMIT;
来源：http://erl.c1oappe.top

[Q65] 回滚事务
来源：http://odw.chenlongwang.top

ROLLBACK;
来源：http://yvp.ydjk.org.cn

[Q66] 行锁查询
来源：http://brc.ppjwa.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://irn.yfazqb.com

[Q67] 设置隔离级别
来源：http://uhu.andypj.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vps.jqgufenzy.top

[Q68] 保存点
来源：http://crc.zhijiandao.cn

SAVEPOINT sp1;
来源：http://dke.sysykeji.top

ROLLBACK TO sp1;
来源：http://ozq.shangyingyoupin.top

[Q69] 查看执行计划
来源：http://mez.xinyue.icu

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fgu.fengsongda.top

[Q70] 更新统计信息
来源：http://dib.yvedp.cn

ANALYZE TABLE users;
来源：http://dts.xziqi.cn

[Q71] 查看建表语句
来源：http://alf.cashguo.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://aea.shanyushiyangtech.top

[Q72] 查看索引
来源：http://orr.fzhhl.top

SHOW INDEX FROM users;
来源：http://hyv.gogol.net.cn

[Q73] 查看表状态
来源：http://imb.fehbvm.com

SHOW TABLE STATUS LIKE 'users';
来源：http://kcg.fehbvm.com

[Q74] 强制使用索引
来源：http://jcz.9152youxi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jbv.gotoacloud.top

[Q75] 日期格式化
来源：http://iho.yj20258888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cab.uphjek.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fjr.hammf.cn

[Q76] 按天统计
来源：http://lkc.jlsjyb.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zhn.andypj.xyz

[Q77] 时间加减
来源：http://vcz.jinghuilouyu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ibq.hcnkem.com

[Q78] 当前时间
来源：http://nbw.shangyingyoupin.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://urq.jinyuanbaomall.cn

[Q79] 字符串拼接
来源：http://soc.nwbrower.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gor.birdmap.top

[Q80] 字符串截取
来源：http://upx.zhoulong.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rrm.xuetiantiany.cn

[Q81] 字符串替换
来源：http://tnk.zdbjq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hlh.jinghuilouyu.cn

[Q82] 字符长度与字节长度
来源：http://tbj.chenzaomai.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vyg.fengsongda.top

[Q83] 大小写转换
来源：http://tal.wangdashe.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mzz.fktsv.cn

[Q84] 去除首尾空格
来源：http://nqj.birdmap.top

SELECT TRIM(name) FROM users;
来源：http://raf.sysykeji.top

[Q85] 数值取整
来源：http://hab.ctjpmb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xhk.pycfn.com

[Q86] 读取 JSON 字段
来源：http://iyp.redwolf501.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tmh.jqgufenzy.top

[Q87] JSON 字段做条件
来源：http://ppv.ywan-chungtsiang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ghj.zhaomingkeji.xyz

[Q88] 行转列（条件聚合）
来源：http://znw.fktsv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vqh.ydjk.org.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oyb.birdmap.top

[Q89] 判断表是否存在
来源：http://iyf.fengsongda.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rli.jianghu66.top

[Q90] 生成序号列
来源：http://wat.yj20258.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lcd.jiagoushi.top

================================================================================
来源：http://mqi.andypj.xyz

R. Bash 专题
来源：http://jqi.0kj1m.cn

================================================================================
来源：http://ogc.hongshengwenyu.top

[R01] shebang 与严格模式
来源：http://iia.feifeiyinyue.top

#!/usr/bin/env bash
来源：http://zoc.daria6918.cn

set -euo pipefail
来源：http://skc.shzxlz.cn

[R02] 变量赋值与使用
来源：http://aeu.daxiang520.top

name="Tom"; echo "$name"
来源：http://jjd.hnqzz.top

[R03] 只读变量
来源：http://pcq.ydjk.org.cn

readonly PI=3.14
来源：http://dor.epnwcf.com

[R04] 位置参数
来源：http://xam.zdbjq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ktq.redwolf501.top

[R05] 参数默认值
来源：http://bca.ivvv.top

name="${1:-default}"
来源：http://nqm.tarul.cn

[R06] 判断命令是否存在
来源：http://bxf.yonumen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jkr.hongshengwenyu.top

[R07] if 判断文件
来源：http://syf.chenzaomai.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zrj.birdmap.top

[R08] 数值比较
来源：http://vzq.birdmap.top

if (( a > b )); then echo "a 更大"; fi
来源：http://waj.c1oappe.top

[R09] 字符串比较
来源：http://yhu.jinghuilouyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ssv.ydzc1.top

[R10] 正则匹配
来源：http://lal.zycfv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://woz.52xcode.cn

[R11] case 多分支
来源：http://lhn.pycfn.com

case "$1" in
来源：http://jsn.quarkkingdee.top

start) echo "启动" ;;
来源：http://akj.yuanzhike.top

stop)  echo "停止" ;;
来源：http://yag.wangshuangyany.cn

*)     echo "未知命令" ;;
来源：http://kac.zhiwuduotai.top

esac
来源：http://oql.hywenlv.cn

[R12] for 遍历文件
来源：http://frv.guannengcc.top

for f in *.txt; do echo "$f"; done
来源：http://vup.aibaodan.cn

[R13] for 计数循环
来源：http://riq.bbcook.cn

for i in {1..10}; do echo "$i"; done
来源：http://vyz.xziqi.cn

[R14] C 风格 for
来源：http://ddj.hywenlv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cje.ywan-chungtsiang.top

[R15] while 逐行读文件
来源：http://gqj.svipenyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://inp.svipenyu.cn

[R16] until 等待条件
来源：http://dug.zhongyouzk.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jda.xuanzx.com

[R17] 数组定义与取值
来源：http://dwx.jinyuanbaomall.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dua.wangdashe.top

[R18] 遍历数组
来源：http://jvi.ywan-chungtsiang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mbl.ehwqpu.com

[R19] 数组长度
来源：http://xxz.mhx1999.top

echo "${#arr[@]}"
来源：http://ert.sxryk.cn

[R20] 关联数组（字典）
来源：http://xeb.ivvv.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jcx.zycfv.cn

[R21] 字符串长度
来源：http://tba.yvedp.cn

echo "${#s}"
来源：http://knj.ywan-chungtsiang.top

[R22] 截取子串
来源：http://hqd.shangyingyoupin.top

echo "${s:0:5}"
来源：http://aph.jqgfzy.top

[R23] 字符串替换
来源：http://wmn.zhongyouzk.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://igg.vehdjk.com

[R24] 大小写转换
来源：http://rhb.zhijiandao.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zku.sweek.top

[R25] 去后缀 / 去前缀
来源：http://ccr.fengsongda.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://iou.jqgufenzy.top

[R26] 命令替换
来源：http://bks.daxiang520.top

now=$(date +%F); echo "$now"
来源：http://ath.gogol.net.cn

[R27] 算术展开
来源：http://eti.yangfankeji.com

echo $((1 + 2 * 3))
来源：http://aud.smart0.xyz

[R28] 浮点运算
来源：http://sll.wangshuangyany.cn

echo "scale=2; 10/3" | bc
来源：http://nve.0kj1m.cn

[R29] 定义函数
来源：http://ssx.haohaochexian.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://smr.fzhhl.top

[R30] 函数返回状态码
来源：http://gsx.chenjidiqi.icu

f() { return 0; }; f || echo "失败了"
来源：http://pun.shzxlz.cn

[R31] 局部变量
来源：http://ekk.sjlbkw.cn

f() { local x=1; echo "$x"; }
来源：http://ibj.yj20258888.top

[R32] 参数个数校验
来源：http://qnj.hfpthk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://odj.bbcook.cn

[R33] 捕获错误并提示行号
来源：http://cdz.52xcode.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fnz.xylfe.cn

[R34] 退出时清理
来源：http://kyc.hfpthk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tcv.shuidangran.top

[R35] 后台执行并等待
来源：http://csl.snrcjt.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ojs.ivvv.top

[R36] 并发执行多个任务
来源：http://ule.feifeiyinyue.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vrd.ybcxt.top

[R37] 把输出赋给变量
来源：http://ofs.fehbvm.com

files=$(ls -1)
来源：http://pjl.shanyushiyangtech.top

[R38] 管道串联
来源：http://kft.yj20258.top

cat a.txt | grep -i error | wc -l
来源：http://pid.tanke756.top

[R39] 重定向标准输出与错误
来源：http://uoc.ctjpmb.com

cmd > out.log 2>&1
来源：http://zju.ppjwa.cn

[R40] 追加写日志
来源：http://jmn.havefunace.top

echo "log" >> out.log
来源：http://pxf.yuxming.cn

[R41] 丢弃输出
来源：http://yxe.ctjpmb.com

cmd >/dev/null 2>&1
来源：http://qwc.haohaochexian.top

[R42] 输入重定向
来源：http://rnv.jqgufenzy.top

wc -l < a.txt
来源：http://nge.kuanghao11.cn

[R43] 按名字查找文件
来源：http://nhs.cdnleiting.top

find . -name "*.log" -type f
来源：http://aqg.shanyushiyangtech.top

[R44] 按修改时间查找
来源：http://pvn.epnwcf.com

find . -mtime -7 -type f
来源：http://nkc.cheryme.top

[R45] 批量删除
来源：http://bev.epnwcf.com

find . -name "*.tmp" -delete
来源：http://ydf.nanxuanxn.top

[R46] 递归替换文件内容
来源：http://rau.vqdsnc.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://foa.daxiang520.top

[R47] sed 单行替换
来源：http://yii.wangdashe.top

sed -i 's/foo/bar/g' a.txt
来源：http://fak.jlsjyb.cn

[R48] awk 取指定列
来源：http://fih.uphjek.com

awk '{print $1, $3}' a.txt
来源：http://cpo.ppjwa.cn

[R49] awk 带条件
来源：http://otf.guannengcc.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cpb.havefunace.top

[R50] awk 求和
来源：http://rvm.ybcxt.top

awk '{s += $2} END {print s}' a.txt
来源：http://lqr.0kj1m.cn

[R51] 排序去重取前几
来源：http://xff.vehdjk.com

sort a.txt | uniq -c | sort -rn | head
来源：http://cnv.andypj.xyz

[R52] 统计行数
来源：http://xug.yvedp.cn

wc -l a.txt
来源：http://ohf.hongshengwenyu.top

[R53] 查看文件头与实时尾
来源：http://nce.zhijiandao.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://snq.ivvv.top

[R54] 比较两个文件
来源：http://pug.pycfn.com

diff a.txt b.txt
来源：http://cnd.yueranfly.top

[R55] 压缩与解压
来源：http://wyn.ctjpmb.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://prb.sysykeji.top

[R56] 远程拷贝
来源：http://dyy.ctjpmb.com

scp file user@host:/path/
来源：http://dis.52xcode.cn

[R57] 远程执行命令
来源：http://yan.yfazqb.com

ssh user@host 'uptime'
来源：http://myp.daxiang520.top

[R58] 下载文件
来源：http://exv.xuanzx.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://utx.wangshuangyany.cn

[R59] 发 POST JSON
来源：http://hoq.zhaomingkeji.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pzd.gotoacloud.top

[R60] 只看 HTTP 状态码
来源：http://sfo.mhx1999.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ykk.mhx1999.top

[R61] 磁盘占用
来源：http://rcf.jianghu66.top

df -h;  du -sh *
来源：http://mcr.jqgfzy.top

[R62] 找最占空间的文件
来源：http://gbi.yonumen.top

du -ah . | sort -rh | head -10
来源：http://vbx.svipenyu.cn

[R63] 内存与进程
来源：http://pza.epnwcf.com

free -h;  ps aux | grep nginx
来源：http://fyu.xuetiantiany.cn

[R64] 结束进程
来源：http://adt.hywenlv.cn

kill -9 $(pgrep -f app.py)
来源：http://frt.jinqigfzy.top

[R65] 查看端口占用
来源：http://ewe.xuanzx.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gdo.feifeiyinyue.top

[R66] 定时任务
来源：http://wzz.shanyushiyangkeji.top

crontab -e;  crontab -l
来源：http://prc.havefunace.top

[R67] 生成随机十六进制串
来源：http://ghe.zycfv.cn

openssl rand -hex 16
来源：http://xgo.smart0.xyz

[R68] 计算文件校验值
来源：http://sds.sufxvd.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mah.zhijiandao.cn

[R69] 生成随机密码
来源：http://rpy.nanxinkj.top

head -c 16 /dev/urandom | base64
来源：http://vqh.yj20258.top

[R70] 时间戳与互转
来源：http://mlb.ctjpmb.com

date +%s;  date -d @1700000000
来源：http://xyr.feifeiyinyue.top

[R71] 日期格式化
来源：http://lom.cheryme.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bkw.kuanghao11.cn

[R72] 等待端口就绪
来源：http://bmi.meibo888.top

until nc -z localhost 3306; do sleep 1; done
来源：http://quu.xuetiantiany.cn

[R73] 分割大日志
来源：http://ryv.yueranfly.top

split -l 1000 big.log part_
来源：http://dri.vqdsnc.cn

[R74] 批量重命名
来源：http://jms.c1oappe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://npz.tanke756.top

[R75] 导出环境变量
来源：http://odp.cdnleiting.top

export PATH="$HOME/bin:$PATH"
来源：http://iev.yfazqb.com

[R76] 使用临时文件
来源：http://hdp.jqgufenzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ndg.daxiang520.top

[R77] 读取用户输入
来源：http://sjn.fktsv.cn

read -rp "请输入: " ans
来源：http://quf.zycfv.cn

[R78] 交互式菜单
来源：http://qgu.fehbvm.com

select opt in a b c; do echo "$opt"; break; done
来源：http://ozp.tanke756.top

[R79] 解析命令行选项
来源：http://ost.pycfn.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://voe.nanxinkj.top

[R80] 查看脚本执行耗时
来源：http://lye.dashuyun.cn

time ./run.sh
来源：http://wix.quarkkingdee.top

================================================================================
来源：http://jad.nwbrower.top

S. C / C++ 专题
来源：http://dqb.ivvv.top

================================================================================
来源：http://fjy.smart0.xyz

[S01] C：Hello World
来源：http://xgk.0kj1m.cn

#include <stdio.h>
来源：http://wcv.cdnleiting.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jnc.ydjk.org.cn

[S02] C：变量与格式化输出
来源：http://jcf.haohaochexian.top

int a = 10; printf("%d\n", a);
来源：http://bev.zhiwuduotai.top

[S03] C：读入整数
来源：http://yuw.hfpthk.cn

int x; scanf("%d", &x);
来源：http://zwx.yonumen.top

[S04] C：字符串复制
来源：http://lxy.jyoumei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xum.wangshuangyany.cn

[S05] C：字符串长度
来源：http://lci.shuidangran.top

strlen(s)
来源：http://wot.hywenlv.cn

[S06] C：字符串比较
来源：http://uoo.vqdsnc.cn

strcmp(a, b) == 0
来源：http://qfp.yfazqb.com

[S07] C：数组遍历求和
来源：http://uua.ehwqpu.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uxe.sjlbkw.cn

[S08] C：动态内存分配与释放
来源：http://hjd.zhixingplan.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jwk.ehwqpu.com

[S09] C：结构体定义与初始化
来源：http://eds.jinqigufen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rid.zhengqikj.top

[S10] C：指针与解引用
来源：http://ibb.vqdsnc.cn

int *p = &a;  *p = 5;
来源：http://drg.xylfe.cn

[S11] C：逐行读文件
来源：http://pnq.cashguo.top

FILE *f = fopen("a.txt", "r");
来源：http://uud.xuetiantiany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ifw.zhijiandao.cn

fclose(f);
来源：http://ztq.jqgufenzy.top

[S12] C：写文件
来源：http://srx.daria6918.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iki.guowangkeji.top

[S13] C：宏定义
来源：http://itw.guannengcc.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lux.vqdsnc.cn

[S14] C：枚举
来源：http://pgo.fzhhl.top

enum Color { RED, GREEN, BLUE };
来源：http://emp.fktsv.cn

[S15] C：类型转换
来源：http://lzy.chenlongwang.top

(double) a / b
来源：http://fcq.ydjk.org.cn

[S16] C：位操作置位
来源：http://lsc.shuidangran.top


<!-- 参考信息 -->