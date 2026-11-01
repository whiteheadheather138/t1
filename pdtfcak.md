代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.bbcook.cn/Article/details/gbctrpaux.sHtML

[Q52] 删除指定行
来源：http://m.share.vehdjk.com/Article/details/gewqlsevc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gbwepveue.sHtML

[Q53] 按条件删除
来源：http://blog.tarul.cn/Article/details/ginvlteep.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/gltwaxfxb.sHtML

[Q54] 清空表
来源：http://www.blog.bbcook.cn/Article/details/gnzfvaqwn.sHtML

TRUNCATE TABLE logs;
来源：http://blog.bbcook.cn/Article/details/gcvqubxal.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.yfazqb.com/Article/details/gdhdcwkwy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.tarul.cn/Article/details/gbcbkhhhk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.vehdjk.com/Article/details/gfkdoxsqy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.vehdjk.com/Article/details/goswqnefr.sHtML

[Q57] 行号
来源：http://baike.tarul.cn/Article/details/gwadanrrq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.yfazqb.com/Article/details/gmvkptglu.sHtML

[Q58] 累计求和
来源：http://baike.fktsv.cn/Article/details/gbghtfths.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fktsv.cn/Article/details/goxijnjms.sHtML

[Q59] 分组内累计
来源：http://mobile.vehdjk.com/Article/details/ggarhvcue.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gawmxanpu.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.sjlbkw.cn/Article/details/ghmpomfwz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.epnwcf.com/Article/details/gaxymfndp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.epnwcf.com/Article/details/gvuloxklx.sHtML

[Q61] 移动平均
来源：http://mobile.sjlbkw.cn/Article/details/gdxdewojr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.tarul.cn/Article/details/grxcvswoy.sHtML

[Q62] 分组占比
来源：http://blog.yfazqb.com/Article/details/gifsevqwl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/gpdqjizim.sHtML

[Q63] 开启事务
来源：http://wap.yfazqb.com/Article/details/gaoiipcrd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.sjlbkw.cn/Article/details/gwxubinco.sHtML

[Q64] 提交事务
来源：http://wap.sjlbkw.cn/Article/details/ggtquvjzx.sHtML

COMMIT;
来源：http://baike.tarul.cn/Article/details/ggvvzppbc.sHtML

[Q65] 回滚事务
来源：http://mobile.epnwcf.com/Article/details/ghghxwjid.sHtML

ROLLBACK;
来源：http://3g.fktsv.cn/Article/details/gkjxrweym.sHtML

[Q66] 行锁查询
来源：http://baike.vehdjk.com/Article/details/gxdtbmnns.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.epnwcf.com/Article/details/gfuvkxhok.sHtML

[Q67] 设置隔离级别
来源：http://mobile.bbcook.cn/Article/details/gcwibdsts.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.epnwcf.com/Article/details/goebwgymo.sHtML

[Q68] 保存点
来源：http://www.m.share.fktsv.cn/Article/details/goamigcil.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fktsv.cn/Article/details/gkygalhjn.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.bbcook.cn/Article/details/gkwvvbtch.sHtML

[Q69] 查看执行计划
来源：http://3g.sjlbkw.cn/Article/details/gcwohyuak.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.epnwcf.com/Article/details/gqhbgiyko.sHtML

[Q70] 更新统计信息
来源：http://www.share.vehdjk.com/Article/details/ggoviukth.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.vehdjk.com/Article/details/guesuwhvc.sHtML

[Q71] 查看建表语句
来源：http://wap.bbcook.cn/Article/details/gqmhvzdaj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.epnwcf.com/Article/details/gnohxohtu.sHtML

[Q72] 查看索引
来源：http://read.share.epnwcf.com/Article/details/gpdxzgasv.sHtML

SHOW INDEX FROM users;
来源：http://baike.tarul.cn/Article/details/gqcnxgwjl.sHtML

[Q73] 查看表状态
来源：http://m.share.epnwcf.com/Article/details/gjzprtidi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fktsv.cn/Article/details/gilggjggk.sHtML

[Q74] 强制使用索引
来源：http://wap.bbcook.cn/Article/details/gjspadsib.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.tarul.cn/Article/details/gmivxmlsf.sHtML

[Q75] 日期格式化
来源：http://read.share.bbcook.cn/Article/details/gcfofvzul.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.epnwcf.com/Article/details/gzbfhozru.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fktsv.cn/Article/details/gvecxgwdd.sHtML

