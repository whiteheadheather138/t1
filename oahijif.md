代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.tarul.cn/Article/details/gzmrgjmif.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.bbcook.cn/Article/details/gtroauobl.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.sjlbkw.cn/Article/details/ggyqvuxfv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.tarul.cn/Article/details/grgxiaugn.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlrbqucg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fktsv.cn/Article/details/gjearmgxf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fktsv.cn/Article/details/glczancui.sHtML

[Q49] 更新单行
来源：http://wap.epnwcf.com/Article/details/gtrxtybkx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/gmeuuassk.sHtML

[Q50] 批量更新
来源：http://www.m.share.yfazqb.com/Article/details/gkszuuvwf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.vehdjk.com/Article/details/ggukzxzsc.sHtML

[Q51] 用子查询更新
来源：http://read.share.epnwcf.com/Article/details/glypvctcp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gipaapfkc.sHtML

[Q52] 删除指定行
来源：http://blog.tarul.cn/Article/details/gdzzjfrtl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.tarul.cn/Article/details/gbvoxckit.sHtML

[Q53] 按条件删除
来源：http://mobile.vehdjk.com/Article/details/ggvzhanri.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.sjlbkw.cn/Article/details/gefqivyqu.sHtML

[Q54] 清空表
来源：http://www.share.tarul.cn/Article/details/gelnjboxu.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.tarul.cn/Article/details/gnybnfmbh.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.tarul.cn/Article/details/gkjhqaojr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.vehdjk.com/Article/details/galdokwmq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.epnwcf.com/Article/details/gzkdpfikx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.tarul.cn/Article/details/grouetiqa.sHtML

[Q57] 行号
来源：http://www.share.vehdjk.com/Article/details/glprlxmei.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.yfazqb.com/Article/details/gjrduzkwg.sHtML

[Q58] 累计求和
来源：http://read.share.tarul.cn/Article/details/gfplkdlbe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gsqwpghbr.sHtML

[Q59] 分组内累计
来源：http://www.share.tarul.cn/Article/details/gnkdtjzfc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gqhofbmuo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.yfazqb.com/Article/details/gunnrffke.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fktsv.cn/Article/details/gewkhyqqs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/goaukyfyg.sHtML

[Q61] 移动平均
来源：http://mobile.vehdjk.com/Article/details/gochztkeg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/goigntzlx.sHtML

[Q62] 分组占比
来源：http://wap.yfazqb.com/Article/details/grhhofmiz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gwyylvubh.sHtML

[Q63] 开启事务
来源：http://read.share.bbcook.cn/Article/details/gkvoythic.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.epnwcf.com/Article/details/gavzsgaoc.sHtML

[Q64] 提交事务
来源：http://mobile.yfazqb.com/Article/details/geextgylk.sHtML

COMMIT;
来源：http://read.share.vehdjk.com/Article/details/gacddwimi.sHtML

[Q65] 回滚事务
来源：http://blog.vehdjk.com/Article/details/goddujxgj.sHtML

ROLLBACK;
来源：http://mobile.tarul.cn/Article/details/gsaxumvcz.sHtML

[Q66] 行锁查询
来源：http://m.share.epnwcf.com/Article/details/gjyfjgplq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.yfazqb.com/Article/details/gaxslnbnj.sHtML

[Q67] 设置隔离级别
来源：http://m.share.yfazqb.com/Article/details/gbshuosku.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrikjetc.sHtML

[Q68] 保存点
来源：http://blog.tarul.cn/Article/details/gkgobjbwt.sHtML

SAVEPOINT sp1;
来源：http://read.share.sjlbkw.cn/Article/details/gvghqxcfi.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.bbcook.cn/Article/details/gymmllxox.sHtML

[Q69] 查看执行计划
来源：http://www.share.tarul.cn/Article/details/grytmgrxw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.epnwcf.com/Article/details/gqazqnxou.sHtML

[Q70] 更新统计信息
来源：http://3g.sjlbkw.cn/Article/details/gfhrxddjq.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fktsv.cn/Article/details/gtipuinrs.sHtML

