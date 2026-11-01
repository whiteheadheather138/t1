代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.yfazqb.com/Article/details/gnhyzuulb.sHtML

[Q58] 累计求和
来源：http://m.share.sjlbkw.cn/Article/details/gicyrhxlo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gkfbirxhw.sHtML

[Q59] 分组内累计
来源：http://www.blog.epnwcf.com/Article/details/gzhiljxbk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gpfejpnvx.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.vehdjk.com/Article/details/gcbsagfbw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.yfazqb.com/Article/details/gsnuuwykb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fktsv.cn/Article/details/gdjoxwamt.sHtML

[Q61] 移动平均
来源：http://www.share.epnwcf.com/Article/details/grzlrcznr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gvefcqqkw.sHtML

[Q62] 分组占比
来源：http://read.share.bbcook.cn/Article/details/gutvltxzq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/gwjjzadsr.sHtML

[Q63] 开启事务
来源：http://www.blog.sjlbkw.cn/Article/details/gavuqxjzt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.yfazqb.com/Article/details/gqyirxlzs.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/ghumhszjb.sHtML

COMMIT;
来源：http://3g.epnwcf.com/Article/details/gojjpncjm.sHtML

[Q65] 回滚事务
来源：http://www.share.epnwcf.com/Article/details/gaiqtneqk.sHtML

ROLLBACK;
来源：http://3g.sjlbkw.cn/Article/details/gnabveios.sHtML

[Q66] 行锁查询
来源：http://www.m.share.yfazqb.com/Article/details/gxawzhile.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.bbcook.cn/Article/details/gbgjuqnwe.sHtML

[Q67] 设置隔离级别
来源：http://wap.yfazqb.com/Article/details/gqqfbwnyg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.vehdjk.com/Article/details/giucqbjow.sHtML

[Q68] 保存点
来源：http://www.share.vehdjk.com/Article/details/giokjslka.sHtML

SAVEPOINT sp1;
来源：http://blog.sjlbkw.cn/Article/details/gqoerptna.sHtML

ROLLBACK TO sp1;
来源：http://wap.fktsv.cn/Article/details/gvmvgjtrm.sHtML

[Q69] 查看执行计划
来源：http://www.blog.sjlbkw.cn/Article/details/gxovcnnzx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.yfazqb.com/Article/details/geexrmyag.sHtML

[Q70] 更新统计信息
来源：http://www.share.fktsv.cn/Article/details/gidpijjxd.sHtML

ANALYZE TABLE users;
来源：http://m.share.yfazqb.com/Article/details/gkrzflilj.sHtML

[Q71] 查看建表语句
来源：http://read.share.yfazqb.com/Article/details/gavmcktbo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.epnwcf.com/Article/details/gyykapnav.sHtML

[Q72] 查看索引
来源：http://wap.yfazqb.com/Article/details/ghtovwmuw.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gvdehqhuu.sHtML

[Q73] 查看表状态
来源：http://www.share.bbcook.cn/Article/details/gewxqdjny.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.vehdjk.com/Article/details/gmcubejqf.sHtML

[Q74] 强制使用索引
来源：http://mobile.epnwcf.com/Article/details/gmxgtltlq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.vehdjk.com/Article/details/gmbckrjyi.sHtML

[Q75] 日期格式化
来源：http://read.share.sjlbkw.cn/Article/details/goxmedkga.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/ghafsefao.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.bbcook.cn/Article/details/gwbaqbpnr.sHtML

[Q76] 按天统计
来源：http://wap.yfazqb.com/Article/details/gikghtzly.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.epnwcf.com/Article/details/gjslbgqxc.sHtML

[Q77] 时间加减
来源：http://www.blog.epnwcf.com/Article/details/gdvhqxctg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.tarul.cn/Article/details/geiwmfnbo.sHtML

[Q78] 当前时间
来源：http://baike.fktsv.cn/Article/details/grnlkuaua.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.epnwcf.com/Article/details/gfnmrtkbu.sHtML

[Q79] 字符串拼接
来源：http://3g.yfazqb.com/Article/details/gegoilhrq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.sjlbkw.cn/Article/details/gxbramtkc.sHtML

[Q80] 字符串截取
来源：http://www.blog.fktsv.cn/Article/details/ggcwgzchg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.vehdjk.com/Article/details/grayvnqeh.sHtML

