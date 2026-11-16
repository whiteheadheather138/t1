代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://wru.0kj1m.cn

JOIN users u ON u.id = o.user_id
来源：http://vfx.iojbl.cn

JOIN products p ON p.id = o.product_id;
来源：http://zmw.fktsv.cn

[Q42] 连接条件附加过滤
来源：http://dhi.shangyingyoupin.top

SELECT u.name, o.amount FROM users u
来源：http://nib.nanxinkj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fua.tarul.cn

[Q43] 标量子查询
来源：http://kfk.daria6918.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cci.zhixingplan.top

[Q44] IN 子查询
来源：http://och.yuxming.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vwb.316326.xyz

[Q45] EXISTS 判断存在
来源：http://xyj.shuidangran.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ers.fktsv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://blf.zdbjq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uyk.ydzc1.top

[Q47] 与平均值比较
来源：http://ijl.vehdjk.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dcc.shuidangran.top

[Q48] CTE 公用表表达式
来源：http://nuh.andypj.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ugk.tianlin.xyz

SELECT * FROM t WHERE c > 5;
来源：http://aey.svipenyu.cn

[Q49] 更新单行
来源：http://zov.snrcjt.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lrm.guowangkeji.top

[Q50] 批量更新
来源：http://ywq.gogol.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cvv.pengpengdd.cyou

[Q51] 用子查询更新
来源：http://vhh.zycfv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dat.chenlongwang.top

[Q52] 删除指定行
来源：http://ifo.yj202588.top

DELETE FROM users WHERE id = 10;
来源：http://eqp.xuanzx.com

[Q53] 按条件删除
来源：http://koa.yuanzhike.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jai.birdmap.top

[Q54] 清空表
来源：http://nmv.sxryk.cn

TRUNCATE TABLE logs;
来源：http://xqa.daria6918.cn

[Q55] 排名（并列占位）
来源：http://jyc.cucudq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qhe.52xcode.cn

[Q56] 密集排名（并列不占位）
来源：http://itf.svipenyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rmi.hcnkem.com

[Q57] 行号
来源：http://hfr.sufxvd.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tjp.sysykeji.top

[Q58] 累计求和
来源：http://viy.nanxuanxn.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rcs.fengsongda.top

[Q59] 分组内累计
来源：http://eud.ydzc1.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oti.jianghu66.top

[Q60] 取上一行 / 下一行
来源：http://oip.jyoumei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vqk.gaohongyu789.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://okg.fengsongda.top

[Q61] 移动平均
来源：http://nrh.sxryk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xwr.daxiang520.top

[Q62] 分组占比
来源：http://hdw.aibaodan.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vjj.yuxming.cn

[Q63] 开启事务
来源：http://wgo.sufxvd.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mes.guowangkeji.top

[Q64] 提交事务
来源：http://llw.andypj.xyz

COMMIT;
来源：http://nyp.cqqwz.cn

[Q65] 回滚事务
来源：http://kas.xuetiantiany.cn

ROLLBACK;
来源：http://vry.sufxvd.cn

[Q66] 行锁查询
来源：http://wjz.cqqwz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jvg.cdnleiting.top

[Q67] 设置隔离级别
来源：http://bks.mhx1999.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nvy.dianchejie.cn

[Q68] 保存点
来源：http://sbv.tian-w.cn

SAVEPOINT sp1;
来源：http://ihk.mhx1999.top

ROLLBACK TO sp1;
来源：http://tbo.wangdashe.top

[Q69] 查看执行计划
来源：http://zgn.fengsongda.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://usi.xingfuxueyuan.xyz

[Q70] 更新统计信息
来源：http://jug.feifeiyinyue.top

ANALYZE TABLE users;
来源：http://jeu.chenlongwang.top

[Q71] 查看建表语句
来源：http://xzi.chenzaomai.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pne.kuanghao11.cn

[Q72] 查看索引
来源：http://zls.zhiwuduotai.top

SHOW INDEX FROM users;
来源：http://pjl.pycfn.com

[Q73] 查看表状态
来源：http://sxf.ctjpmb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://ipv.tanke756.top

[Q74] 强制使用索引
来源：http://tzu.fengsongda.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zwe.yuxming.cn

[Q75] 日期格式化
来源：http://ydm.zhiwuduotai.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ffg.bjfxy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pra.hysaishi.cn

[Q76] 按天统计
来源：http://zaq.bbcook.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://aie.zycfv.cn

[Q77] 时间加减
来源：http://gro.zhongyouzk.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jhj.vqdsnc.cn

[Q78] 当前时间
来源：http://dzi.zhengqikj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nfa.sweek.top