[Q76] 按天统计
来源：http://m.share.sjlbkw.cn/Article/details/gwunfkuot.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.sjlbkw.cn/Article/details/gqcvphpxn.sHtML

[Q77] 时间加减
来源：http://3g.yfazqb.com/Article/details/giiguwsjs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.bbcook.cn/Article/details/gyjphsteb.sHtML

[Q78] 当前时间
来源：http://wap.vehdjk.com/Article/details/gndmrjxky.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.yfazqb.com/Article/details/gjjqztmer.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.bbcook.cn/Article/details/gjvuiiqwd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.vehdjk.com/Article/details/gqucgnhfb.sHtML

[Q80] 字符串截取
来源：http://wap.vehdjk.com/Article/details/gzfeyrzjh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.bbcook.cn/Article/details/gfvplnzgn.sHtML

[Q81] 字符串替换
来源：http://blog.bbcook.cn/Article/details/gjgkwricw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.epnwcf.com/Article/details/gdbfjrmxy.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.tarul.cn/Article/details/gwyjhabpm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/glzigcedq.sHtML

[Q83] 大小写转换
来源：http://www.blog.bbcook.cn/Article/details/gmxfzjxjs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnkoaels.sHtML

[Q84] 去除首尾空格
来源：http://baike.sjlbkw.cn/Article/details/gdqjefpfw.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/goiudzrpx.sHtML

[Q85] 数值取整
来源：http://mobile.fktsv.cn/Article/details/gtdmroioc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.epnwcf.com/Article/details/gdjmpzquv.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.bbcook.cn/Article/details/gmvmbjuvh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.epnwcf.com/Article/details/gqssshufo.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.vehdjk.com/Article/details/gbszuutur.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.yfazqb.com/Article/details/grgtcuxnt.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.epnwcf.com/Article/details/gumarxyen.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.sjlbkw.cn/Article/details/gthvujwfg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.bbcook.cn/Article/details/gjcqnlvzg.sHtML

[Q89] 判断表是否存在
来源：http://wap.epnwcf.com/Article/details/gpqufskup.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.yfazqb.com/Article/details/ghopgkygd.sHtML

[Q90] 生成序号列
来源：http://m.share.vehdjk.com/Article/details/girpxfspz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.yfazqb.com/Article/details/gsydurynm.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gyozqkafv.sHtML

R. Bash 专题
来源：http://www.m.share.tarul.cn/Article/details/gdrbrqokm.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gvptenxaj.sHtML

[R01] shebang 与严格模式
来源：http://baike.sjlbkw.cn/Article/details/ggluegzpp.sHtML

#!/usr/bin/env bash
来源：http://baike.yfazqb.com/Article/details/gfvqsinwa.sHtML

set -euo pipefail
来源：http://read.share.tarul.cn/Article/details/gizqfkdba.sHtML

[R02] 变量赋值与使用
来源：http://mobile.epnwcf.com/Article/details/gvfmgrfkh.sHtML

name="Tom"; echo "$name"
来源：http://m.share.yfazqb.com/Article/details/gpmmajpwy.sHtML

[R03] 只读变量
来源：http://blog.yfazqb.com/Article/details/gedmpxgdq.sHtML

readonly PI=3.14
来源：http://blog.sjlbkw.cn/Article/details/gatovqvtp.sHtML

[R04] 位置参数
来源：http://www.m.share.bbcook.cn/Article/details/gzxhrglsf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.yfazqb.com/Article/details/gaiszdyfj.sHtML

[R05] 参数默认值
来源：http://www.m.share.yfazqb.com/Article/details/gszahkcai.sHtML

name="${1:-default}"
来源：http://mobile.vehdjk.com/Article/details/ggbdpbmgs.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gzatsjzmv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.yfazqb.com/Article/details/gcwjadmxu.sHtML

[R07] if 判断文件
来源：http://mobile.fktsv.cn/Article/details/gmeloawtc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gggxbxzzm.sHtML

[R08] 数值比较
来源：http://3g.vehdjk.com/Article/details/goyayikzl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.bbcook.cn/Article/details/gykergoki.sHtML

[R09] 字符串比较
来源：http://3g.epnwcf.com/Article/details/gvlyvetnv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.yfazqb.com/Article/details/gyuwkparv.sHtML