[Q71] 查看建表语句
来源：http://3g.tarul.cn/Article/details/gymhkecbl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.bbcook.cn/Article/details/gflcgaakd.sHtML

[Q72] 查看索引
来源：http://www.blog.fktsv.cn/Article/details/gebmasvft.sHtML

SHOW INDEX FROM users;
来源：http://www.share.vehdjk.com/Article/details/guvmojykx.sHtML

[Q73] 查看表状态
来源：http://wap.yfazqb.com/Article/details/ghhbdklfi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.epnwcf.com/Article/details/gbybjkctx.sHtML

[Q74] 强制使用索引
来源：http://read.share.sjlbkw.cn/Article/details/gcqroflhv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fktsv.cn/Article/details/gryjiveps.sHtML

[Q75] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gkwknirbr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.vehdjk.com/Article/details/glfzcsonl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.vehdjk.com/Article/details/gpcrlvjwl.sHtML

[Q76] 按天统计
来源：http://mobile.sjlbkw.cn/Article/details/gpmfsgasu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.yfazqb.com/Article/details/gpewomqgi.sHtML

[Q77] 时间加减
来源：http://www.blog.tarul.cn/Article/details/gtgtbgkce.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.yfazqb.com/Article/details/gjwejmgtb.sHtML

[Q78] 当前时间
来源：http://read.share.sjlbkw.cn/Article/details/grqavzlcn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.epnwcf.com/Article/details/gssrjdyts.sHtML

[Q79] 字符串拼接
来源：http://www.share.epnwcf.com/Article/details/gcoiunvdt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.yfazqb.com/Article/details/gsnarwkzv.sHtML

[Q80] 字符串截取
来源：http://www.blog.vehdjk.com/Article/details/ghxpqikbf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gavnakmop.sHtML

[Q81] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/gbfevribr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.bbcook.cn/Article/details/ghzaczdiv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fktsv.cn/Article/details/gvkancssm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/glknoeyhp.sHtML

[Q83] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/grzoeufdg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.tarul.cn/Article/details/gogmrnxdb.sHtML

[Q84] 去除首尾空格
来源：http://3g.vehdjk.com/Article/details/gdexpuhhg.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/gxsvvtnfl.sHtML

[Q85] 数值取整
来源：http://www.blog.sjlbkw.cn/Article/details/gomcwixuj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fktsv.cn/Article/details/guyjktffx.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.tarul.cn/Article/details/gtjasleyj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.epnwcf.com/Article/details/grjoxqwik.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.yfazqb.com/Article/details/ghmkxumjy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.tarul.cn/Article/details/gqqvywmnu.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fktsv.cn/Article/details/gjxvfrgdx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fktsv.cn/Article/details/gugxeqcal.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.yfazqb.com/Article/details/ggoxrabwk.sHtML

[Q89] 判断表是否存在
来源：http://wap.vehdjk.com/Article/details/gqbaqyqae.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.tarul.cn/Article/details/gyzmecfik.sHtML

[Q90] 生成序号列
来源：http://wap.fktsv.cn/Article/details/gtwjwhpct.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.yfazqb.com/Article/details/ggitgecov.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/guzhnoioh.sHtML

R. Bash 专题
来源：http://www.share.epnwcf.com/Article/details/gvuiqemsp.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gcjtcsjcc.sHtML

[R01] shebang 与严格模式
来源：http://m.share.bbcook.cn/Article/details/gdidxhecc.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.vehdjk.com/Article/details/gjwqxgssh.sHtML

set -euo pipefail
来源：http://blog.epnwcf.com/Article/details/gvvvleqlb.sHtML

[R02] 变量赋值与使用
来源：http://blog.epnwcf.com/Article/details/gswboalsj.sHtML

name="Tom"; echo "$name"
来源：http://m.share.tarul.cn/Article/details/gpajakfef.sHtML

[R03] 只读变量
来源：http://3g.bbcook.cn/Article/details/gszljddys.sHtML

readonly PI=3.14
来源：http://baike.epnwcf.com/Article/details/gyzuhsvcu.sHtML

[R04] 位置参数
来源：http://wap.epnwcf.com/Article/details/gqqrpthbn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.vehdjk.com/Article/details/gfswiuzli.sHtML