[Q79] 字符串拼接
来源：http://rcn.tian-w.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tmi.zdqjudy.top

[Q80] 字符串截取
来源：http://hlv.nwbrower.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ewr.fanxiaobao.xyz

[Q81] 字符串替换
来源：http://kou.svipenyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qun.jyoumei.cn

[Q82] 字符长度与字节长度
来源：http://aup.hcnkem.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jkv.shzxlz.cn

[Q83] 大小写转换
来源：http://kln.fengsongda.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fet.yj20258888.top

[Q84] 去除首尾空格
来源：http://cih.ivvv.top

SELECT TRIM(name) FROM users;
来源：http://aei.sysykeji.top

[Q85] 数值取整
来源：http://rvv.nanxinkj.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hnv.gaohongyu789.top

[Q86] 读取 JSON 字段
来源：http://wqk.epnwcf.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dwn.ybcxt.top

[Q87] JSON 字段做条件
来源：http://gpc.bjfxy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gjf.nanxuanxn.top

[Q88] 行转列（条件聚合）
来源：http://dhe.kuanghao11.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tzj.wangdashe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://use.andypj.xyz

[Q89] 判断表是否存在
来源：http://enm.zhixingplan.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uup.shanyushiyangkeji.top

[Q90] 生成序号列
来源：http://nge.jyoumei.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fhv.ppjwa.cn

================================================================================
来源：http://jha.shuidangran.top

R. Bash 专题
来源：http://cac.ydjk.org.cn

================================================================================
来源：http://lhn.dashuyun.cn

[R01] shebang 与严格模式
来源：http://wge.hongshengwenyu.top

#!/usr/bin/env bash
来源：http://ofw.zycfv.cn

set -euo pipefail
来源：http://zca.zdbjq.cn

[R02] 变量赋值与使用
来源：http://jcg.nwbrower.top

name="Tom"; echo "$name"
来源：http://swi.zhengqikj.top

[R03] 只读变量
来源：http://nzc.zdqjudy.top

readonly PI=3.14
来源：http://lrr.zhijiandao.cn

[R04] 位置参数
来源：http://sfb.pengpengdd.cyou

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hgu.hesvh.cn

[R05] 参数默认值
来源：http://lbp.cashguo.top

name="${1:-default}"
来源：http://rkc.hcnkem.com

[R06] 判断命令是否存在
来源：http://vlw.mhx1999.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tow.quarkkingdee.top

[R07] if 判断文件
来源：http://awy.zycfv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dor.yuxming.cn

[R08] 数值比较
来源：http://eym.xuetiantiany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mrb.ivvv.top

[R09] 字符串比较
来源：http://kty.ppjwa.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nuf.uphjek.com

[R10] 正则匹配
来源：http://eit.birdmap.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rmy.316326.xyz

[R11] case 多分支
来源：http://xiw.sweek.top

case "$1" in
来源：http://tdx.mhx1999.top

start) echo "启动" ;;
来源：http://azc.ydzc1.top

stop)  echo "停止" ;;
来源：http://otj.chenlongwang.top

*)     echo "未知命令" ;;
来源：http://tqe.zycfv.cn

esac
来源：http://use.fanxiaobao.xyz

[R12] for 遍历文件
来源：http://byz.daria6918.cn

for f in *.txt; do echo "$f"; done
来源：http://inf.birdmap.top

[R13] for 计数循环
来源：http://mvw.chenjidiqi.icu

for i in {1..10}; do echo "$i"; done
来源：http://jbd.nanxinkj.top

[R14] C 风格 for
来源：http://xpv.fengsongda.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://git.pycfn.com

[R15] while 逐行读文件
来源：http://kmq.zycfv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qwn.xuanzx.com

[R16] until 等待条件
来源：http://syq.aizwys.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hud.jyoumei.cn

[R17] 数组定义与取值
来源：http://cmd.epnwcf.com

arr=(a b c); echo "${arr[0]}"
来源：http://mhk.ivvv.top

[R18] 遍历数组
来源：http://jle.52xcode.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uwo.andypj.xyz

[R19] 数组长度
来源：http://oax.yanxiufei.cn

echo "${#arr[@]}"
来源：http://fwc.cdnleiting.top

[R20] 关联数组（字典）
来源：http://byn.snrcjt.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tdi.hesvh.cn

[R21] 字符串长度
来源：http://jaz.cheryme.top

echo "${#s}"
来源：http://juz.zhiwuduotai.top

[R22] 截取子串
来源：http://yty.jinqigfzy.top

echo "${s:0:5}"
来源：http://dtg.cashguo.top

[R23] 字符串替换
来源：http://clg.zhiwuduotai.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bfo.bbcook.cn

