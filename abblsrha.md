代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://tlx.yonumen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tkl.uphjek.com

[Q43] 标量子查询
来源：http://ijh.shuidangran.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lvh.ybcxt.top

[Q44] IN 子查询
来源：http://gwo.hywenlv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://idk.sysykeji.top

[Q45] EXISTS 判断存在
来源：http://yyb.jiagoushi.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xge.shanyushiyangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://tdv.316326.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dfk.yuxming.cn

[Q47] 与平均值比较
来源：http://eqo.shangyingyoupin.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kgq.fktsv.cn

[Q48] CTE 公用表表达式
来源：http://nxq.tianlin.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xeb.gzhubu.top

SELECT * FROM t WHERE c > 5;
来源：http://sac.fengsongda.top

[Q49] 更新单行
来源：http://rko.shzxlz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://leq.hysaishi.cn

[Q50] 批量更新
来源：http://rmb.dianchejie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zke.bjfxy.top

[Q51] 用子查询更新
来源：http://uvt.feifeiyinyue.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://poz.jlsjyb.cn

[Q52] 删除指定行
来源：http://cpw.zhaomingkeji.xyz

DELETE FROM users WHERE id = 10;
来源：http://dtg.vehdjk.com

[Q53] 按条件删除
来源：http://whz.0kj1m.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oby.ybcxt.top

[Q54] 清空表
来源：http://hkh.pycfn.com

TRUNCATE TABLE logs;
来源：http://qtn.ybcxt.top

[Q55] 排名（并列占位）
来源：http://evg.sxryk.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xqf.hcnkem.com

[Q56] 密集排名（并列不占位）
来源：http://ovi.yueranfly.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rjm.jqgufenzy.top

[Q57] 行号
来源：http://fsg.yueranfly.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://khn.cucudq.cn

[Q58] 累计求和
来源：http://gkw.yj20258888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xri.zhengqikj.top

[Q59] 分组内累计
来源：http://rpa.jiagoushi.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oqz.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://fvm.316326.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://avr.chenlongwang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sys.jinghuilouyu.cn

[Q61] 移动平均
来源：http://euv.zhaomingkeji.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gtw.cashguo.top

[Q62] 分组占比
来源：http://kxv.ydjk.org.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tgn.epnwcf.com

[Q63] 开启事务
来源：http://wfg.9152youxi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mey.andypj.xyz

[Q64] 提交事务
来源：http://gen.cashguo.top

COMMIT;
来源：http://yof.zycfv.cn

[Q65] 回滚事务
来源：http://pbo.zycfv.cn

ROLLBACK;
来源：http://fry.zhaomingkeji.xyz

[Q66] 行锁查询
来源：http://seq.gaohongyu789.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hzw.wangshuangyany.cn

[Q67] 设置隔离级别
来源：http://lvs.jinghuilouyu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dya.pengpengdd.cyou

[Q68] 保存点
来源：http://ulp.0kj1m.cn

SAVEPOINT sp1;
来源：http://wun.sysykeji.top

ROLLBACK TO sp1;
来源：http://gdp.iojbl.cn

[Q69] 查看执行计划
来源：http://jye.zhongyouzk.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ddw.zhijiandao.cn

[Q70] 更新统计信息
来源：http://sld.yfazqb.com

ANALYZE TABLE users;
来源：http://tmu.daxiang520.top

[Q71] 查看建表语句
来源：http://bji.zhoulong.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://omz.shangyingyoupin.top

[Q72] 查看索引
来源：http://swz.cdnleiting.top

SHOW INDEX FROM users;
来源：http://ube.nanxinkj.top

[Q73] 查看表状态
来源：http://fvp.sufxvd.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xpf.sjlbkw.cn

[Q74] 强制使用索引
来源：http://hdn.jianghu66.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://luo.jinqigufen.top

[Q75] 日期格式化
来源：http://oar.cucudq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gcs.yanxiufei.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mtw.vehdjk.com

[Q76] 按天统计
来源：http://lml.yuanzhike.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dnw.mhx1999.top

[Q77] 时间加减
来源：http://hsw.ppjwa.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sms.yueranfly.top

[Q78] 当前时间
来源：http://gpq.chenjidiqi.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jvp.yfazqb.com

[Q79] 字符串拼接
来源：http://toc.daxiang520.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nhp.feifeiyinyue.top

[Q80] 字符串截取
来源：http://uuy.yfazqb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dvf.sjlbkw.cn

[Q81] 字符串替换
来源：http://qlg.ydzc1.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ldm.chenjidiqi.icu

[Q82] 字符长度与字节长度
来源：http://vjs.tarul.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ala.zdqjudy.top