[R05] 参数默认值
来源：http://www.share.yfazqb.com/Article/details/gbvcqlxsi.sHtML

name="${1:-default}"
来源：http://3g.sjlbkw.cn/Article/details/gbnfsammf.sHtML

[R06] 判断命令是否存在
来源：http://www.share.tarul.cn/Article/details/gbszauzji.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.vehdjk.com/Article/details/grrrvxqza.sHtML

[R07] if 判断文件
来源：http://3g.sjlbkw.cn/Article/details/grbubwwel.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.sjlbkw.cn/Article/details/gkjyrlyih.sHtML

[R08] 数值比较
来源：http://read.share.vehdjk.com/Article/details/gxozimuin.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.epnwcf.com/Article/details/grlhuopig.sHtML

[R09] 字符串比较
来源：http://mobile.yfazqb.com/Article/details/gkbbjxyqo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.yfazqb.com/Article/details/gpdnietek.sHtML

[R10] 正则匹配
来源：http://www.blog.tarul.cn/Article/details/gggjbyacl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.yfazqb.com/Article/details/gndtvnwtd.sHtML

[R11] case 多分支
来源：http://3g.yfazqb.com/Article/details/gdtnbgtgr.sHtML

case "$1" in
来源：http://3g.vehdjk.com/Article/details/gykhksstg.sHtML

start) echo "启动" ;;
来源：http://www.share.yfazqb.com/Article/details/gcgllzegs.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.bbcook.cn/Article/details/gfgsfhgzr.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gyhtbvvvg.sHtML

esac
来源：http://blog.bbcook.cn/Article/details/gilyvluwd.sHtML

[R12] for 遍历文件
来源：http://baike.bbcook.cn/Article/details/gxrxqqvfr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fktsv.cn/Article/details/glwydrgen.sHtML

[R13] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/gqdaqppnc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.tarul.cn/Article/details/gygbykzht.sHtML

[R14] C 风格 for
来源：http://baike.epnwcf.com/Article/details/gfeufpjlt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.vehdjk.com/Article/details/gvsauocui.sHtML

[R15] while 逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gpzdrfhrz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.epnwcf.com/Article/details/gqsymxopv.sHtML

[R16] until 等待条件
来源：http://mobile.yfazqb.com/Article/details/gasvzkowg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/gzhplgeru.sHtML

[R17] 数组定义与取值
来源：http://mobile.tarul.cn/Article/details/gnnxluxch.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.bbcook.cn/Article/details/gcindhqjg.sHtML

[R18] 遍历数组
来源：http://wap.vehdjk.com/Article/details/gvgpgkigf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.epnwcf.com/Article/details/gmkblzgvk.sHtML

[R19] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/ghhfnwzan.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fktsv.cn/Article/details/gyxpotojt.sHtML

[R20] 关联数组（字典）
来源：http://blog.epnwcf.com/Article/details/gvzbtryqk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.yfazqb.com/Article/details/gdchosdsn.sHtML

[R21] 字符串长度
来源：http://mobile.vehdjk.com/Article/details/gygrxbvnx.sHtML

echo "${#s}"
来源：http://m.share.sjlbkw.cn/Article/details/gwokcskhv.sHtML

[R22] 截取子串
来源：http://www.share.yfazqb.com/Article/details/gguujeekp.sHtML

echo "${s:0:5}"
来源：http://www.share.fktsv.cn/Article/details/gzydhanky.sHtML

[R23] 字符串替换
来源：http://blog.epnwcf.com/Article/details/gchtolawg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.epnwcf.com/Article/details/gwbtouwdw.sHtML

[R24] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gpqjqznlc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.bbcook.cn/Article/details/ggesblsoz.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.sjlbkw.cn/Article/details/gfskzjtui.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.epnwcf.com/Article/details/govhccpcl.sHtML

[R26] 命令替换
来源：http://blog.vehdjk.com/Article/details/gljcetfaz.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.epnwcf.com/Article/details/gsjhlpsdr.sHtML

[R27] 算术展开
来源：http://blog.sjlbkw.cn/Article/details/gaejjuunu.sHtML

