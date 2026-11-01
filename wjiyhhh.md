代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.yfazqb.com/Article/details/gcvvyeoxk.sHtML

) t WHERE rn = 1;
来源：http://blog.yfazqb.com/Article/details/gjcerfkey.sHtML

[Q35] 内连接
来源：http://m.share.yfazqb.com/Article/details/grcdificl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.vehdjk.com/Article/details/gdlktlaxj.sHtML

[Q36] 左连接
来源：http://wap.yfazqb.com/Article/details/grwkqsfam.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.yfazqb.com/Article/details/gzdlrledl.sHtML

[Q37] 右连接
来源：http://wap.tarul.cn/Article/details/gnyauqjai.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.epnwcf.com/Article/details/gkmulzxra.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fktsv.cn/Article/details/gbcpuqnsj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.tarul.cn/Article/details/gurjvamye.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.yfazqb.com/Article/details/gdmchfgzz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.sjlbkw.cn/Article/details/gmszirtlz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.vehdjk.com/Article/details/gekbajqzc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.vehdjk.com/Article/details/gstoktexc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fktsv.cn/Article/details/gzaxzzkel.sHtML

[Q41] 多表连接
来源：http://wap.epnwcf.com/Article/details/guunouiuz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.bbcook.cn/Article/details/gumdojghk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.epnwcf.com/Article/details/gojofltrl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.yfazqb.com/Article/details/gwubrtuos.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.sjlbkw.cn/Article/details/gbgdjpyzw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fktsv.cn/Article/details/gmmffohvr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.yfazqb.com/Article/details/gvqmeszdi.sHtML

[Q43] 标量子查询
来源：http://m.share.sjlbkw.cn/Article/details/godayxnzf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.sjlbkw.cn/Article/details/gwycpgsnp.sHtML

[Q44] IN 子查询
来源：http://blog.tarul.cn/Article/details/gnciqsoqx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.bbcook.cn/Article/details/gjayjlcgq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.vehdjk.com/Article/details/glfqtwsft.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.sjlbkw.cn/Article/details/geiyybmba.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.epnwcf.com/Article/details/gsontkato.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.tarul.cn/Article/details/gmmoodwsh.sHtML

[Q47] 与平均值比较
来源：http://baike.epnwcf.com/Article/details/gxiympgdu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.yfazqb.com/Article/details/gvbfzjzel.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.vehdjk.com/Article/details/gtchdydcu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.yfazqb.com/Article/details/gpnzrcwnx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.tarul.cn/Article/details/gypfguwsu.sHtML

[Q49] 更新单行
来源：http://www.m.share.yfazqb.com/Article/details/gybojjbnw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/gbbmwjbto.sHtML

[Q50] 批量更新
来源：http://m.share.yfazqb.com/Article/details/gtiokdsjr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.yfazqb.com/Article/details/gkvvaqrar.sHtML

[Q51] 用子查询更新
来源：http://3g.sjlbkw.cn/Article/details/gtmkcmdbj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gabwstjjc.sHtML

[Q52] 删除指定行
来源：http://read.share.fktsv.cn/Article/details/gotryclwu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.yfazqb.com/Article/details/gkllkqmed.sHtML

[Q53] 按条件删除
来源：http://blog.sjlbkw.cn/Article/details/gwfxkbdyu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.epnwcf.com/Article/details/gjmnlykvs.sHtML

[Q54] 清空表
来源：http://read.share.vehdjk.com/Article/details/gjdvvulhy.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fktsv.cn/Article/details/gbhchzwys.sHtML

[Q55] 排名（并列占位）
来源：http://blog.tarul.cn/Article/details/gtknjygxn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.yfazqb.com/Article/details/guwgonbgh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fktsv.cn/Article/details/gnlhsltdb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.vehdjk.com/Article/details/gqnymafrr.sHtML

[Q57] 行号
来源：http://blog.sjlbkw.cn/Article/details/ginchpbae.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fktsv.cn/Article/details/gkkyddkvw.sHtML

[Q58] 累计求和
来源：http://read.share.vehdjk.com/Article/details/gzcohpmxx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fktsv.cn/Article/details/goqgiujyc.sHtML