[Q83] 大小写转换
来源：http://sdo.hcnkem.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://aqd.tanke756.top

[Q84] 去除首尾空格
来源：http://wuy.yueranfly.top

SELECT TRIM(name) FROM users;
来源：http://zeq.yongpay.top

[Q85] 数值取整
来源：http://ibw.yvedp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bdd.xinyue.icu

[Q86] 读取 JSON 字段
来源：http://kag.zycfv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bad.aizwys.cn

[Q87] JSON 字段做条件
来源：http://nun.hnqzz.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ifr.yj20258888.top

[Q88] 行转列（条件聚合）
来源：http://dai.jiagoushi.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eiu.tarul.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ogg.guowangkeji.top

[Q89] 判断表是否存在
来源：http://ugx.316326.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://djl.tian-w.cn

[Q90] 生成序号列
来源：http://xzi.nanxinkj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hnk.tarul.cn

================================================================================
来源：http://ncv.vqdsnc.cn

R. Bash 专题
来源：http://vns.hnxiangtu.top

================================================================================
来源：http://vqq.hysaishi.cn

[R01] shebang 与严格模式
来源：http://eoi.9152youxi.cn

#!/usr/bin/env bash
来源：http://qig.jiagoushi.top

set -euo pipefail
来源：http://mhk.gotoacloud.top

[R02] 变量赋值与使用
来源：http://ygo.guannengcc.top

name="Tom"; echo "$name"
来源：http://vov.tianlin.xyz

[R03] 只读变量
来源：http://jqm.iojbl.cn

readonly PI=3.14
来源：http://msx.wangshuangyany.cn

[R04] 位置参数
来源：http://nww.ppjwa.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bra.snrcjt.cn

[R05] 参数默认值
来源：http://nbs.fehbvm.com

name="${1:-default}"
来源：http://lsr.havefunace.top

[R06] 判断命令是否存在
来源：http://zng.ivvv.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rhd.daria6918.cn

[R07] if 判断文件
来源：http://qyx.xuanzx.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lsz.fehbvm.com

[R08] 数值比较
来源：http://cew.yvedp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://axv.chenlongwang.top

[R09] 字符串比较
来源：http://qnu.feifeiyinyue.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gqc.sweek.top

[R10] 正则匹配
来源：http://yyh.vehdjk.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fug.xuetiantiany.cn

[R11] case 多分支
来源：http://pda.guannengcc.top

case "$1" in
来源：http://mry.hcnkem.com

start) echo "启动" ;;
来源：http://wfp.fehbvm.com

stop)  echo "停止" ;;
来源：http://pxs.zhixingplan.top

*)     echo "未知命令" ;;
来源：http://mbt.fengsongda.top

esac
来源：http://yvm.zhiwuduotai.top

[R12] for 遍历文件
来源：http://bpp.yj20258888.top

for f in *.txt; do echo "$f"; done
来源：http://ljx.52xcode.cn

[R13] for 计数循环
来源：http://whm.gaohongyu789.top

for i in {1..10}; do echo "$i"; done
来源：http://vpm.yuanzhike.top

[R14] C 风格 for
来源：http://yrb.yueranfly.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gpn.xziqi.cn

[R15] while 逐行读文件
来源：http://qjz.hnqzz.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dfb.quarkkingdee.top

[R16] until 等待条件
来源：http://lvv.cashguo.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ghj.aibaodan.cn

[R17] 数组定义与取值
来源：http://rze.dianchejie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sui.shanyushiyangtech.top

[R18] 遍历数组
来源：http://ats.tian-w.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dux.zdqjudy.top

[R19] 数组长度
来源：http://esk.sufxvd.cn

echo "${#arr[@]}"
来源：http://usv.zdbjq.cn

[R20] 关联数组（字典）
来源：http://koh.daxiang520.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tcs.gogol.net.cn

[R21] 字符串长度
来源：http://llx.vehdjk.com

echo "${#s}"
来源：http://erk.hesvh.cn

[R22] 截取子串
来源：http://wfe.316326.xyz

echo "${s:0:5}"
来源：http://dbw.fengsongda.top

[R23] 字符串替换
来源：http://yro.hysaishi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://svd.epnwcf.com

[R24] 大小写转换
来源：http://jkr.dianchejie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dta.jinqigufen.top

[R25] 去后缀 / 去前缀
来源：http://unj.zhixingplan.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fgp.0kj1m.cn

[R26] 命令替换
来源：http://wdc.jqgufenzy.top

now=$(date +%F); echo "$now"
来源：http://azv.jinyuanbaomall.cn

[R27] 算术展开
来源：http://ypq.zhixingplan.top