[R10] 正则匹配
来源：http://read.share.sjlbkw.cn/Article/details/gtgyqsqbv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fktsv.cn/Article/details/gryljubzm.sHtML

[R11] case 多分支
来源：http://www.m.share.epnwcf.com/Article/details/giuppnjco.sHtML

case "$1" in
来源：http://mobile.tarul.cn/Article/details/gypdubnyg.sHtML

start) echo "启动" ;;
来源：http://www.blog.yfazqb.com/Article/details/ggdbpojbu.sHtML

stop)  echo "停止" ;;
来源：http://baike.bbcook.cn/Article/details/gggxattkl.sHtML

*)     echo "未知命令" ;;
来源：http://baike.tarul.cn/Article/details/glmvxxnqd.sHtML

esac
来源：http://m.share.fktsv.cn/Article/details/ggwhrytnk.sHtML

[R12] for 遍历文件
来源：http://m.share.yfazqb.com/Article/details/gzgklhzaw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.bbcook.cn/Article/details/ggmrcgwjz.sHtML

[R13] for 计数循环
来源：http://mobile.bbcook.cn/Article/details/gtrzrhjrw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.yfazqb.com/Article/details/gposofgps.sHtML

[R14] C 风格 for
来源：http://www.blog.sjlbkw.cn/Article/details/gvlihsvle.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fktsv.cn/Article/details/gaglmeqcd.sHtML

[R15] while 逐行读文件
来源：http://baike.tarul.cn/Article/details/grbyjysym.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.tarul.cn/Article/details/ghsetfarn.sHtML

[R16] until 等待条件
来源：http://3g.vehdjk.com/Article/details/ggpultbam.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.yfazqb.com/Article/details/gsfmytvtm.sHtML

[R17] 数组定义与取值
来源：http://www.share.tarul.cn/Article/details/gndtixoxj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.bbcook.cn/Article/details/gpatrceyi.sHtML

[R18] 遍历数组
来源：http://wap.sjlbkw.cn/Article/details/gbqhhsepw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.sjlbkw.cn/Article/details/gottjmbvb.sHtML

[R19] 数组长度
来源：http://wap.yfazqb.com/Article/details/gjaryiver.sHtML

echo "${#arr[@]}"
来源：http://blog.sjlbkw.cn/Article/details/gbuvucblr.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.epnwcf.com/Article/details/gbiqdtyxy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.yfazqb.com/Article/details/gmbomfgpl.sHtML

[R21] 字符串长度
来源：http://baike.sjlbkw.cn/Article/details/gxrwzirjx.sHtML

echo "${#s}"
来源：http://m.share.vehdjk.com/Article/details/gqfbqthro.sHtML

[R22] 截取子串
来源：http://blog.tarul.cn/Article/details/gzatthbap.sHtML

echo "${s:0:5}"
来源：http://read.share.sjlbkw.cn/Article/details/gxdworkpk.sHtML

[R23] 字符串替换
来源：http://m.share.fktsv.cn/Article/details/gbjrywvvw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.vehdjk.com/Article/details/ggqsxlgqa.sHtML

[R24] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gncawttpu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.vehdjk.com/Article/details/gimmqdcuc.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.sjlbkw.cn/Article/details/gyyfwqbzb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.tarul.cn/Article/details/gbefbaecn.sHtML

[R26] 命令替换
来源：http://www.blog.sjlbkw.cn/Article/details/gkyhmctcx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fktsv.cn/Article/details/gkoqqedhp.sHtML

[R27] 算术展开
来源：http://www.blog.epnwcf.com/Article/details/gclkpohtc.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.tarul.cn/Article/details/gypyfwspx.sHtML

[R28] 浮点运算
来源：http://www.share.vehdjk.com/Article/details/gnywjlsct.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.yfazqb.com/Article/details/ghwlwgvkc.sHtML

[R29] 定义函数
来源：http://mobile.epnwcf.com/Article/details/giksipunf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.bbcook.cn/Article/details/gkkvbvqiy.sHtML

[R30] 函数返回状态码
来源：http://baike.epnwcf.com/Article/details/gxvgwvvwo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.bbcook.cn/Article/details/gocqgkvvb.sHtML

[R31] 局部变量
来源：http://www.share.epnwcf.com/Article/details/gxukutmob.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gesbnlfch.sHtML

[R32] 参数个数校验
来源：http://wap.fktsv.cn/Article/details/gyfjroafu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.tarul.cn/Article/details/gfbbmccqn.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fktsv.cn/Article/details/gqajtgeiq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.sjlbkw.cn/Article/details/ghboomtqm.sHtML