[R24] 大小写转换
来源：http://mmb.dashuyun.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cye.ppjwa.cn

[R25] 去后缀 / 去前缀
来源：http://ehv.wangdashe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://kvc.iojbl.cn

[R26] 命令替换
来源：http://vew.haohaochexian.top

now=$(date +%F); echo "$now"
来源：http://ikq.hnqzz.top

[R27] 算术展开
来源：http://xsm.xziqi.cn

echo $((1 + 2 * 3))
来源：http://mib.gotoacloud.top

[R28] 浮点运算
来源：http://zps.pycfn.com

echo "scale=2; 10/3" | bc
来源：http://oyb.chenlongwang.top

[R29] 定义函数
来源：http://ypy.aizwys.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kzm.c1oappe.top

[R30] 函数返回状态码
来源：http://adc.guannengcc.top

f() { return 0; }; f || echo "失败了"
来源：http://ces.ydzc1.top

[R31] 局部变量
来源：http://igc.52xcode.cn

f() { local x=1; echo "$x"; }
来源：http://lqs.vehdjk.com

[R32] 参数个数校验
来源：http://mkj.zhijiandao.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rpz.0kj1m.cn

[R33] 捕获错误并提示行号
来源：http://bgz.smart0.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vvh.ivvv.top

[R34] 退出时清理
来源：http://iel.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hgo.svipenyu.cn

[R35] 后台执行并等待
来源：http://tsa.bjfxy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://tdd.redwolf501.top

[R36] 并发执行多个任务
来源：http://zze.52xcode.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xty.pengpengdd.cyou

[R37] 把输出赋给变量
来源：http://tqy.ivvv.top

files=$(ls -1)
来源：http://yva.daxiang520.top

[R38] 管道串联
来源：http://vtf.vqdsnc.cn

cat a.txt | grep -i error | wc -l
来源：http://zhe.fehbvm.com

[R39] 重定向标准输出与错误
来源：http://pib.daria6918.cn

cmd > out.log 2>&1
来源：http://fyv.epnwcf.com

[R40] 追加写日志
来源：http://sou.yj20258.top

echo "log" >> out.log
来源：http://dbw.pengpengdd.cyou

[R41] 丢弃输出
来源：http://tqs.smart0.xyz

cmd >/dev/null 2>&1
来源：http://rjs.svipenyu.cn

[R42] 输入重定向
来源：http://ygj.uphjek.com

wc -l < a.txt
来源：http://qwp.ybcxt.top

[R43] 按名字查找文件
来源：http://kel.ybcxt.top

find . -name "*.log" -type f
来源：http://dsj.redwolf501.top

[R44] 按修改时间查找
来源：http://ffz.tarul.cn

find . -mtime -7 -type f
来源：http://rxi.jinqigfzy.top

[R45] 批量删除
来源：http://sla.gotoacloud.top

find . -name "*.tmp" -delete
来源：http://iww.9152youxi.cn

[R46] 递归替换文件内容
来源：http://zjl.0kj1m.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xta.gogol.net.cn

[R47] sed 单行替换
来源：http://lrc.tanke756.top

sed -i 's/foo/bar/g' a.txt
来源：http://imc.sufxvd.cn

[R48] awk 取指定列
来源：http://avw.havefunace.top

awk '{print $1, $3}' a.txt
来源：http://zjy.sweek.top

[R49] awk 带条件
来源：http://shg.aibaodan.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qlt.hysaishi.cn

[R50] awk 求和
来源：http://zym.chenzaomai.com

awk '{s += $2} END {print s}' a.txt
来源：http://yuh.tarul.cn

[R51] 排序去重取前几
来源：http://dpx.ywan-chungtsiang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rhe.zdqjudy.top

[R52] 统计行数
来源：http://hnb.andypj.xyz

wc -l a.txt
来源：http://uet.cdnleiting.top

[R53] 查看文件头与实时尾
来源：http://yep.hammf.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dxo.nwbrower.top

[R54] 比较两个文件
来源：http://ume.ydzc1.top

diff a.txt b.txt
来源：http://jzw.zhoulong.xyz

[R55] 压缩与解压
来源：http://ueu.nwbrower.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xse.svipenyu.cn

[R56] 远程拷贝
来源：http://rwj.cdnleiting.top

scp file user@host:/path/
来源：http://stn.aibaodan.cn

[R57] 远程执行命令
来源：http://crk.tarul.cn

ssh user@host 'uptime'
来源：http://jjg.jqgufenzy.top

[R58] 下载文件
来源：http://euv.ywan-chungtsiang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eea.guannengcc.top

[R59] 发 POST JSON
来源：http://emz.9152youxi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pyo.jinyuanbaomall.cn

