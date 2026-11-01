代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.bbcook.cn/Article/details/gltlzwcfb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.sjlbkw.cn/Article/details/gkdutsgbp.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.yfazqb.com/Article/details/gkuxbmaay.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fktsv.cn/Article/details/gkdeuvrwq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.epnwcf.com/Article/details/gdiwsqhif.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.vehdjk.com/Article/details/gkmruslej.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.yfazqb.com/Article/details/guironzkt.sHtML

[Q41] 多表连接
来源：http://m.share.tarul.cn/Article/details/gjakreuqj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.vehdjk.com/Article/details/gzdzymuge.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.tarul.cn/Article/details/gtbfdgqfs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fktsv.cn/Article/details/gvsdqnajr.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fktsv.cn/Article/details/guskfrdid.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.bbcook.cn/Article/details/gznpcmejl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.sjlbkw.cn/Article/details/glzbxwzcv.sHtML

[Q43] 标量子查询
来源：http://mobile.tarul.cn/Article/details/gcsyzpgsx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fktsv.cn/Article/details/gqcimugmd.sHtML

[Q44] IN 子查询
来源：http://wap.bbcook.cn/Article/details/gqguqwwss.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.tarul.cn/Article/details/gcoizdhiz.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.yfazqb.com/Article/details/gfgcdgkaa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.yfazqb.com/Article/details/gpuecpogw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.yfazqb.com/Article/details/gdtwugcps.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.epnwcf.com/Article/details/gapsuzmql.sHtML

[Q47] 与平均值比较
来源：http://read.share.tarul.cn/Article/details/gptcmsctu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.sjlbkw.cn/Article/details/grhpjtkih.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.bbcook.cn/Article/details/gerapvrjd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.bbcook.cn/Article/details/gmnemmlvm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.sjlbkw.cn/Article/details/gbpxtolal.sHtML

[Q49] 更新单行
来源：http://www.blog.bbcook.cn/Article/details/gjbxgnhzd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.epnwcf.com/Article/details/gmjfjjndd.sHtML

[Q50] 批量更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gosrqvadv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.tarul.cn/Article/details/ghlzeekjc.sHtML

[Q51] 用子查询更新
来源：http://blog.yfazqb.com/Article/details/guirpdsxr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fktsv.cn/Article/details/gyuahqcjw.sHtML

[Q52] 删除指定行
来源：http://wap.tarul.cn/Article/details/gdbmdrjcy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gtkwyvyxo.sHtML

[Q53] 按条件删除
来源：http://www.share.bbcook.cn/Article/details/gfitlfolv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.tarul.cn/Article/details/gkejjxoju.sHtML

[Q54] 清空表
来源：http://wap.vehdjk.com/Article/details/gbboimxez.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.sjlbkw.cn/Article/details/gkhptwvph.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.tarul.cn/Article/details/glikzjhcl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.tarul.cn/Article/details/gzkbrfkul.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.epnwcf.com/Article/details/gnahupvpz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.bbcook.cn/Article/details/gyzxshsfb.sHtML

[Q57] 行号
来源：http://read.share.fktsv.cn/Article/details/gijnffvwv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.bbcook.cn/Article/details/gjakdtwfg.sHtML

[Q58] 累计求和
来源：http://m.share.bbcook.cn/Article/details/guxntyafq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gagpfvsry.sHtML

[Q59] 分组内累计
来源：http://www.share.epnwcf.com/Article/details/gvqinmkhc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gwbxmljgn.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.bbcook.cn/Article/details/gufybtluz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.vehdjk.com/Article/details/gmzlpsdrd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gccvysqrk.sHtML

[Q61] 移动平均
来源：http://baike.yfazqb.com/Article/details/gkldoyvlz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gbqpkeqxb.sHtML

[Q62] 分组占比
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpstktbp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.epnwcf.com/Article/details/gukxcjpgy.sHtML

[Q63] 开启事务
来源：http://blog.yfazqb.com/Article/details/gzwetjufr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.yfazqb.com/Article/details/gobridcdu.sHtML

[Q64] 提交事务
来源：http://m.share.bbcook.cn/Article/details/gnnsoaiba.sHtML

COMMIT;
来源：http://m.share.tarul.cn/Article/details/ghmlfdxhp.sHtML