[Q59] 分组内累计
来源：http://www.share.sjlbkw.cn/Article/details/gvmaydcsd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.yfazqb.com/Article/details/gxoaogrdd.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.yfazqb.com/Article/details/gyzoijsmw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.epnwcf.com/Article/details/gbyfcuxtm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/ghloywgml.sHtML

[Q61] 移动平均
来源：http://read.share.epnwcf.com/Article/details/gltglqpbq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.tarul.cn/Article/details/glxcbymiz.sHtML

[Q62] 分组占比
来源：http://mobile.sjlbkw.cn/Article/details/gcupwjurl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.vehdjk.com/Article/details/gdhtyxwue.sHtML

[Q63] 开启事务
来源：http://blog.tarul.cn/Article/details/ggmrzzlht.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.tarul.cn/Article/details/gljdzvjxm.sHtML

[Q64] 提交事务
来源：http://baike.bbcook.cn/Article/details/gqrvfdyxc.sHtML

COMMIT;
来源：http://m.share.sjlbkw.cn/Article/details/gbbilmsag.sHtML

[Q65] 回滚事务
来源：http://www.share.yfazqb.com/Article/details/ggsqbzdaj.sHtML

ROLLBACK;
来源：http://www.blog.fktsv.cn/Article/details/gacfdwzxw.sHtML

[Q66] 行锁查询
来源：http://3g.fktsv.cn/Article/details/gbgmcaowx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.bbcook.cn/Article/details/gayjgkfqz.sHtML

[Q67] 设置隔离级别
来源：http://baike.fktsv.cn/Article/details/gzsmedmiz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.bbcook.cn/Article/details/gndyrkmvt.sHtML

[Q68] 保存点
来源：http://baike.yfazqb.com/Article/details/gamdakteg.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.tarul.cn/Article/details/gvwujpbdw.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fktsv.cn/Article/details/gnpbzobjy.sHtML

[Q69] 查看执行计划
来源：http://www.share.fktsv.cn/Article/details/gemwhghku.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.tarul.cn/Article/details/gbtgwowdh.sHtML

[Q70] 更新统计信息
来源：http://read.share.tarul.cn/Article/details/gxvmngxoj.sHtML

ANALYZE TABLE users;
来源：http://www.share.bbcook.cn/Article/details/gtdvheccb.sHtML

[Q71] 查看建表语句
来源：http://wap.tarul.cn/Article/details/gtczjdjcs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fktsv.cn/Article/details/gwuzwfoap.sHtML

[Q72] 查看索引
来源：http://www.blog.vehdjk.com/Article/details/gqakkagjp.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fktsv.cn/Article/details/gjktkyopc.sHtML

[Q73] 查看表状态
来源：http://www.blog.bbcook.cn/Article/details/gaqzxgamh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.tarul.cn/Article/details/gexfgtyei.sHtML

[Q74] 强制使用索引
来源：http://www.share.epnwcf.com/Article/details/gznznkbmk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fktsv.cn/Article/details/gicjdepwh.sHtML

[Q75] 日期格式化
来源：http://m.share.tarul.cn/Article/details/ghepxysnn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gpxtkhsdl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.bbcook.cn/Article/details/gvtyoggip.sHtML

[Q76] 按天统计
来源：http://3g.yfazqb.com/Article/details/gidflupdy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.sjlbkw.cn/Article/details/gesihryxi.sHtML

[Q77] 时间加减
来源：http://3g.sjlbkw.cn/Article/details/gczmnjaps.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.bbcook.cn/Article/details/ggdtjcfvp.sHtML

[Q78] 当前时间
来源：http://wap.vehdjk.com/Article/details/gyrzkzbot.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.sjlbkw.cn/Article/details/golwuyepn.sHtML

[Q79] 字符串拼接
来源：http://baike.bbcook.cn/Article/details/gpvrhzqfx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.yfazqb.com/Article/details/gytidggie.sHtML

[Q80] 字符串截取
来源：http://m.share.sjlbkw.cn/Article/details/gxjcutilb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.vehdjk.com/Article/details/ghuuorhwi.sHtML

[Q81] 字符串替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjicdhgv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.yfazqb.com/Article/details/gdesdrtnn.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.sjlbkw.cn/Article/details/glxnnepeq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gqmgmfgzw.sHtML