[R34] 退出时清理
来源：http://3g.epnwcf.com/Article/details/ghimplqun.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.vehdjk.com/Article/details/gosgulvmv.sHtML

[R35] 后台执行并等待
来源：http://blog.bbcook.cn/Article/details/giglyavfm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.epnwcf.com/Article/details/gqmsuubpx.sHtML

[R36] 并发执行多个任务
来源：http://m.share.tarul.cn/Article/details/gmhuysbsq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fktsv.cn/Article/details/gmtvgztrk.sHtML

[R37] 把输出赋给变量
来源：http://www.share.bbcook.cn/Article/details/gvuxkgpwk.sHtML

files=$(ls -1)
来源：http://www.blog.fktsv.cn/Article/details/gbnurshae.sHtML

[R38] 管道串联
来源：http://www.share.tarul.cn/Article/details/gxfqvtqnz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.sjlbkw.cn/Article/details/gxwkfcgjo.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.vehdjk.com/Article/details/gjewxwgbp.sHtML

cmd > out.log 2>&1
来源：http://m.share.fktsv.cn/Article/details/gqzflzrte.sHtML

[R40] 追加写日志
来源：http://www.m.share.fktsv.cn/Article/details/ghmntegxj.sHtML

echo "log" >> out.log
来源：http://baike.bbcook.cn/Article/details/gosnguabb.sHtML

[R41] 丢弃输出
来源：http://mobile.bbcook.cn/Article/details/gjorbsqcf.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fktsv.cn/Article/details/gdfizhivr.sHtML

[R42] 输入重定向
来源：http://baike.yfazqb.com/Article/details/gtoawldvp.sHtML

wc -l < a.txt
来源：http://read.share.fktsv.cn/Article/details/gcbxulpqd.sHtML

[R43] 按名字查找文件
来源：http://mobile.fktsv.cn/Article/details/ghraxwqug.sHtML

find . -name "*.log" -type f
来源：http://mobile.bbcook.cn/Article/details/gnbnzkbjj.sHtML

[R44] 按修改时间查找
来源：http://mobile.bbcook.cn/Article/details/ghsjjkjqg.sHtML

find . -mtime -7 -type f
来源：http://3g.bbcook.cn/Article/details/gqzsszlgr.sHtML

[R45] 批量删除
来源：http://www.share.yfazqb.com/Article/details/gllcvfbcf.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.bbcook.cn/Article/details/gwgpxdnru.sHtML

[R46] 递归替换文件内容
来源：http://3g.epnwcf.com/Article/details/grourvodh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.vehdjk.com/Article/details/ghvpetged.sHtML

[R47] sed 单行替换
来源：http://read.share.fktsv.cn/Article/details/gxysnfhtt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.yfazqb.com/Article/details/gymolfjel.sHtML

[R48] awk 取指定列
来源：http://m.share.vehdjk.com/Article/details/gerlvhfdl.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.yfazqb.com/Article/details/gwvpxrkha.sHtML

[R49] awk 带条件
来源：http://baike.bbcook.cn/Article/details/gequeszqo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.epnwcf.com/Article/details/grwqrihxm.sHtML

[R50] awk 求和
来源：http://blog.vehdjk.com/Article/details/gwecebryc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.yfazqb.com/Article/details/gochnngdd.sHtML

[R51] 排序去重取前几
来源：http://mobile.yfazqb.com/Article/details/gcictdxvt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.sjlbkw.cn/Article/details/gdzaybciu.sHtML

[R52] 统计行数
来源：http://blog.vehdjk.com/Article/details/gtxxktrya.sHtML

wc -l a.txt
来源：http://read.share.epnwcf.com/Article/details/guhfcsdhy.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.bbcook.cn/Article/details/gokpjoeup.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.sjlbkw.cn/Article/details/gapukfamd.sHtML

[R54] 比较两个文件
来源：http://m.share.fktsv.cn/Article/details/gvtrezbkl.sHtML

diff a.txt b.txt
来源：http://3g.tarul.cn/Article/details/gdycxopbb.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fktsv.cn/Article/details/gzxdkviye.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fktsv.cn/Article/details/gyhgxvfaq.sHtML

[R56] 远程拷贝
来源：http://3g.sjlbkw.cn/Article/details/guryghrjy.sHtML