[Q65] 回滚事务
来源：http://www.share.sjlbkw.cn/Article/details/gjwtdypiq.sHtML

ROLLBACK;
来源：http://baike.epnwcf.com/Article/details/gycuvyski.sHtML

[Q66] 行锁查询
来源：http://www.share.fktsv.cn/Article/details/guucfpckd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.epnwcf.com/Article/details/grwwwhjbf.sHtML

[Q67] 设置隔离级别
来源：http://m.share.tarul.cn/Article/details/gshhxkdmf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.vehdjk.com/Article/details/gysmysouj.sHtML

[Q68] 保存点
来源：http://www.share.epnwcf.com/Article/details/gmhrvhsqh.sHtML

SAVEPOINT sp1;
来源：http://3g.yfazqb.com/Article/details/gmhwyaawl.sHtML

ROLLBACK TO sp1;
来源：http://3g.bbcook.cn/Article/details/goigvbvjl.sHtML

[Q69] 查看执行计划
来源：http://read.share.bbcook.cn/Article/details/gmjvkgyya.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.bbcook.cn/Article/details/giqtgdqza.sHtML

[Q70] 更新统计信息
来源：http://3g.sjlbkw.cn/Article/details/gjvbnkocr.sHtML

ANALYZE TABLE users;
来源：http://read.share.tarul.cn/Article/details/gwacgaznh.sHtML

[Q71] 查看建表语句
来源：http://mobile.bbcook.cn/Article/details/gsygrrlse.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.epnwcf.com/Article/details/gcabufufp.sHtML

[Q72] 查看索引
来源：http://www.m.share.fktsv.cn/Article/details/gixfumdqw.sHtML

SHOW INDEX FROM users;
来源：http://blog.bbcook.cn/Article/details/gcrudgvxq.sHtML

[Q73] 查看表状态
来源：http://www.m.share.epnwcf.com/Article/details/gpardgdgb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.bbcook.cn/Article/details/gfcntkufo.sHtML

[Q74] 强制使用索引
来源：http://baike.fktsv.cn/Article/details/guucqrrmo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.yfazqb.com/Article/details/grrrcweol.sHtML

[Q75] 日期格式化
来源：http://m.share.bbcook.cn/Article/details/gfjowyugt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.epnwcf.com/Article/details/ghaozblpt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.yfazqb.com/Article/details/guexjvaiv.sHtML

[Q76] 按天统计
来源：http://m.share.fktsv.cn/Article/details/gedjgooon.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.yfazqb.com/Article/details/grrtdgbjc.sHtML

[Q77] 时间加减
来源：http://www.m.share.epnwcf.com/Article/details/gxvopsseb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.yfazqb.com/Article/details/gkbrzgifo.sHtML

[Q78] 当前时间
来源：http://www.m.share.fktsv.cn/Article/details/gstmsnlny.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.yfazqb.com/Article/details/ggmxzkzps.sHtML

[Q79] 字符串拼接
来源：http://read.share.vehdjk.com/Article/details/gdkjspmvl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.bbcook.cn/Article/details/gbrfffaxn.sHtML

[Q80] 字符串截取
来源：http://mobile.bbcook.cn/Article/details/ggqjhdfsz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.yfazqb.com/Article/details/gyqvfnfpj.sHtML

[Q81] 字符串替换
来源：http://www.share.fktsv.cn/Article/details/gmvbmeyzi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.vehdjk.com/Article/details/guaelxauw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.yfazqb.com/Article/details/gcwafsjjy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gosrjhkiw.sHtML

[Q83] 大小写转换
来源：http://3g.epnwcf.com/Article/details/gqdujqyqe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gsibviznc.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.bbcook.cn/Article/details/gbngztmix.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/goklkrmvn.sHtML

[Q85] 数值取整
来源：http://wap.fktsv.cn/Article/details/ghrgywjzs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.vehdjk.com/Article/details/gchvyqolr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.yfazqb.com/Article/details/gajqyidag.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.tarul.cn/Article/details/gislbudyt.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.bbcook.cn/Article/details/gexwavrfr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.sjlbkw.cn/Article/details/glzythier.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.vehdjk.com/Article/details/gftzihaxs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.epnwcf.com/Article/details/glicrgdeg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.epnwcf.com/Article/details/gttbscmax.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.epnwcf.com/Article/details/gugnygqhd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fktsv.cn/Article/details/gpopmkduv.sHtML