[Q81] 字符串替换
来源：http://baike.bbcook.cn/Article/details/gyumbjdtx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.bbcook.cn/Article/details/gacbguzut.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fktsv.cn/Article/details/grwkufcak.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gpjdjguba.sHtML

[Q83] 大小写转换
来源：http://blog.tarul.cn/Article/details/gczwwjstl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/ggtupkjsm.sHtML

[Q84] 去除首尾空格
来源：http://www.share.bbcook.cn/Article/details/gzdpfzoyg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gzthiatad.sHtML

[Q85] 数值取整
来源：http://mobile.sjlbkw.cn/Article/details/gfuviqdbc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.vehdjk.com/Article/details/glafqobrz.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.sjlbkw.cn/Article/details/gqiqohbbs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.sjlbkw.cn/Article/details/ghzdkehgv.sHtML

[Q87] JSON 字段做条件
来源：http://baike.sjlbkw.cn/Article/details/gospmfpgr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fktsv.cn/Article/details/ghoyeqaqe.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.yfazqb.com/Article/details/gbrhulzga.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.yfazqb.com/Article/details/gbgtlxxer.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.yfazqb.com/Article/details/gsrhxgoll.sHtML

[Q89] 判断表是否存在
来源：http://mobile.vehdjk.com/Article/details/gzruazzuc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.vehdjk.com/Article/details/gdztfkago.sHtML

[Q90] 生成序号列
来源：http://mobile.vehdjk.com/Article/details/gauynlbyi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.bbcook.cn/Article/details/gqkwncydj.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/guxhzunpd.sHtML

R. Bash 专题
来源：http://blog.vehdjk.com/Article/details/gabvisyhy.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gxnrdyvxc.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fktsv.cn/Article/details/gsleghjgt.sHtML

#!/usr/bin/env bash
来源：http://read.share.bbcook.cn/Article/details/gaevwvlrh.sHtML

set -euo pipefail
来源：http://wap.epnwcf.com/Article/details/gagixsuig.sHtML

[R02] 变量赋值与使用
来源：http://blog.sjlbkw.cn/Article/details/gejgbxntl.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.sjlbkw.cn/Article/details/gvnwlgiag.sHtML

[R03] 只读变量
来源：http://wap.epnwcf.com/Article/details/gxhqmajey.sHtML

readonly PI=3.14
来源：http://blog.fktsv.cn/Article/details/gbelzhhhk.sHtML

[R04] 位置参数
来源：http://read.share.sjlbkw.cn/Article/details/gvcopkucx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.yfazqb.com/Article/details/genlzprle.sHtML

[R05] 参数默认值
来源：http://mobile.sjlbkw.cn/Article/details/ghxdqrrek.sHtML

name="${1:-default}"
来源：http://wap.bbcook.cn/Article/details/gvhtjbxud.sHtML

[R06] 判断命令是否存在
来源：http://wap.epnwcf.com/Article/details/gcyfoclba.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/gjhalwthc.sHtML

[R07] if 判断文件
来源：http://3g.yfazqb.com/Article/details/gihkrnvwr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.bbcook.cn/Article/details/gjqpujxju.sHtML

[R08] 数值比较
来源：http://baike.yfazqb.com/Article/details/giltndphf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.vehdjk.com/Article/details/gyiwktuhv.sHtML

[R09] 字符串比较
来源：http://baike.yfazqb.com/Article/details/gcuhoryse.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.vehdjk.com/Article/details/gjuyxmvcm.sHtML

[R10] 正则匹配
来源：http://3g.sjlbkw.cn/Article/details/gntnrsvrw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.sjlbkw.cn/Article/details/gafejyrhe.sHtML

[R11] case 多分支
来源：http://3g.bbcook.cn/Article/details/gkuuzanaa.sHtML

case "$1" in
来源：http://www.blog.sjlbkw.cn/Article/details/gxurvsykd.sHtML

start) echo "启动" ;;
来源：http://wap.bbcook.cn/Article/details/gmjhezywu.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.yfazqb.com/Article/details/gzujlfbre.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.tarul.cn/Article/details/gxwvcnjln.sHtML

esac
来源：http://www.m.share.tarul.cn/Article/details/gahylxtrl.sHtML