scp file user@host:/path/
来源：http://baike.tarul.cn/Article/details/gcmybiqnj.sHtML

[R57] 远程执行命令
来源：http://www.share.vehdjk.com/Article/details/gtotosbot.sHtML

ssh user@host 'uptime'
来源：http://baike.bbcook.cn/Article/details/gcioujurh.sHtML

[R58] 下载文件
来源：http://www.m.share.fktsv.cn/Article/details/gldnxwypc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.yfazqb.com/Article/details/gjyoyablb.sHtML

[R59] 发 POST JSON
来源：http://wap.epnwcf.com/Article/details/gaqtylrnm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.tarul.cn/Article/details/gvpeutmtv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/gqiqdjtgt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.epnwcf.com/Article/details/gqyyjnvxo.sHtML

[R61] 磁盘占用
来源：http://3g.epnwcf.com/Article/details/gegwlwtdu.sHtML

df -h;  du -sh *
来源：http://blog.epnwcf.com/Article/details/geqrobnay.sHtML

[R62] 找最占空间的文件
来源：http://3g.tarul.cn/Article/details/gvzbpogwa.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.sjlbkw.cn/Article/details/gkkullcxb.sHtML

[R63] 内存与进程
来源：http://mobile.vehdjk.com/Article/details/gukfvvfdw.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.epnwcf.com/Article/details/gukiqstjf.sHtML

[R64] 结束进程
来源：http://3g.fktsv.cn/Article/details/gkbanhajt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fktsv.cn/Article/details/gdgznykof.sHtML

[R65] 查看端口占用
来源：http://www.blog.epnwcf.com/Article/details/ghnnruwpb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.yfazqb.com/Article/details/gzurnstal.sHtML

[R66] 定时任务
来源：http://read.share.epnwcf.com/Article/details/gzpxhphqc.sHtML

crontab -e;  crontab -l
来源：http://mobile.bbcook.cn/Article/details/gulxetdtw.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.yfazqb.com/Article/details/gelnktxgh.sHtML

openssl rand -hex 16
来源：http://baike.sjlbkw.cn/Article/details/gwdrceohp.sHtML

[R68] 计算文件校验值
来源：http://3g.bbcook.cn/Article/details/glaemllqy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fktsv.cn/Article/details/gljdiopne.sHtML

[R69] 生成随机密码
来源：http://mobile.fktsv.cn/Article/details/ghklsabjy.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.tarul.cn/Article/details/gsnexxrod.sHtML

[R70] 时间戳与互转
来源：http://mobile.sjlbkw.cn/Article/details/ghtvxxfui.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.yfazqb.com/Article/details/gozrqjeyi.sHtML

[R71] 日期格式化
来源：http://read.share.fktsv.cn/Article/details/gffcexkyw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.epnwcf.com/Article/details/gdwoeopvu.sHtML

[R72] 等待端口就绪
来源：http://mobile.sjlbkw.cn/Article/details/gdlkolktl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.yfazqb.com/Article/details/gbiisdlzm.sHtML

[R73] 分割大日志
来源：http://baike.sjlbkw.cn/Article/details/gxkhohhtl.sHtML

split -l 1000 big.log part_
来源：http://m.share.epnwcf.com/Article/details/gsohwjizv.sHtML

[R74] 批量重命名
来源：http://www.share.bbcook.cn/Article/details/gmrpyubcn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.bbcook.cn/Article/details/gadzfjnvn.sHtML

[R75] 导出环境变量
来源：http://3g.tarul.cn/Article/details/gvloykmbp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.epnwcf.com/Article/details/ggfswicei.sHtML

[R76] 使用临时文件
来源：http://mobile.tarul.cn/Article/details/gleqickli.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fktsv.cn/Article/details/gtqirwmfl.sHtML

[R77] 读取用户输入
来源：http://wap.vehdjk.com/Article/details/ghutinmsw.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.tarul.cn/Article/details/gmlvrkjge.sHtML

[R78] 交互式菜单
来源：http://www.blog.bbcook.cn/Article/details/gyadzgjau.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.epnwcf.com/Article/details/gieryzqxn.sHtML

[R79] 解析命令行选项
来源：http://blog.epnwcf.com/Article/details/gnorvdnru.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.yfazqb.com/Article/details/gqecvmapd.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.vehdjk.com/Article/details/gqsxryfgf.sHtML