[Q90] 生成序号列
来源：http://www.m.share.yfazqb.com/Article/details/gizdxqztp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.bbcook.cn/Article/details/gpvngaglf.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/grgcwjpbl.sHtML

R. Bash 专题
来源：http://3g.bbcook.cn/Article/details/ghxakynld.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gjfkppvdj.sHtML

[R01] shebang 与严格模式
来源：http://wap.yfazqb.com/Article/details/gnxvzxjsk.sHtML

#!/usr/bin/env bash
来源：http://blog.fktsv.cn/Article/details/gonawdixr.sHtML

set -euo pipefail
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsiywbqx.sHtML

[R02] 变量赋值与使用
来源：http://3g.fktsv.cn/Article/details/gbqjzcbdq.sHtML

name="Tom"; echo "$name"
来源：http://read.share.vehdjk.com/Article/details/gsnpdayie.sHtML

[R03] 只读变量
来源：http://blog.sjlbkw.cn/Article/details/ggviljung.sHtML

readonly PI=3.14
来源：http://read.share.tarul.cn/Article/details/gepawhyhn.sHtML

[R04] 位置参数
来源：http://blog.epnwcf.com/Article/details/gvjjdsdxs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fktsv.cn/Article/details/ggzwyzgzt.sHtML

[R05] 参数默认值
来源：http://3g.yfazqb.com/Article/details/goymnoxop.sHtML

name="${1:-default}"
来源：http://baike.vehdjk.com/Article/details/gnvuywfxq.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.bbcook.cn/Article/details/gelqgpmnc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.epnwcf.com/Article/details/gysfueicn.sHtML

[R07] if 判断文件
来源：http://3g.tarul.cn/Article/details/gdxblyyke.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.tarul.cn/Article/details/gwkuvvnmf.sHtML

[R08] 数值比较
来源：http://www.share.sjlbkw.cn/Article/details/gyzvfdwyl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.epnwcf.com/Article/details/gtdhrtxcm.sHtML

[R09] 字符串比较
来源：http://www.blog.bbcook.cn/Article/details/gairmgugg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.vehdjk.com/Article/details/gveprurfi.sHtML

[R10] 正则匹配
来源：http://baike.tarul.cn/Article/details/grcxtxasf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fktsv.cn/Article/details/gyguzumtk.sHtML

[R11] case 多分支
来源：http://www.m.share.yfazqb.com/Article/details/gfsuvtdpl.sHtML

case "$1" in
来源：http://wap.vehdjk.com/Article/details/gwdqlwajp.sHtML

start) echo "启动" ;;
来源：http://blog.vehdjk.com/Article/details/gmkbuhvvd.sHtML

stop)  echo "停止" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gzqytgmyc.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.vehdjk.com/Article/details/gcbfbgwgm.sHtML

esac
来源：http://m.share.bbcook.cn/Article/details/gcaojenai.sHtML

[R12] for 遍历文件
来源：http://www.m.share.tarul.cn/Article/details/gzmepjzeo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.bbcook.cn/Article/details/grqnlcbix.sHtML

[R13] for 计数循环
来源：http://www.blog.yfazqb.com/Article/details/gfvtynsun.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.sjlbkw.cn/Article/details/gynrhjlay.sHtML

[R14] C 风格 for
来源：http://read.share.tarul.cn/Article/details/gpngrflky.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.bbcook.cn/Article/details/gaswmpqws.sHtML

[R15] while 逐行读文件
来源：http://mobile.epnwcf.com/Article/details/gjantuolw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.bbcook.cn/Article/details/gsyalzshx.sHtML

[R16] until 等待条件
来源：http://wap.fktsv.cn/Article/details/gyfxhhmpm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/gauefzqjv.sHtML

[R17] 数组定义与取值
来源：http://mobile.vehdjk.com/Article/details/gjkpfjcpm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.yfazqb.com/Article/details/gjnvddreo.sHtML

[R18] 遍历数组
来源：http://www.share.sjlbkw.cn/Article/details/gfrqjrqbv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.tarul.cn/Article/details/gpgdcpzff.sHtML

[R19] 数组长度
来源：http://read.share.bbcook.cn/Article/details/gwnphkcbz.sHtML