[R60] 只看 HTTP 状态码
来源：http://qvz.jinyuanbaomall.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vto.wangdashe.top

[R61] 磁盘占用
来源：http://tsj.sysykeji.top

df -h;  du -sh *
来源：http://cld.yvedp.cn

[R62] 找最占空间的文件
来源：http://iem.sjlbkw.cn

du -ah . | sort -rh | head -10
来源：http://ojv.mhx1999.top

[R63] 内存与进程
来源：http://sgv.shzxlz.cn

free -h;  ps aux | grep nginx
来源：http://eif.jinghuilouyu.cn

[R64] 结束进程
来源：http://vrp.nwbrower.top

kill -9 $(pgrep -f app.py)
来源：http://qyl.xuetiantiany.cn

[R65] 查看端口占用
来源：http://jrq.fengsongda.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://flc.uphjek.com

[R66] 定时任务
来源：http://ckn.vqdsnc.cn

crontab -e;  crontab -l
来源：http://xtl.yangfankeji.com

[R67] 生成随机十六进制串
来源：http://nvd.yangfankeji.com

openssl rand -hex 16
来源：http://adf.jinqigufen.top

[R68] 计算文件校验值
来源：http://ujs.iojbl.cn

sha256sum a.txt;  md5sum a.txt
来源：http://orc.yonumen.top

[R69] 生成随机密码
来源：http://kdc.shzxlz.cn

head -c 16 /dev/urandom | base64
来源：http://hdv.chenzaomai.com

[R70] 时间戳与互转
来源：http://sou.uphjek.com

date +%s;  date -d @1700000000
来源：http://kcz.mhx1999.top

[R71] 日期格式化
来源：http://msg.gzhubu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://blw.aizwys.cn

[R72] 等待端口就绪
来源：http://iih.pengpengdd.cyou

until nc -z localhost 3306; do sleep 1; done
来源：http://teh.zhaomingkeji.xyz

[R73] 分割大日志
来源：http://slp.sufxvd.cn

split -l 1000 big.log part_
来源：http://qha.shanyushiyangkeji.top

[R74] 批量重命名
来源：http://ssi.fehbvm.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fir.sweek.top

[R75] 导出环境变量
来源：http://jml.jinyuanbaomall.cn

export PATH="$HOME/bin:$PATH"
来源：http://fks.chenlongwang.top

[R76] 使用临时文件
来源：http://rju.nwbrower.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ncz.yonumen.top

[R77] 读取用户输入
来源：http://mxs.wangdashe.top

read -rp "请输入: " ans
来源：http://zbw.ywan-chungtsiang.top

[R78] 交互式菜单
来源：http://axm.xingfuxueyuan.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://hhw.tanke756.top

[R79] 解析命令行选项
来源：http://zam.cashguo.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ztm.daxiang520.top

[R80] 查看脚本执行耗时
来源：http://xly.shangyingyoupin.top

time ./run.sh
来源：http://spc.xziqi.cn

================================================================================
来源：http://rsw.ydzc1.top

S. C / C++ 专题
来源：http://ony.jqgfzy.top

================================================================================
来源：http://nqa.jinqigufen.top

[S01] C：Hello World
来源：http://zeq.pycfn.com

#include <stdio.h>
来源：http://rwx.jianghu66.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://avd.sufxvd.cn

[S02] C：变量与格式化输出
来源：http://npa.tian-w.cn

int a = 10; printf("%d\n", a);
来源：http://yqn.shangyingyoupin.top

[S03] C：读入整数
来源：http://lkx.zhijiandao.cn

int x; scanf("%d", &x);
来源：http://tbu.fanxiaobao.xyz

[S04] C：字符串复制
来源：http://eaf.nanxuanxn.top

char dst[32]; strcpy(dst, "hi");
来源：http://zcn.svipenyu.cn

[S05] C：字符串长度
来源：http://mtx.gaohongyu789.top

strlen(s)
来源：http://xkz.shangyingyoupin.top

[S06] C：字符串比较
来源：http://nwz.yvedp.cn

strcmp(a, b) == 0
来源：http://ynv.ctjpmb.com

[S07] C：数组遍历求和
来源：http://xme.yongpay.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://puv.jinqigfzy.top

[S08] C：动态内存分配与释放
来源：http://woz.yonumen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fzw.svipenyu.cn

[S09] C：结构体定义与初始化
来源：http://cao.hysaishi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qgv.fehbvm.com

[S10] C：指针与解引用
来源：http://xpx.smart0.xyz

int *p = &a;  *p = 5;
来源：http://lhl.zdbjq.cn

[S11] C：逐行读文件
来源：http://pqo.jqgufenzy.top


<!-- 参考信息 -->