echo $((1 + 2 * 3))
来源：http://3g.tarul.cn/Article/details/gdppbkiuy.sHtML

[R28] 浮点运算
来源：http://mobile.tarul.cn/Article/details/goyjslqlx.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.sjlbkw.cn/Article/details/gzrjyhugy.sHtML

[R29] 定义函数
来源：http://www.m.share.epnwcf.com/Article/details/gpzrssdmi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.tarul.cn/Article/details/gbninlkac.sHtML

[R30] 函数返回状态码
来源：http://read.share.epnwcf.com/Article/details/gcdvsnykf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fktsv.cn/Article/details/gpqhpiziz.sHtML

[R31] 局部变量
来源：http://www.share.sjlbkw.cn/Article/details/gyktaanms.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.epnwcf.com/Article/details/gsquumfhb.sHtML

[R32] 参数个数校验
来源：http://baike.yfazqb.com/Article/details/gcdaufycj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.vehdjk.com/Article/details/gsproujuq.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.sjlbkw.cn/Article/details/ghjgypcyi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fktsv.cn/Article/details/gtoragzvf.sHtML

[R34] 退出时清理
来源：http://blog.yfazqb.com/Article/details/ghbklfybo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/ggtpzffmp.sHtML

[R35] 后台执行并等待
来源：http://www.share.tarul.cn/Article/details/gaxxppwcx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.sjlbkw.cn/Article/details/geodsdlza.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fktsv.cn/Article/details/gmvzshtec.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.epnwcf.com/Article/details/garioqikl.sHtML

[R37] 把输出赋给变量
来源：http://m.share.yfazqb.com/Article/details/gnqvxikhn.sHtML

files=$(ls -1)
来源：http://www.blog.bbcook.cn/Article/details/gwqqracgx.sHtML

[R38] 管道串联
来源：http://blog.sjlbkw.cn/Article/details/gblwcptcq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.yfazqb.com/Article/details/glwrzevfh.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.yfazqb.com/Article/details/gjhahfpqf.sHtML

cmd > out.log 2>&1
来源：http://mobile.tarul.cn/Article/details/gzmxxirpp.sHtML

[R40] 追加写日志
来源：http://baike.yfazqb.com/Article/details/gzrgceggi.sHtML

echo "log" >> out.log
来源：http://www.m.share.bbcook.cn/Article/details/gvkusqkzj.sHtML

[R41] 丢弃输出
来源：http://3g.bbcook.cn/Article/details/gdawapovy.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.tarul.cn/Article/details/giojtuyea.sHtML

[R42] 输入重定向
来源：http://baike.sjlbkw.cn/Article/details/gmjwqszgu.sHtML

wc -l < a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gjrphukac.sHtML

[R43] 按名字查找文件
来源：http://wap.vehdjk.com/Article/details/gjoutxdfv.sHtML

find . -name "*.log" -type f
来源：http://m.share.vehdjk.com/Article/details/gzyhkhtig.sHtML

[R44] 按修改时间查找
来源：http://mobile.epnwcf.com/Article/details/gkrluplmo.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.vehdjk.com/Article/details/gumgaoeyx.sHtML

[R45] 批量删除
来源：http://m.share.yfazqb.com/Article/details/gcbzsnndq.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fktsv.cn/Article/details/gyiuyokso.sHtML

[R46] 递归替换文件内容
来源：http://wap.yfazqb.com/Article/details/gcvznlcuq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.tarul.cn/Article/details/gingwvnqd.sHtML

[R47] sed 单行替换
来源：http://3g.bbcook.cn/Article/details/gsejakuhh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.vehdjk.com/Article/details/gragwqzbu.sHtML

[R48] awk 取指定列
来源：http://www.blog.vehdjk.com/Article/details/gpyxvgxem.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.epnwcf.com/Article/details/gkbgekrql.sHtML

[R49] awk 带条件
来源：http://read.share.fktsv.cn/Article/details/glwbfukbz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.bbcook.cn/Article/details/gmpwzxjgd.sHtML

[R50] awk 求和
来源：http://3g.epnwcf.com/Article/details/gtqffjsbl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.tarul.cn/Article/details/gqehnszad.sHtML