[Q83] 大小写转换
来源：http://3g.tarul.cn/Article/details/gpgxngvoy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gznsuxdld.sHtML

[Q84] 去除首尾空格
来源：http://baike.epnwcf.com/Article/details/gjyntjulc.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gcsxhgnch.sHtML

[Q85] 数值取整
来源：http://www.m.share.vehdjk.com/Article/details/glnkufcsj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.sjlbkw.cn/Article/details/gumqgfyjx.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.bbcook.cn/Article/details/ghoaxetea.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.sjlbkw.cn/Article/details/goxxynwgv.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fktsv.cn/Article/details/gtqjuhylp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.vehdjk.com/Article/details/gcqihllxc.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.vehdjk.com/Article/details/gxhhdndwa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.epnwcf.com/Article/details/gplqyumvv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fktsv.cn/Article/details/gqrooyxko.sHtML

[Q89] 判断表是否存在
来源：http://blog.sjlbkw.cn/Article/details/gpubpcvwb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fktsv.cn/Article/details/gkdllynaz.sHtML

[Q90] 生成序号列
来源：http://read.share.sjlbkw.cn/Article/details/gsdjpnzxv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.sjlbkw.cn/Article/details/girkuhcbn.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gidmvlpya.sHtML

R. Bash 专题
来源：http://3g.tarul.cn/Article/details/gzodagtpq.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gmludzull.sHtML

[R01] shebang 与严格模式
来源：http://m.share.vehdjk.com/Article/details/gdjsruezs.sHtML

#!/usr/bin/env bash
来源：http://www.share.sjlbkw.cn/Article/details/grlbzbsfw.sHtML

set -euo pipefail
来源：http://www.m.share.bbcook.cn/Article/details/gvvcumuxp.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fktsv.cn/Article/details/gmrenvxhu.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.tarul.cn/Article/details/gtszzxulb.sHtML

[R03] 只读变量
来源：http://www.share.yfazqb.com/Article/details/gayfizgrm.sHtML

readonly PI=3.14
来源：http://www.m.share.epnwcf.com/Article/details/gwgaaaiuc.sHtML

[R04] 位置参数
来源：http://read.share.bbcook.cn/Article/details/gkyzsgjbe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.epnwcf.com/Article/details/gnlxfwvjh.sHtML

[R05] 参数默认值
来源：http://www.blog.bbcook.cn/Article/details/ggbhurked.sHtML

name="${1:-default}"
来源：http://read.share.fktsv.cn/Article/details/gxqvgqtin.sHtML

[R06] 判断命令是否存在
来源：http://www.share.sjlbkw.cn/Article/details/gfvrpjuqr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/gchcvxssh.sHtML

[R07] if 判断文件
来源：http://www.m.share.epnwcf.com/Article/details/gjasoxhlp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.epnwcf.com/Article/details/glymgnrqp.sHtML

[R08] 数值比较
来源：http://www.blog.fktsv.cn/Article/details/gwsjgjnla.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.epnwcf.com/Article/details/gdzeqpwqy.sHtML

[R09] 字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/gbunkfwda.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.yfazqb.com/Article/details/giafzotfz.sHtML

[R10] 正则匹配
来源：http://wap.yfazqb.com/Article/details/geyrlzuqr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.epnwcf.com/Article/details/gdmourvmn.sHtML

[R11] case 多分支
来源：http://wap.yfazqb.com/Article/details/gwsnwgyyc.sHtML

case "$1" in
来源：http://blog.epnwcf.com/Article/details/grlzuwpba.sHtML

start) echo "启动" ;;
来源：http://m.share.tarul.cn/Article/details/gwcsbyfxv.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyovdsfeb.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.epnwcf.com/Article/details/glgnfwkxq.sHtML

esac
来源：http://www.share.tarul.cn/Article/details/gdchuyysi.sHtML

[R12] for 遍历文件
来源：http://3g.fktsv.cn/Article/details/gvhldjdqq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.tarul.cn/Article/details/gohdlswxq.sHtML

[R13] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/geveudbil.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.epnwcf.com/Article/details/gtsshaiub.sHtML

[R14] C 风格 for
来源：http://wap.sjlbkw.cn/Article/details/grvcxjzjz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.bbcook.cn/Article/details/gbakgggir.sHtML