echo "${#arr[@]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gtvljyzdj.sHtML

[R20] 关联数组（字典）
来源：http://www.share.epnwcf.com/Article/details/gzucyqqoy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.yfazqb.com/Article/details/gbpyeurdt.sHtML

[R21] 字符串长度
来源：http://baike.tarul.cn/Article/details/gxhqpxuod.sHtML

echo "${#s}"
来源：http://3g.yfazqb.com/Article/details/gfiqzcola.sHtML

[R22] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gswvoxkmu.sHtML

echo "${s:0:5}"
来源：http://m.share.sjlbkw.cn/Article/details/gesdxlomo.sHtML

[R23] 字符串替换
来源：http://m.share.epnwcf.com/Article/details/gwqmyzpsb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.sjlbkw.cn/Article/details/gorvccvue.sHtML

[R24] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/gxfxlznki.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.bbcook.cn/Article/details/ggvmiaenm.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.bbcook.cn/Article/details/gbjeiztdg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.tarul.cn/Article/details/gngleoray.sHtML

[R26] 命令替换
来源：http://mobile.epnwcf.com/Article/details/ggiykaphf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.vehdjk.com/Article/details/gufwuibdg.sHtML

[R27] 算术展开
来源：http://www.share.vehdjk.com/Article/details/gjiawknfl.sHtML

echo $((1 + 2 * 3))
来源：http://blog.bbcook.cn/Article/details/ghvwmsrxl.sHtML

[R28] 浮点运算
来源：http://read.share.fktsv.cn/Article/details/grdubvmfm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.sjlbkw.cn/Article/details/gewobgohg.sHtML

[R29] 定义函数
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnhkrhzq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fktsv.cn/Article/details/ghayzvhcz.sHtML

[R30] 函数返回状态码
来源：http://baike.sjlbkw.cn/Article/details/gxtxmyprm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.vehdjk.com/Article/details/gterhknrh.sHtML

[R31] 局部变量
来源：http://www.m.share.yfazqb.com/Article/details/ghevsmoqw.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.yfazqb.com/Article/details/gjuggmfaa.sHtML

[R32] 参数个数校验
来源：http://3g.bbcook.cn/Article/details/gmiyzprrk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/gneopxwzg.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.bbcook.cn/Article/details/guplzgnub.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.sjlbkw.cn/Article/details/gyrchkklh.sHtML

[R34] 退出时清理
来源：http://wap.epnwcf.com/Article/details/gswuhgrcm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fktsv.cn/Article/details/glhtfhhzc.sHtML

[R35] 后台执行并等待
来源：http://mobile.vehdjk.com/Article/details/gokcivdey.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.tarul.cn/Article/details/gqciiucmp.sHtML

[R36] 并发执行多个任务
来源：http://m.share.sjlbkw.cn/Article/details/gdoucxuyk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fktsv.cn/Article/details/gapliyugi.sHtML

[R37] 把输出赋给变量
来源：http://3g.fktsv.cn/Article/details/gppkoqrrg.sHtML

files=$(ls -1)
来源：http://read.share.sjlbkw.cn/Article/details/guwxhsyiu.sHtML

[R38] 管道串联
来源：http://read.share.bbcook.cn/Article/details/guonevkxc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fktsv.cn/Article/details/gakuzbmua.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.yfazqb.com/Article/details/gekbfzvvw.sHtML

cmd > out.log 2>&1
来源：http://3g.epnwcf.com/Article/details/gvcdbtsja.sHtML

[R40] 追加写日志
来源：http://www.m.share.epnwcf.com/Article/details/gplimyhcc.sHtML

echo "log" >> out.log
来源：http://www.share.sjlbkw.cn/Article/details/gerrsktam.sHtML

[R41] 丢弃输出
来源：http://m.share.epnwcf.com/Article/details/gupnrqfbk.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.tarul.cn/Article/details/gujzlekcu.sHtML

[R42] 输入重定向
来源：http://blog.epnwcf.com/Article/details/gfrddplku.sHtML

wc -l < a.txt
来源：http://mobile.bbcook.cn/Article/details/goivwlkdp.sHtML

[R43] 按名字查找文件
来源：http://www.share.sjlbkw.cn/Article/details/gjjjjgnxs.sHtML