[R12] for 遍历文件
来源：http://read.share.tarul.cn/Article/details/gafaxqpfk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.bbcook.cn/Article/details/gytnlwqap.sHtML

[R13] for 计数循环
来源：http://baike.vehdjk.com/Article/details/gfwbdohdp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.yfazqb.com/Article/details/gutisiuhx.sHtML

[R14] C 风格 for
来源：http://3g.tarul.cn/Article/details/gahhryevj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/gqigfyuld.sHtML

[R15] while 逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gozmarplo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.tarul.cn/Article/details/guimduarv.sHtML

[R16] until 等待条件
来源：http://www.m.share.bbcook.cn/Article/details/gimtpmgwm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gtabpbyae.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fktsv.cn/Article/details/gqiiqqjfa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fktsv.cn/Article/details/goyzzkedp.sHtML

[R18] 遍历数组
来源：http://m.share.vehdjk.com/Article/details/gkvtbcxwb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.bbcook.cn/Article/details/gigjnggwj.sHtML

[R19] 数组长度
来源：http://mobile.fktsv.cn/Article/details/gyfstvtox.sHtML

echo "${#arr[@]}"
来源：http://baike.fktsv.cn/Article/details/ggjxijpxv.sHtML

[R20] 关联数组（字典）
来源：http://blog.sjlbkw.cn/Article/details/gfvrddirw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.tarul.cn/Article/details/gfluvcrjk.sHtML

[R21] 字符串长度
来源：http://www.share.fktsv.cn/Article/details/gqeirwgox.sHtML

echo "${#s}"
来源：http://mobile.bbcook.cn/Article/details/gfiwzqwkq.sHtML

[R22] 截取子串
来源：http://3g.tarul.cn/Article/details/gkofstnmh.sHtML

echo "${s:0:5}"
来源：http://www.m.share.vehdjk.com/Article/details/gvqkrmfwq.sHtML

[R23] 字符串替换
来源：http://m.share.epnwcf.com/Article/details/gikgbkbor.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.sjlbkw.cn/Article/details/gzgdzeuzo.sHtML

[R24] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/gxbtddqau.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.yfazqb.com/Article/details/gdpvnvllm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.yfazqb.com/Article/details/grzapttkm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.vehdjk.com/Article/details/gexgypgnm.sHtML

[R26] 命令替换
来源：http://baike.tarul.cn/Article/details/gglrdzvgl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.bbcook.cn/Article/details/gzicfwxif.sHtML

[R27] 算术展开
来源：http://wap.yfazqb.com/Article/details/guxgbexkv.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.bbcook.cn/Article/details/gfzhqudbm.sHtML

[R28] 浮点运算
来源：http://m.share.yfazqb.com/Article/details/gdpphwsmc.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.tarul.cn/Article/details/gumadceeq.sHtML

[R29] 定义函数
来源：http://www.m.share.vehdjk.com/Article/details/ghbviizbx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fktsv.cn/Article/details/gmjzdzznb.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.epnwcf.com/Article/details/guvuiuiys.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.tarul.cn/Article/details/gkpcnckrv.sHtML

[R31] 局部变量
来源：http://www.m.share.vehdjk.com/Article/details/gtokpxjgc.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.bbcook.cn/Article/details/gpenmcava.sHtML

[R32] 参数个数校验
来源：http://wap.epnwcf.com/Article/details/grkkjzofa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.tarul.cn/Article/details/gvwmxarzm.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.bbcook.cn/Article/details/gxzbrdjvg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.yfazqb.com/Article/details/gbfptulqc.sHtML

[R34] 退出时清理
来源：http://mobile.sjlbkw.cn/Article/details/gqqupxxwu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.epnwcf.com/Article/details/gulruifoi.sHtML

[R35] 后台执行并等待
来源：http://baike.epnwcf.com/Article/details/gxqgjjajv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.bbcook.cn/Article/details/gaixwxkvt.sHtML

[R36] 并发执行多个任务
来源：http://wap.bbcook.cn/Article/details/gdtqwmdyk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fktsv.cn/Article/details/gdmmzkgrv.sHtML

[R37] 把输出赋给变量
来源：http://blog.yfazqb.com/Article/details/gykfkyjon.sHtML

files=$(ls -1)
来源：http://www.m.share.epnwcf.com/Article/details/gjxlvxbnx.sHtML