[R51] 排序去重取前几
来源：http://www.blog.bbcook.cn/Article/details/gihhusizt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.tarul.cn/Article/details/gxqbbbmen.sHtML

[R52] 统计行数
来源：http://3g.bbcook.cn/Article/details/gyrpgqtyi.sHtML

wc -l a.txt
来源：http://www.share.bbcook.cn/Article/details/ggqihvxmd.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fktsv.cn/Article/details/gvtxcncyf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.epnwcf.com/Article/details/gyucqgsda.sHtML

[R54] 比较两个文件
来源：http://mobile.tarul.cn/Article/details/gnbjvkenq.sHtML

diff a.txt b.txt
来源：http://read.share.vehdjk.com/Article/details/gblbzlxif.sHtML

[R55] 压缩与解压
来源：http://wap.vehdjk.com/Article/details/gbjlxwlwy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fktsv.cn/Article/details/gkubjztfr.sHtML

[R56] 远程拷贝
来源：http://www.share.epnwcf.com/Article/details/gbsqtjtgc.sHtML

scp file user@host:/path/
来源：http://baike.epnwcf.com/Article/details/gqahwwydi.sHtML

[R57] 远程执行命令
来源：http://wap.epnwcf.com/Article/details/gvnwnjsxq.sHtML

ssh user@host 'uptime'
来源：http://m.share.epnwcf.com/Article/details/gbexfnswk.sHtML

[R58] 下载文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gktkqgtfk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fktsv.cn/Article/details/gktcfvzwt.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.bbcook.cn/Article/details/gwbkcrerr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fktsv.cn/Article/details/gyycyeywl.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/gasmqdhud.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.tarul.cn/Article/details/gjentndut.sHtML

[R61] 磁盘占用
来源：http://m.share.sjlbkw.cn/Article/details/gmgdldcgz.sHtML

df -h;  du -sh *
来源：http://wap.yfazqb.com/Article/details/gyazdnzqd.sHtML

[R62] 找最占空间的文件
来源：http://wap.fktsv.cn/Article/details/grjsxswji.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.yfazqb.com/Article/details/gwrcakvps.sHtML

[R63] 内存与进程
来源：http://www.blog.vehdjk.com/Article/details/gejnyigag.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.bbcook.cn/Article/details/gshcoukph.sHtML

[R64] 结束进程
来源：http://www.blog.sjlbkw.cn/Article/details/guxgijwri.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.tarul.cn/Article/details/gptlhpwte.sHtML

[R65] 查看端口占用
来源：http://read.share.fktsv.cn/Article/details/gwvmcrplm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fktsv.cn/Article/details/ghedopidy.sHtML

[R66] 定时任务
来源：http://m.share.bbcook.cn/Article/details/gaqfzlzkg.sHtML

crontab -e;  crontab -l
来源：http://m.share.yfazqb.com/Article/details/gdsqehddh.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.tarul.cn/Article/details/gopsmmifr.sHtML

openssl rand -hex 16
来源：http://mobile.fktsv.cn/Article/details/ggxzgtkzz.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.bbcook.cn/Article/details/ghrdhsnnx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/glguvtpgl.sHtML

[R69] 生成随机密码
来源：http://www.blog.bbcook.cn/Article/details/gcvkoxxal.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.vehdjk.com/Article/details/gjbsvkpfo.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fktsv.cn/Article/details/gnjtdcrnm.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.vehdjk.com/Article/details/gzihesfez.sHtML

[R71] 日期格式化
来源：http://3g.tarul.cn/Article/details/gcbbilttf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fktsv.cn/Article/details/gepzhdrlo.sHtML

[R72] 等待端口就绪
来源：http://read.share.yfazqb.com/Article/details/gnutodeau.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/grslnprju.sHtML

[R73] 分割大日志
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkpllyxs.sHtML

split -l 1000 big.log part_
来源：http://www.share.fktsv.cn/Article/details/ghvijhdrf.sHtML

[R74] 批量重命名
来源：http://www.m.share.vehdjk.com/Article/details/gyggibuez.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.sjlbkw.cn/Article/details/gxhlwjhfr.sHtML