find . -name "*.log" -type f
来源：http://read.share.tarul.cn/Article/details/gsxdvqvye.sHtML

[R44] 按修改时间查找
来源：http://read.share.yfazqb.com/Article/details/gjfilrelc.sHtML

find . -mtime -7 -type f
来源：http://www.blog.vehdjk.com/Article/details/gjkmleypg.sHtML

[R45] 批量删除
来源：http://www.blog.sjlbkw.cn/Article/details/gzqteadlm.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.yfazqb.com/Article/details/gdlkgdxvv.sHtML

[R46] 递归替换文件内容
来源：http://wap.fktsv.cn/Article/details/gsncsekjs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.sjlbkw.cn/Article/details/grotokpwg.sHtML

[R47] sed 单行替换
来源：http://m.share.epnwcf.com/Article/details/gjvuoqqyc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.yfazqb.com/Article/details/ghoqdblsw.sHtML

[R48] awk 取指定列
来源：http://baike.tarul.cn/Article/details/gilsgmqfh.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.bbcook.cn/Article/details/gqcheeund.sHtML

[R49] awk 带条件
来源：http://read.share.tarul.cn/Article/details/gmcrjsgpq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.yfazqb.com/Article/details/gzpfdnesy.sHtML

[R50] awk 求和
来源：http://m.share.tarul.cn/Article/details/gulclezfk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fktsv.cn/Article/details/ghuhgkgwf.sHtML

[R51] 排序去重取前几
来源：http://m.share.vehdjk.com/Article/details/ggzrzpyty.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.bbcook.cn/Article/details/gwepqtlcx.sHtML

[R52] 统计行数
来源：http://read.share.vehdjk.com/Article/details/ghmptgzma.sHtML

wc -l a.txt
来源：http://www.share.bbcook.cn/Article/details/gromuqqnp.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fktsv.cn/Article/details/gxjfokyxv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.bbcook.cn/Article/details/gsfvrvqzd.sHtML

[R54] 比较两个文件
来源：http://www.blog.bbcook.cn/Article/details/gegprnthd.sHtML

diff a.txt b.txt
来源：http://3g.vehdjk.com/Article/details/goulcrucz.sHtML

[R55] 压缩与解压
来源：http://read.share.sjlbkw.cn/Article/details/gcuycklva.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.vehdjk.com/Article/details/glcytgbtx.sHtML

[R56] 远程拷贝
来源：http://wap.yfazqb.com/Article/details/gnjqdadzk.sHtML

scp file user@host:/path/
来源：http://read.share.sjlbkw.cn/Article/details/gctiavkgm.sHtML

[R57] 远程执行命令
来源：http://baike.tarul.cn/Article/details/gtnkulrmb.sHtML

ssh user@host 'uptime'
来源：http://m.share.yfazqb.com/Article/details/gajwyhasn.sHtML

[R58] 下载文件
来源：http://3g.epnwcf.com/Article/details/gyhqvbwws.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.epnwcf.com/Article/details/ghfitgtkb.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fktsv.cn/Article/details/gtenzsdhs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.bbcook.cn/Article/details/gwzbcvhoy.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.vehdjk.com/Article/details/gchajktmk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.sjlbkw.cn/Article/details/gktqxnhqj.sHtML

[R61] 磁盘占用
来源：http://www.share.fktsv.cn/Article/details/gzrvzbpbt.sHtML

df -h;  du -sh *
来源：http://www.m.share.epnwcf.com/Article/details/gxhrrozpb.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.tarul.cn/Article/details/gnevvewrq.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.tarul.cn/Article/details/gqabazbdx.sHtML

[R63] 内存与进程
来源：http://mobile.yfazqb.com/Article/details/gpnnmckfr.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.bbcook.cn/Article/details/gvgnuvjfn.sHtML

[R64] 结束进程
来源：http://wap.bbcook.cn/Article/details/gyvihujkt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.sjlbkw.cn/Article/details/gbteizzim.sHtML

[R65] 查看端口占用
来源：http://wap.epnwcf.com/Article/details/ggngjeitp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fktsv.cn/Article/details/gfmjmwepf.sHtML

[R66] 定时任务
来源：http://read.share.yfazqb.com/Article/details/gkncqprrp.sHtML

crontab -e;  crontab -l
来源：http://3g.bbcook.cn/Article/details/gtourmalx.sHtML