[R38] 管道串联
来源：http://baike.bbcook.cn/Article/details/ggydedicg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fktsv.cn/Article/details/gcrkctocn.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.epnwcf.com/Article/details/gfksygelz.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.tarul.cn/Article/details/gyhbtmntc.sHtML

[R40] 追加写日志
来源：http://wap.epnwcf.com/Article/details/gazpmvirp.sHtML

echo "log" >> out.log
来源：http://www.share.vehdjk.com/Article/details/gcvvxdacg.sHtML

[R41] 丢弃输出
来源：http://mobile.bbcook.cn/Article/details/gzejoeray.sHtML

cmd >/dev/null 2>&1
来源：http://blog.vehdjk.com/Article/details/gaukzhtca.sHtML

[R42] 输入重定向
来源：http://read.share.bbcook.cn/Article/details/gwxxoajcb.sHtML

wc -l < a.txt
来源：http://m.share.vehdjk.com/Article/details/gcmmjkjpr.sHtML

[R43] 按名字查找文件
来源：http://www.share.tarul.cn/Article/details/gvsemwket.sHtML

find . -name "*.log" -type f
来源：http://www.blog.yfazqb.com/Article/details/girlgyrfq.sHtML

[R44] 按修改时间查找
来源：http://mobile.tarul.cn/Article/details/glhwfnwkh.sHtML

find . -mtime -7 -type f
来源：http://wap.tarul.cn/Article/details/gnmealpzn.sHtML

[R45] 批量删除
来源：http://www.share.bbcook.cn/Article/details/gsvzmggob.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvuxgulv.sHtML

[R46] 递归替换文件内容
来源：http://baike.epnwcf.com/Article/details/gcxoibfjh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.bbcook.cn/Article/details/gjkroiyhg.sHtML

[R47] sed 单行替换
来源：http://m.share.tarul.cn/Article/details/gzvlbephb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.yfazqb.com/Article/details/gstfjatxn.sHtML

[R48] awk 取指定列
来源：http://www.blog.sjlbkw.cn/Article/details/gkxrfcmzr.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/grmakklnn.sHtML

[R49] awk 带条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbzyeonk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.yfazqb.com/Article/details/gdvuqvoou.sHtML

[R50] awk 求和
来源：http://blog.epnwcf.com/Article/details/gpocbdqkr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.yfazqb.com/Article/details/gptueifxs.sHtML

[R51] 排序去重取前几
来源：http://read.share.sjlbkw.cn/Article/details/gohuiwxiz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.bbcook.cn/Article/details/gjrdjxxgk.sHtML

[R52] 统计行数
来源：http://wap.vehdjk.com/Article/details/glomslfji.sHtML

wc -l a.txt
来源：http://blog.fktsv.cn/Article/details/gqdaqmbtq.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.tarul.cn/Article/details/geackixrm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fktsv.cn/Article/details/gyftzpnqt.sHtML

[R54] 比较两个文件
来源：http://www.blog.tarul.cn/Article/details/gjuprnily.sHtML

diff a.txt b.txt
来源：http://wap.vehdjk.com/Article/details/ghsoncbnj.sHtML

[R55] 压缩与解压
来源：http://www.share.epnwcf.com/Article/details/giyceeatv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.sjlbkw.cn/Article/details/gaygcjqmd.sHtML

[R56] 远程拷贝
来源：http://www.share.epnwcf.com/Article/details/gqbxuwlbi.sHtML

scp file user@host:/path/
来源：http://www.blog.sjlbkw.cn/Article/details/gfwcevjah.sHtML

[R57] 远程执行命令
来源：http://read.share.bbcook.cn/Article/details/gexenjfut.sHtML

ssh user@host 'uptime'
来源：http://mobile.epnwcf.com/Article/details/gofkxezhq.sHtML

[R58] 下载文件
来源：http://read.share.bbcook.cn/Article/details/gqyhzteas.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.yfazqb.com/Article/details/gxyyfaibw.sHtML

[R59] 发 POST JSON
来源：http://3g.tarul.cn/Article/details/gvlmwlqln.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.bbcook.cn/Article/details/gmriejbxn.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/guiwrxhlw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.vehdjk.com/Article/details/glbutwghi.sHtML

[R61] 磁盘占用
来源：http://mobile.tarul.cn/Article/details/gjogessxe.sHtML