[R75] 导出环境变量
来源：http://read.share.fktsv.cn/Article/details/geidwupze.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.vehdjk.com/Article/details/goxlnrxfu.sHtML

[R76] 使用临时文件
来源：http://blog.vehdjk.com/Article/details/gxodwiwah.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gocslhgsr.sHtML

[R77] 读取用户输入
来源：http://3g.bbcook.cn/Article/details/gjbcwumpt.sHtML

read -rp "请输入: " ans
来源：http://3g.fktsv.cn/Article/details/gzihdmqjm.sHtML

[R78] 交互式菜单
来源：http://read.share.yfazqb.com/Article/details/gsedfedbf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.tarul.cn/Article/details/gytoacegx.sHtML

[R79] 解析命令行选项
来源：http://www.share.bbcook.cn/Article/details/grppzbcmq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.sjlbkw.cn/Article/details/govvbhcsw.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fktsv.cn/Article/details/gmbwisplm.sHtML

time ./run.sh
来源：http://read.share.tarul.cn/Article/details/ggvwkhqma.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gimgfqkdz.sHtML

S. C / C++ 专题
来源：http://mobile.yfazqb.com/Article/details/gxjjwavqp.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gdghqidbf.sHtML

[S01] C：Hello World
来源：http://read.share.yfazqb.com/Article/details/gvjfquuya.sHtML

#include <stdio.h>
来源：http://www.blog.bbcook.cn/Article/details/gidnxpbii.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.tarul.cn/Article/details/ghxvfvzlm.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.vehdjk.com/Article/details/grykfcoij.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.bbcook.cn/Article/details/geuygsmut.sHtML

[S03] C：读入整数
来源：http://3g.vehdjk.com/Article/details/gjlwtrhcr.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.vehdjk.com/Article/details/gmbkxotpi.sHtML

[S04] C：字符串复制
来源：http://www.share.fktsv.cn/Article/details/gppvqtghy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.yfazqb.com/Article/details/gvujcdrjk.sHtML

[S05] C：字符串长度
来源：http://read.share.fktsv.cn/Article/details/geoyzektf.sHtML

strlen(s)
来源：http://baike.sjlbkw.cn/Article/details/gwdleiwts.sHtML

[S06] C：字符串比较
来源：http://wap.epnwcf.com/Article/details/gggietcce.sHtML

strcmp(a, b) == 0
来源：http://www.blog.sjlbkw.cn/Article/details/gsfavxvhw.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fktsv.cn/Article/details/gcvucbknq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.tarul.cn/Article/details/gcopkavfq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.bbcook.cn/Article/details/gvtvgnkpb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.vehdjk.com/Article/details/gxzmyohrn.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.epnwcf.com/Article/details/glzgbtcpz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.vehdjk.com/Article/details/gjejnsxbt.sHtML

[S10] C：指针与解引用
来源：http://read.share.fktsv.cn/Article/details/grpeblhyg.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.yfazqb.com/Article/details/gbrdudnnw.sHtML

[S11] C：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gdjoddvmz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.vehdjk.com/Article/details/gvldogtwi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.vehdjk.com/Article/details/ghajcjfsf.sHtML

fclose(f);
来源：http://m.share.vehdjk.com/Article/details/gtvmvzufd.sHtML

[S12] C：写文件
来源：http://wap.epnwcf.com/Article/details/gcikhhpqg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.epnwcf.com/Article/details/gycicdzos.sHtML

[S13] C：宏定义
来源：http://3g.epnwcf.com/Article/details/gdvajzrkv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.sjlbkw.cn/Article/details/gxhkcogat.sHtML

[S14] C：枚举
来源：http://mobile.sjlbkw.cn/Article/details/gpldgjjdl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.yfazqb.com/Article/details/gutkyipxo.sHtML

[S15] C：类型转换
来源：http://mobile.epnwcf.com/Article/details/gjmdfdbvs.sHtML

(double) a / b
来源：http://blog.yfazqb.com/Article/details/gqxuqrqhq.sHtML

[S16] C：位操作置位
来源：http://baike.epnwcf.com/Article/details/gtfwpzmuy.sHtML


<!-- 参考信息 -->