[R67] 生成随机十六进制串
来源：http://baike.bbcook.cn/Article/details/gjiaddthw.sHtML

openssl rand -hex 16
来源：http://baike.sjlbkw.cn/Article/details/gjykrxfso.sHtML

[R68] 计算文件校验值
来源：http://baike.fktsv.cn/Article/details/gdsnowacn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.bbcook.cn/Article/details/gbmvyezyl.sHtML

[R69] 生成随机密码
来源：http://m.share.bbcook.cn/Article/details/gziytexje.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.yfazqb.com/Article/details/ggcegamss.sHtML

[R70] 时间戳与互转
来源：http://baike.fktsv.cn/Article/details/ggzxqutvn.sHtML

date +%s;  date -d @1700000000
来源：http://blog.bbcook.cn/Article/details/gzsnpqeat.sHtML

[R71] 日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/gobhhwzcn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.vehdjk.com/Article/details/gmjmjwryx.sHtML

[R72] 等待端口就绪
来源：http://baike.yfazqb.com/Article/details/gfqtykoyr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fktsv.cn/Article/details/giqlybvkd.sHtML

[R73] 分割大日志
来源：http://baike.vehdjk.com/Article/details/gwddqmxzq.sHtML

split -l 1000 big.log part_
来源：http://mobile.yfazqb.com/Article/details/garqlhexh.sHtML

[R74] 批量重命名
来源：http://wap.fktsv.cn/Article/details/glhxwqbxs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.vehdjk.com/Article/details/glldlykyu.sHtML

[R75] 导出环境变量
来源：http://baike.sjlbkw.cn/Article/details/gaaogpkco.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fktsv.cn/Article/details/gnwyvhiaw.sHtML

[R76] 使用临时文件
来源：http://www.blog.bbcook.cn/Article/details/gylewjinc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/gyhdmqcbd.sHtML

[R77] 读取用户输入
来源：http://wap.sjlbkw.cn/Article/details/gmoltoomt.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.yfazqb.com/Article/details/gixozkxtn.sHtML

[R78] 交互式菜单
来源：http://wap.tarul.cn/Article/details/gtfgdzlri.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.bbcook.cn/Article/details/gcyyrrazc.sHtML

[R79] 解析命令行选项
来源：http://baike.epnwcf.com/Article/details/gbcqaolfn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.yfazqb.com/Article/details/galmgndgp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.sjlbkw.cn/Article/details/gginjzbqj.sHtML

time ./run.sh
来源：http://www.m.share.yfazqb.com/Article/details/gbmkpihwz.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gktkmgdwc.sHtML

S. C / C++ 专题
来源：http://www.m.share.bbcook.cn/Article/details/gjxhugfze.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbvxquogc.sHtML

[S01] C：Hello World
来源：http://read.share.epnwcf.com/Article/details/gwdbnxqus.sHtML

#include <stdio.h>
来源：http://baike.bbcook.cn/Article/details/gfhblzccx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.yfazqb.com/Article/details/gkerezdgj.sHtML

[S02] C：变量与格式化输出
来源：http://blog.bbcook.cn/Article/details/gxfxaaspm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.yfazqb.com/Article/details/gdzfyblfk.sHtML

[S03] C：读入整数
来源：http://baike.yfazqb.com/Article/details/gbzdhuqnr.sHtML

int x; scanf("%d", &x);
来源：http://blog.tarul.cn/Article/details/gfcsuyozk.sHtML

[S04] C：字符串复制
来源：http://wap.fktsv.cn/Article/details/gxtnalzwf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.epnwcf.com/Article/details/gpyxyakqu.sHtML

[S05] C：字符串长度
来源：http://blog.vehdjk.com/Article/details/gpednxbbx.sHtML

strlen(s)
来源：http://wap.fktsv.cn/Article/details/gdsnobkfg.sHtML

[S06] C：字符串比较
来源：http://wap.vehdjk.com/Article/details/goagffsre.sHtML

strcmp(a, b) == 0
来源：http://3g.sjlbkw.cn/Article/details/gxxqvzufk.sHtML

[S07] C：数组遍历求和
来源：http://baike.epnwcf.com/Article/details/gbkcqjgpn.sHtML


<!-- 参考信息 -->