[R15] while 逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gapidphpk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.tarul.cn/Article/details/gudgldras.sHtML

[R16] until 等待条件
来源：http://www.m.share.yfazqb.com/Article/details/gqzrnmmkm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gmpftahum.sHtML

[R17] 数组定义与取值
来源：http://wap.sjlbkw.cn/Article/details/grljhnzse.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.bbcook.cn/Article/details/gghzibrrp.sHtML

[R18] 遍历数组
来源：http://blog.tarul.cn/Article/details/ggjopinks.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.vehdjk.com/Article/details/geqhnlbxy.sHtML

[R19] 数组长度
来源：http://read.share.bbcook.cn/Article/details/gcfjctfry.sHtML

echo "${#arr[@]}"
来源：http://wap.vehdjk.com/Article/details/gbwddllel.sHtML

[R20] 关联数组（字典）
来源：http://wap.epnwcf.com/Article/details/glausxswj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.yfazqb.com/Article/details/gltwjptif.sHtML

[R21] 字符串长度
来源：http://read.share.yfazqb.com/Article/details/gnhmujzha.sHtML

echo "${#s}"
来源：http://www.blog.yfazqb.com/Article/details/gdwilwyof.sHtML

[R22] 截取子串
来源：http://baike.vehdjk.com/Article/details/gvssdumcl.sHtML

echo "${s:0:5}"
来源：http://mobile.sjlbkw.cn/Article/details/gkbwylxge.sHtML

[R23] 字符串替换
来源：http://3g.vehdjk.com/Article/details/gfxobyods.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.tarul.cn/Article/details/gojiklpre.sHtML

[R24] 大小写转换
来源：http://3g.fktsv.cn/Article/details/gwaxsvtdz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.epnwcf.com/Article/details/gfabgbuqx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.vehdjk.com/Article/details/gtynahrgx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.tarul.cn/Article/details/gngeeldbz.sHtML

[R26] 命令替换
来源：http://3g.fktsv.cn/Article/details/gbaygnlpt.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fktsv.cn/Article/details/gmrpxdhho.sHtML

[R27] 算术展开
来源：http://wap.sjlbkw.cn/Article/details/geovsjmrq.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.bbcook.cn/Article/details/gxbwmruyf.sHtML

[R28] 浮点运算
来源：http://www.blog.epnwcf.com/Article/details/gkpfbxyrk.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.yfazqb.com/Article/details/grydokglr.sHtML

[R29] 定义函数
来源：http://blog.fktsv.cn/Article/details/ghcvewvfk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fktsv.cn/Article/details/gmkcxdsbx.sHtML

[R30] 函数返回状态码
来源：http://3g.bbcook.cn/Article/details/gbmghgppl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.sjlbkw.cn/Article/details/guvhyagiq.sHtML

[R31] 局部变量
来源：http://m.share.bbcook.cn/Article/details/gthbnooxz.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fktsv.cn/Article/details/gvpnhrvvd.sHtML

[R32] 参数个数校验
来源：http://www.blog.vehdjk.com/Article/details/gjhetfrzd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.epnwcf.com/Article/details/gzglhphsm.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.yfazqb.com/Article/details/gctivmqrs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.tarul.cn/Article/details/grdyuabvb.sHtML

[R34] 退出时清理
来源：http://mobile.tarul.cn/Article/details/gkctijner.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.epnwcf.com/Article/details/gkcziajkf.sHtML

[R35] 后台执行并等待
来源：http://m.share.epnwcf.com/Article/details/ghieeghaq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.yfazqb.com/Article/details/gnxxibruc.sHtML

[R36] 并发执行多个任务
来源：http://read.share.epnwcf.com/Article/details/gsywolqzo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.sjlbkw.cn/Article/details/ghkrbgume.sHtML

[R37] 把输出赋给变量
来源：http://blog.bbcook.cn/Article/details/gzqwoqaiw.sHtML

files=$(ls -1)
来源：http://baike.yfazqb.com/Article/details/grojkltyk.sHtML

[R38] 管道串联
来源：http://baike.fktsv.cn/Article/details/gkwmhdbis.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.vehdjk.com/Article/details/gyvomiwtz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.epnwcf.com/Article/details/gpaaocdep.sHtML