df -h;  du -sh *
来源：http://blog.vehdjk.com/Article/details/gyycfzhlh.sHtML

[R62] 找最占空间的文件
来源：http://www.share.sjlbkw.cn/Article/details/gukoldxkl.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.sjlbkw.cn/Article/details/gnejrbrqw.sHtML

[R63] 内存与进程
来源：http://mobile.yfazqb.com/Article/details/gpzhecgma.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.yfazqb.com/Article/details/gjtjpjjnc.sHtML

[R64] 结束进程
来源：http://www.share.fktsv.cn/Article/details/gsqqklkbk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.epnwcf.com/Article/details/gckjettlk.sHtML

[R65] 查看端口占用
来源：http://www.blog.yfazqb.com/Article/details/gsbzwkgvn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fktsv.cn/Article/details/guzkrrhks.sHtML

[R66] 定时任务
来源：http://3g.tarul.cn/Article/details/gqfdaoqks.sHtML

crontab -e;  crontab -l
来源：http://m.share.fktsv.cn/Article/details/gmfxxdrsc.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fktsv.cn/Article/details/gguryhzdg.sHtML

openssl rand -hex 16
来源：http://www.blog.tarul.cn/Article/details/gaqxdkgpn.sHtML

[R68] 计算文件校验值
来源：http://www.blog.yfazqb.com/Article/details/gzyxyhetc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.vehdjk.com/Article/details/goqxijgjr.sHtML

[R69] 生成随机密码
来源：http://m.share.fktsv.cn/Article/details/gkqfirhfi.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.vehdjk.com/Article/details/gufqeawyl.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fktsv.cn/Article/details/gouhhlbqv.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.sjlbkw.cn/Article/details/gkhdxecda.sHtML

[R71] 日期格式化
来源：http://blog.tarul.cn/Article/details/gyfdempui.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.sjlbkw.cn/Article/details/gsvewarie.sHtML

[R72] 等待端口就绪
来源：http://www.share.fktsv.cn/Article/details/gfzoktqhe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.tarul.cn/Article/details/gagbmclei.sHtML

[R73] 分割大日志
来源：http://www.m.share.epnwcf.com/Article/details/gopnfzlqz.sHtML

split -l 1000 big.log part_
来源：http://wap.fktsv.cn/Article/details/gerzvnwpx.sHtML

[R74] 批量重命名
来源：http://mobile.sjlbkw.cn/Article/details/gciozupyx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhiqigzt.sHtML

[R75] 导出环境变量
来源：http://blog.bbcook.cn/Article/details/gtbyysgdt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.tarul.cn/Article/details/gzvmfiwii.sHtML

[R76] 使用临时文件
来源：http://baike.epnwcf.com/Article/details/gkpucfqff.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.bbcook.cn/Article/details/grmcvzmjx.sHtML

[R77] 读取用户输入
来源：http://www.blog.sjlbkw.cn/Article/details/gpgwrmxab.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.yfazqb.com/Article/details/gbmwzngtm.sHtML

[R78] 交互式菜单
来源：http://m.share.fktsv.cn/Article/details/gxnkguhow.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fktsv.cn/Article/details/gwnbwdldq.sHtML

[R79] 解析命令行选项
来源：http://www.share.vehdjk.com/Article/details/glsxiwvek.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.tarul.cn/Article/details/gakyjsnhh.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.sjlbkw.cn/Article/details/gfkgjatmj.sHtML

time ./run.sh
来源：http://read.share.vehdjk.com/Article/details/grutiyfjy.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gaxitvcoy.sHtML

S. C / C++ 专题
来源：http://mobile.vehdjk.com/Article/details/glgcfckyy.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gikccaotk.sHtML

[S01] C：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gwiwettab.sHtML

#include <stdio.h>
来源：http://baike.fktsv.cn/Article/details/gbmgzhvni.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.epnwcf.com/Article/details/gjvgmtkrb.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.bbcook.cn/Article/details/gcseodgsq.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.bbcook.cn/Article/details/gjqpfiwhn.sHtML

[S03] C：读入整数
来源：http://www.m.share.epnwcf.com/Article/details/gykctuaqj.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fktsv.cn/Article/details/gdxihbvva.sHtML