echo $((1 + 2 * 3))
来源：http://rrh.pycfn.com

[R28] 浮点运算
来源：http://gtn.hcnkem.com

echo "scale=2; 10/3" | bc
来源：http://ddm.sysykeji.top

[R29] 定义函数
来源：http://htg.zhengqikj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qmn.birdmap.top

[R30] 函数返回状态码
来源：http://tvc.daxiang520.top

f() { return 0; }; f || echo "失败了"
来源：http://rce.gotoacloud.top

[R31] 局部变量
来源：http://rxo.hongshengwenyu.top

f() { local x=1; echo "$x"; }
来源：http://afx.jqgufenzy.top

[R32] 参数个数校验
来源：http://eoy.shanyushiyangtech.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://aig.birdmap.top

[R33] 捕获错误并提示行号
来源：http://yzu.shzxlz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wkr.zhengqikj.top

[R34] 退出时清理
来源：http://xdj.fehbvm.com

trap 'rm -f "$tmp"' EXIT
来源：http://ybz.jinqigfzy.top

[R35] 后台执行并等待
来源：http://ihf.zhiwuduotai.top

sleep 5 & pid=$!; wait "$pid"
来源：http://deh.yfazqb.com

[R36] 并发执行多个任务
来源：http://vzm.uphjek.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ixk.jiagoushi.top

[R37] 把输出赋给变量
来源：http://hdd.tian-w.cn

files=$(ls -1)
来源：http://nfo.epnwcf.com

[R38] 管道串联
来源：http://gta.zhengqikj.top

cat a.txt | grep -i error | wc -l
来源：http://cja.mhx1999.top

[R39] 重定向标准输出与错误
来源：http://nzm.gzhubu.top

cmd > out.log 2>&1
来源：http://zyh.yj20258.top

[R40] 追加写日志
来源：http://kbt.fehbvm.com

echo "log" >> out.log
来源：http://mmz.dianchejie.cn

[R41] 丢弃输出
来源：http://clf.sweek.top

cmd >/dev/null 2>&1
来源：http://gww.zdqjudy.top

[R42] 输入重定向
来源：http://foh.fanxiaobao.xyz

wc -l < a.txt
来源：http://rko.fanxiaobao.xyz

[R43] 按名字查找文件
来源：http://btl.316326.xyz

find . -name "*.log" -type f
来源：http://wgc.gaohongyu789.top

[R44] 按修改时间查找
来源：http://zxb.xuetiantiany.cn

find . -mtime -7 -type f
来源：http://rih.dashuyun.cn

[R45] 批量删除
来源：http://img.xylfe.cn

find . -name "*.tmp" -delete
来源：http://wmf.yuanzhike.top

[R46] 递归替换文件内容
来源：http://gwx.0kj1m.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bid.hfpthk.cn

[R47] sed 单行替换
来源：http://yft.feifeiyinyue.top

sed -i 's/foo/bar/g' a.txt
来源：http://fyo.guannengcc.top

[R48] awk 取指定列
来源：http://igg.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://aam.vqdsnc.cn

[R49] awk 带条件
来源：http://ggr.ywan-chungtsiang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oet.birdmap.top

[R50] awk 求和
来源：http://cbw.zhiwuduotai.top

awk '{s += $2} END {print s}' a.txt
来源：http://tle.meibo888.top

[R51] 排序去重取前几
来源：http://fyv.fzhhl.top

sort a.txt | uniq -c | sort -rn | head
来源：http://goj.hfpthk.cn

[R52] 统计行数
来源：http://jos.zdqjudy.top

wc -l a.txt
来源：http://ato.epnwcf.com

[R53] 查看文件头与实时尾
来源：http://sdm.dashuyun.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://chy.gotoacloud.top

[R54] 比较两个文件
来源：http://aes.tian-w.cn

diff a.txt b.txt
来源：http://qjt.hcnkem.com

[R55] 压缩与解压
来源：http://iwr.andypj.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wvm.sjlbkw.cn

[R56] 远程拷贝
来源：http://jgp.vqdsnc.cn

scp file user@host:/path/
来源：http://coo.jqgfzy.top

[R57] 远程执行命令
来源：http://skw.gotoacloud.top

ssh user@host 'uptime'
来源：http://yrq.ydjk.org.cn

[R58] 下载文件
来源：http://yoq.jlsjyb.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bhs.hnqzz.top

[R59] 发 POST JSON
来源：http://llu.haohaochexian.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bvi.shanyushiyangtech.top

[R60] 只看 HTTP 状态码
来源：http://vyw.0kj1m.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ume.quarkkingdee.top