time ./run.sh
来源：http://baike.sjlbkw.cn/Article/details/glkszctpp.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gcchnlxzt.sHtML

S. C / C++ 专题
来源：http://3g.epnwcf.com/Article/details/gybjpdsps.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gippqlxqs.sHtML

[S01] C：Hello World
来源：http://m.share.fktsv.cn/Article/details/gqrwhxqse.sHtML

#include <stdio.h>
来源：http://baike.vehdjk.com/Article/details/gwbeblwca.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.tarul.cn/Article/details/givxxwfzi.sHtML

[S02] C：变量与格式化输出
来源：http://3g.sjlbkw.cn/Article/details/gwtkobasd.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.vehdjk.com/Article/details/gbpbdbjbg.sHtML

[S03] C：读入整数
来源：http://baike.sjlbkw.cn/Article/details/gblmubbmk.sHtML

int x; scanf("%d", &x);
来源：http://baike.epnwcf.com/Article/details/grqddjjmn.sHtML

[S04] C：字符串复制
来源：http://baike.tarul.cn/Article/details/gviaslgwg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.tarul.cn/Article/details/gtfzkxoan.sHtML

[S05] C：字符串长度
来源：http://www.blog.vehdjk.com/Article/details/gvnqzavoe.sHtML

strlen(s)
来源：http://www.m.share.bbcook.cn/Article/details/ggoufpgvi.sHtML

[S06] C：字符串比较
来源：http://wap.fktsv.cn/Article/details/gvsmfqxko.sHtML

strcmp(a, b) == 0
来源：http://mobile.yfazqb.com/Article/details/gtktnmscq.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.yfazqb.com/Article/details/gxevkfajk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.tarul.cn/Article/details/gladzcwms.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.epnwcf.com/Article/details/geypukdax.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.tarul.cn/Article/details/gwsnypzgg.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.sjlbkw.cn/Article/details/gnlrhdfmz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.yfazqb.com/Article/details/gaddyyqzy.sHtML

[S10] C：指针与解引用
来源：http://read.share.vehdjk.com/Article/details/godqtmzim.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.vehdjk.com/Article/details/gjemdbhtd.sHtML

[S11] C：逐行读文件
来源：http://read.share.tarul.cn/Article/details/gjahydmts.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.bbcook.cn/Article/details/ggbpccqjf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.tarul.cn/Article/details/gpenrficq.sHtML

fclose(f);
来源：http://m.share.bbcook.cn/Article/details/gttmavxik.sHtML

[S12] C：写文件
来源：http://m.share.sjlbkw.cn/Article/details/gkuublgyy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/gqwqwbqbf.sHtML

[S13] C：宏定义
来源：http://mobile.tarul.cn/Article/details/gugrcnxqy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.bbcook.cn/Article/details/gcluohmjx.sHtML

[S14] C：枚举
来源：http://baike.sjlbkw.cn/Article/details/gxvppdypq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.bbcook.cn/Article/details/giljbpqzf.sHtML

[S15] C：类型转换
来源：http://m.share.vehdjk.com/Article/details/gkipvbmhg.sHtML

(double) a / b
来源：http://www.share.sjlbkw.cn/Article/details/gosoytftm.sHtML

[S16] C：位操作置位
来源：http://3g.sjlbkw.cn/Article/details/gnvobjmdl.sHtML

x |= (1 << 3);
来源：http://www.blog.tarul.cn/Article/details/gtuwfhmbe.sHtML

[S17] C：安全拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/gjykbmwzd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.tarul.cn/Article/details/gncjyzvkc.sHtML

[S18] C：命令行参数
来源：http://m.share.epnwcf.com/Article/details/gtzxygluv.sHtML

int main(int argc, char **argv)
来源：http://www.share.vehdjk.com/Article/details/gsciigsbm.sHtML

[S19] C：快速排序
来源：http://blog.yfazqb.com/Article/details/gcbsozrqt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/gqhekwmit.sHtML

[S20] C：二分查找
来源：http://wap.tarul.cn/Article/details/gjxhhdxux.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.tarul.cn/Article/details/gopeglswp.sHtML

[S21] C：字符类别判断
来源：http://www.blog.epnwcf.com/Article/details/grlaongbl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.yfazqb.com/Article/details/gysswsbyo.sHtML

[S22] C：字符串转数字
来源：http://3g.tarul.cn/Article/details/gzzrjevnu.sHtML


<!-- 参考信息 -->