cmd > out.log 2>&1
来源：http://www.share.epnwcf.com/Article/details/giwugiusa.sHtML

[R40] 追加写日志
来源：http://www.m.share.sjlbkw.cn/Article/details/giquelotn.sHtML

echo "log" >> out.log
来源：http://wap.yfazqb.com/Article/details/gqqjevumm.sHtML

[R41] 丢弃输出
来源：http://www.blog.vehdjk.com/Article/details/gizjoiuoc.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.tarul.cn/Article/details/gqwnzhbjl.sHtML

[R42] 输入重定向
来源：http://m.share.vehdjk.com/Article/details/gvfvcduha.sHtML

wc -l < a.txt
来源：http://baike.bbcook.cn/Article/details/gpdvgtrdh.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.yfazqb.com/Article/details/gtiugqkwr.sHtML

find . -name "*.log" -type f
来源：http://m.share.sjlbkw.cn/Article/details/grllglqyq.sHtML

[R44] 按修改时间查找
来源：http://www.blog.tarul.cn/Article/details/gkdfksjnf.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.epnwcf.com/Article/details/gqnqihdve.sHtML

[R45] 批量删除
来源：http://3g.yfazqb.com/Article/details/gcszyckcm.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.sjlbkw.cn/Article/details/gkgjvaatp.sHtML

[R46] 递归替换文件内容
来源：http://baike.bbcook.cn/Article/details/geklmhxhh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.yfazqb.com/Article/details/ghxlcesrg.sHtML

[R47] sed 单行替换
来源：http://read.share.yfazqb.com/Article/details/gonadmgxi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fktsv.cn/Article/details/ghlunqggx.sHtML

[R48] awk 取指定列
来源：http://wap.sjlbkw.cn/Article/details/gqnjyfaby.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnnrthkk.sHtML

[R49] awk 带条件
来源：http://www.share.yfazqb.com/Article/details/gagqjjfvi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.bbcook.cn/Article/details/gkqchjtzr.sHtML

[R50] awk 求和
来源：http://blog.tarul.cn/Article/details/gssfstvmk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fktsv.cn/Article/details/gnaiawxvn.sHtML

[R51] 排序去重取前几
来源：http://mobile.fktsv.cn/Article/details/ghiicqkjm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.yfazqb.com/Article/details/gqqbuzeks.sHtML

[R52] 统计行数
来源：http://www.m.share.vehdjk.com/Article/details/grneojute.sHtML

wc -l a.txt
来源：http://baike.fktsv.cn/Article/details/glfyhpsya.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.bbcook.cn/Article/details/gvwpyvhvw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.tarul.cn/Article/details/gdmjiltlt.sHtML

[R54] 比较两个文件
来源：http://read.share.epnwcf.com/Article/details/gbqpdjxmv.sHtML

diff a.txt b.txt
来源：http://www.blog.yfazqb.com/Article/details/gfpzscjsz.sHtML

[R55] 压缩与解压
来源：http://www.blog.sjlbkw.cn/Article/details/gkmpycsxh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.epnwcf.com/Article/details/gdxktpghp.sHtML

[R56] 远程拷贝
来源：http://wap.epnwcf.com/Article/details/gjpfzbufv.sHtML

scp file user@host:/path/
来源：http://www.m.share.yfazqb.com/Article/details/gtsbcmrph.sHtML

[R57] 远程执行命令
来源：http://www.share.vehdjk.com/Article/details/gzsnwschh.sHtML

ssh user@host 'uptime'
来源：http://www.blog.vehdjk.com/Article/details/govjuxodw.sHtML

[R58] 下载文件
来源：http://read.share.epnwcf.com/Article/details/glkihuewp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.bbcook.cn/Article/details/gcacjmvme.sHtML

[R59] 发 POST JSON
来源：http://blog.yfazqb.com/Article/details/gvwoblaje.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.tarul.cn/Article/details/gegrentvt.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.sjlbkw.cn/Article/details/ghooqgmdz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.bbcook.cn/Article/details/gropczhja.sHtML

[R61] 磁盘占用
来源：http://www.share.epnwcf.com/Article/details/gjgknrxeb.sHtML