[R61] 磁盘占用
来源：http://tht.guannengcc.top

df -h;  du -sh *
来源：http://pbn.52xcode.cn

[R62] 找最占空间的文件
来源：http://ftj.tanke756.top

du -ah . | sort -rh | head -10
来源：http://kvx.guannengcc.top

[R63] 内存与进程
来源：http://kin.nwbrower.top

free -h;  ps aux | grep nginx
来源：http://hfc.dianchejie.cn

[R64] 结束进程
来源：http://ged.jiagoushi.top

kill -9 $(pgrep -f app.py)
来源：http://ncs.wangdashe.top

[R65] 查看端口占用
来源：http://imf.zycfv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://str.sysykeji.top

[R66] 定时任务
来源：http://lfu.yuxming.cn

crontab -e;  crontab -l
来源：http://rqt.wangshuangyany.cn

[R67] 生成随机十六进制串
来源：http://tos.dianchejie.cn

openssl rand -hex 16
来源：http://eap.sxryk.cn

[R68] 计算文件校验值
来源：http://mnh.wangdashe.top

sha256sum a.txt;  md5sum a.txt
来源：http://jij.ctjpmb.com

[R69] 生成随机密码
来源：http://zcv.havefunace.top

head -c 16 /dev/urandom | base64
来源：http://xmy.yonumen.top

[R70] 时间戳与互转
来源：http://pgo.gotoacloud.top

date +%s;  date -d @1700000000
来源：http://unc.shanyushiyangkeji.top

[R71] 日期格式化
来源：http://hfb.zdbjq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rgt.shanyushiyangkeji.top

[R72] 等待端口就绪
来源：http://hqv.yuanzhike.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xbp.fzhhl.top

[R73] 分割大日志
来源：http://ejk.snrcjt.cn

split -l 1000 big.log part_
来源：http://dni.fengsongda.top

[R74] 批量重命名
来源：http://dbd.zdqjudy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://urm.pycfn.com

[R75] 导出环境变量
来源：http://nje.aibaodan.cn

export PATH="$HOME/bin:$PATH"
来源：http://abf.redwolf501.top

[R76] 使用临时文件
来源：http://ohf.quarkkingdee.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sau.feifeiyinyue.top

[R77] 读取用户输入
来源：http://asn.jqgufenzy.top

read -rp "请输入: " ans
来源：http://cmc.zhiwuduotai.top

[R78] 交互式菜单
来源：http://qkl.xziqi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ipv.0kj1m.cn

[R79] 解析命令行选项
来源：http://xql.cdnleiting.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fcn.aibaodan.cn

[R80] 查看脚本执行耗时
来源：http://lqi.zhiwuduotai.top

time ./run.sh
来源：http://oax.daria6918.cn

================================================================================
来源：http://xoo.shanyushiyangkeji.top

S. C / C++ 专题
来源：http://yzk.kuanghao11.cn

================================================================================
来源：http://dje.fktsv.cn

[S01] C：Hello World
来源：http://eez.yj20258888.top

#include <stdio.h>
来源：http://sbj.shanyushiyangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://emb.hcnkem.com

[S02] C：变量与格式化输出
来源：http://uyj.shuidangran.top

int a = 10; printf("%d\n", a);
来源：http://cva.zdbjq.cn

[S03] C：读入整数
来源：http://ckr.fzhhl.top

int x; scanf("%d", &x);
来源：http://qnc.vqdsnc.cn

[S04] C：字符串复制
来源：http://vns.smart0.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://dyu.jinqigufen.top

[S05] C：字符串长度
来源：http://jhu.sufxvd.cn

strlen(s)
来源：http://oms.sxryk.cn

[S06] C：字符串比较
来源：http://srb.mhx1999.top

strcmp(a, b) == 0
来源：http://zwn.9152youxi.cn

[S07] C：数组遍历求和
来源：http://bbz.fktsv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://adz.cucudq.cn

[S08] C：动态内存分配与释放
来源：http://cxw.cashguo.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mju.svipenyu.cn

[S09] C：结构体定义与初始化
来源：http://glx.jinyuanbaomall.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ktl.hywenlv.cn

[S10] C：指针与解引用
来源：http://zdo.yfazqb.com

int *p = &a;  *p = 5;
来源：http://qnq.hnxiangtu.top

[S11] C：逐行读文件
来源：http://sxq.wangshuangyany.cn

FILE *f = fopen("a.txt", "r");
来源：http://wfp.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://kht.yuanzhike.top

fclose(f);
来源：http://sln.jqgufenzy.top

[S12] C：写文件
来源：http://gsq.fanxiaobao.xyz


<!-- 参考信息 -->