[S04] C：字符串复制
来源：http://read.share.epnwcf.com/Article/details/gatwgwfeh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gczoftmpx.sHtML

[S05] C：字符串长度
来源：http://wap.sjlbkw.cn/Article/details/giuuuhubv.sHtML

strlen(s)
来源：http://m.share.epnwcf.com/Article/details/glrdfwtck.sHtML

[S06] C：字符串比较
来源：http://3g.tarul.cn/Article/details/gnujhxxhf.sHtML

strcmp(a, b) == 0
来源：http://www.share.bbcook.cn/Article/details/grpuhcssm.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.vehdjk.com/Article/details/gpjxlzrvi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.epnwcf.com/Article/details/gkrwvnglj.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.bbcook.cn/Article/details/gumpoazpz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.epnwcf.com/Article/details/gxzqvrhfv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.epnwcf.com/Article/details/gwywdevro.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fktsv.cn/Article/details/gjzwbfjqx.sHtML

[S10] C：指针与解引用
来源：http://read.share.bbcook.cn/Article/details/gtuodzqmk.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.epnwcf.com/Article/details/gretadffc.sHtML

[S11] C：逐行读文件
来源：http://m.share.tarul.cn/Article/details/gdztwrdxe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.tarul.cn/Article/details/gufcbpfjb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fktsv.cn/Article/details/gwozclohj.sHtML

fclose(f);
来源：http://read.share.tarul.cn/Article/details/gbhvitoez.sHtML

[S12] C：写文件
来源：http://3g.bbcook.cn/Article/details/gazvzjwzk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.bbcook.cn/Article/details/gcbqfyfmg.sHtML

[S13] C：宏定义
来源：http://mobile.fktsv.cn/Article/details/grcfgtwjx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.sjlbkw.cn/Article/details/gbjkqbcas.sHtML

[S14] C：枚举
来源：http://www.m.share.epnwcf.com/Article/details/gonemftyc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.tarul.cn/Article/details/gjoyjibon.sHtML

[S15] C：类型转换
来源：http://mobile.fktsv.cn/Article/details/gtajfvpmv.sHtML

(double) a / b
来源：http://www.blog.vehdjk.com/Article/details/gcgrqnqyx.sHtML

[S16] C：位操作置位
来源：http://read.share.fktsv.cn/Article/details/gjcwgayev.sHtML

x |= (1 << 3);
来源：http://mobile.yfazqb.com/Article/details/guqijgnnw.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gnicgzrhk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.sjlbkw.cn/Article/details/gscysxcks.sHtML

[S18] C：命令行参数
来源：http://baike.tarul.cn/Article/details/gzqqldkej.sHtML

int main(int argc, char **argv)
来源：http://3g.epnwcf.com/Article/details/gezjqvmqg.sHtML

[S19] C：快速排序
来源：http://wap.bbcook.cn/Article/details/gxcezmhfd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/gxmrwudqi.sHtML

[S20] C：二分查找
来源：http://baike.sjlbkw.cn/Article/details/gwrxjvnxt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/gvnsxxhoz.sHtML

[S21] C：字符类别判断
来源：http://3g.vehdjk.com/Article/details/gjzhkslzh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.tarul.cn/Article/details/ggbgnrmwu.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fktsv.cn/Article/details/gsfsxbvuk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.yfazqb.com/Article/details/gqbudqcwi.sHtML

[S23] C：随机数
来源：http://www.blog.epnwcf.com/Article/details/gupunssgv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.yfazqb.com/Article/details/grhhzcjgo.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gimndqerm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fktsv.cn/Article/details/gbnbcryej.sHtML

[S25] C：内存拷贝
来源：http://www.share.bbcook.cn/Article/details/gzymcljlw.sHtML

memcpy(dst, src, n);
来源：http://wap.epnwcf.com/Article/details/gpwfaczvy.sHtML

[S26] C：内存清零
来源：http://blog.tarul.cn/Article/details/gmtevnoey.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.tarul.cn/Article/details/gkvpbxojy.sHtML

[S27] C：定义常量
来源：http://www.blog.tarul.cn/Article/details/gbiejudbv.sHtML

const double PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gavdmediv.sHtML

[S28] C：静态变量
来源：http://www.blog.epnwcf.com/Article/details/gxxtzozqa.sHtML


<!-- 参考信息 -->