df -h;  du -sh *
来源：http://read.share.yfazqb.com/Article/details/gzjtmmwdm.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.vehdjk.com/Article/details/gvkxyvqsy.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.sjlbkw.cn/Article/details/gwkppoyni.sHtML

[R63] 内存与进程
来源：http://www.blog.fktsv.cn/Article/details/gdjmxoamu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.sjlbkw.cn/Article/details/gsgccekfc.sHtML

[R64] 结束进程
来源：http://3g.epnwcf.com/Article/details/gsyrhvgni.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.bbcook.cn/Article/details/gtytqfnfe.sHtML

[R65] 查看端口占用
来源：http://blog.sjlbkw.cn/Article/details/ghpgatvyk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fktsv.cn/Article/details/gioqtckxq.sHtML

[R66] 定时任务
来源：http://3g.sjlbkw.cn/Article/details/gxncdnsgd.sHtML

crontab -e;  crontab -l
来源：http://3g.yfazqb.com/Article/details/gkukysarf.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.vehdjk.com/Article/details/ghucojknv.sHtML

openssl rand -hex 16
来源：http://m.share.vehdjk.com/Article/details/gqzbvfjrz.sHtML

[R68] 计算文件校验值
来源：http://wap.fktsv.cn/Article/details/gkxysifme.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.bbcook.cn/Article/details/gqqulxquj.sHtML

[R69] 生成随机密码
来源：http://mobile.epnwcf.com/Article/details/gpajlvtsb.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.tarul.cn/Article/details/gukuzavld.sHtML

[R70] 时间戳与互转
来源：http://wap.bbcook.cn/Article/details/gbyqzwzhl.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.vehdjk.com/Article/details/gtsmxnpdq.sHtML

[R71] 日期格式化
来源：http://read.share.epnwcf.com/Article/details/gknyjbrhj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.sjlbkw.cn/Article/details/grbpqrfja.sHtML

[R72] 等待端口就绪
来源：http://www.blog.yfazqb.com/Article/details/gcsehgqwi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.bbcook.cn/Article/details/gazyzeeoi.sHtML

[R73] 分割大日志
来源：http://m.share.sjlbkw.cn/Article/details/gvuiwyaaw.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.bbcook.cn/Article/details/gynsmizfg.sHtML

[R74] 批量重命名
来源：http://www.blog.bbcook.cn/Article/details/gaesmkuqg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.tarul.cn/Article/details/gsjznoibd.sHtML

[R75] 导出环境变量
来源：http://read.share.vehdjk.com/Article/details/gkitwddob.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.sjlbkw.cn/Article/details/ghotgqqbj.sHtML

[R76] 使用临时文件
来源：http://www.m.share.epnwcf.com/Article/details/gbuuluxfk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.bbcook.cn/Article/details/gzoihlxme.sHtML

[R77] 读取用户输入
来源：http://m.share.fktsv.cn/Article/details/gdlubmxvl.sHtML

read -rp "请输入: " ans
来源：http://m.share.sjlbkw.cn/Article/details/gbbpalgir.sHtML

[R78] 交互式菜单
来源：http://wap.yfazqb.com/Article/details/gudftfvpi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.bbcook.cn/Article/details/geausukmv.sHtML

[R79] 解析命令行选项
来源：http://blog.vehdjk.com/Article/details/gnxwuhzsb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.vehdjk.com/Article/details/gosggngxt.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.tarul.cn/Article/details/gopuiyfbq.sHtML

time ./run.sh
来源：http://wap.vehdjk.com/Article/details/glmwmcefu.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gnwosxbik.sHtML

S. C / C++ 专题
来源：http://www.m.share.epnwcf.com/Article/details/gnmnmyjnf.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gtaspvqmf.sHtML

[S01] C：Hello World
来源：http://mobile.yfazqb.com/Article/details/geufoszhr.sHtML

#include <stdio.h>
来源：http://www.share.sjlbkw.cn/Article/details/gtsiovoki.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.sjlbkw.cn/Article/details/gzlextwgq.sHtML

[S02] C：变量与格式化输出
来源：http://baike.yfazqb.com/Article/details/ggtcglufh.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.epnwcf.com/Article/details/gpnlfhsvk.sHtML

[S03] C：读入整数
来源：http://mobile.vehdjk.com/Article/details/grqyyhfwn.sHtML


<!-- 参考信息 -->