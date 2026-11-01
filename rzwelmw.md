代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.vehdjk.com/Article/details/gzgywbrlp.sHtML

[Q26] 计数
来源：http://blog.sjlbkw.cn/Article/details/gngqdiodc.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gwprtnpqo.sHtML

[Q27] 条件计数
来源：http://wap.yfazqb.com/Article/details/giifgubot.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.tarul.cn/Article/details/gnhmcmrml.sHtML

[Q28] 求和与平均
来源：http://read.share.vehdjk.com/Article/details/gxnzypbgw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gctdaddlt.sHtML

[Q29] 最大最小值
来源：http://m.share.epnwcf.com/Article/details/gdxqwlniw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gwnpfsnyh.sHtML

[Q30] 分组统计
来源：http://baike.epnwcf.com/Article/details/gmqsfzzee.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/gqkmdfvko.sHtML

[Q31] 分组后过滤
来源：http://wap.fktsv.cn/Article/details/gvkvsthio.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.bbcook.cn/Article/details/gidshsjuf.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gdyyisqst.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/gdxzkuorg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.sjlbkw.cn/Article/details/geuhirald.sHtML

[Q33] 多列分组
来源：http://baike.bbcook.cn/Article/details/gwingotis.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fktsv.cn/Article/details/gvcgmprjh.sHtML

[Q34] 每组取第一条
来源：http://www.share.fktsv.cn/Article/details/gckgnkvil.sHtML

SELECT * FROM (
来源：http://wap.bbcook.cn/Article/details/gifwensvz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.sjlbkw.cn/Article/details/guuxtdils.sHtML

) t WHERE rn = 1;
来源：http://mobile.vehdjk.com/Article/details/gzalnnrnn.sHtML

[Q35] 内连接
来源：http://read.share.yfazqb.com/Article/details/gdendudrj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/gdgemtrcp.sHtML

[Q36] 左连接
来源：http://m.share.fktsv.cn/Article/details/gxzaqphsn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.tarul.cn/Article/details/gkdtgkgjw.sHtML

[Q37] 右连接
来源：http://www.m.share.vehdjk.com/Article/details/ggnfimcjg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.yfazqb.com/Article/details/gruvohqsa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.vehdjk.com/Article/details/gclurbwye.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fktsv.cn/Article/details/gzlsbzluz.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.bbcook.cn/Article/details/gaimxpdpl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fktsv.cn/Article/details/gyahkktmi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.vehdjk.com/Article/details/gmarviwwo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.sjlbkw.cn/Article/details/gijzfgake.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.yfazqb.com/Article/details/gzryvjwre.sHtML

[Q41] 多表连接
来源：http://mobile.vehdjk.com/Article/details/grmjsinxf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.tarul.cn/Article/details/gleivqhwa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.yfazqb.com/Article/details/gckhbobdv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.sjlbkw.cn/Article/details/gtkyfseuz.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fktsv.cn/Article/details/ghdcsfeun.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.tarul.cn/Article/details/gaqlszjhr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.epnwcf.com/Article/details/grbvrumqx.sHtML

[Q43] 标量子查询
来源：http://baike.bbcook.cn/Article/details/gavtwuvze.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.sjlbkw.cn/Article/details/gnzhnbsvp.sHtML

[Q44] IN 子查询
来源：http://m.share.bbcook.cn/Article/details/gmwwbujuy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fktsv.cn/Article/details/glnkgjkgk.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.epnwcf.com/Article/details/gbyfrtfln.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.sjlbkw.cn/Article/details/glrlqxose.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.yfazqb.com/Article/details/gxckqxojv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.yfazqb.com/Article/details/gequvcrgb.sHtML

[Q47] 与平均值比较
来源：http://read.share.fktsv.cn/Article/details/gvkkewmhs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.epnwcf.com/Article/details/gqnuhhuee.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.yfazqb.com/Article/details/ghfxucltg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.sjlbkw.cn/Article/details/gwbbjzuev.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.bbcook.cn/Article/details/gbygwvzke.sHtML

[Q49] 更新单行
来源：http://www.share.yfazqb.com/Article/details/gzkkxywtz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.vehdjk.com/Article/details/gylmfvsyz.sHtML

[Q50] 批量更新
来源：http://m.share.fktsv.cn/Article/details/gdkjwowbc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.sjlbkw.cn/Article/details/grkfusemy.sHtML

[Q51] 用子查询更新
来源：http://read.share.bbcook.cn/Article/details/gvcfubsdc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.tarul.cn/Article/details/gysmygguv.sHtML

[Q52] 删除指定行
来源：http://www.share.sjlbkw.cn/Article/details/gykxrdyma.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.sjlbkw.cn/Article/details/gmvwumuld.sHtML

[Q53] 按条件删除
来源：http://m.share.yfazqb.com/Article/details/gqfkqgkdr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.tarul.cn/Article/details/goddxpxqu.sHtML

[Q54] 清空表
来源：http://m.share.tarul.cn/Article/details/gzinradpm.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.bbcook.cn/Article/details/glehylody.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.sjlbkw.cn/Article/details/grjchakky.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.yfazqb.com/Article/details/gjavghcul.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.yfazqb.com/Article/details/ggrfirghe.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.tarul.cn/Article/details/gdjofvmjq.sHtML

[Q57] 行号
来源：http://www.m.share.tarul.cn/Article/details/gelxlxihv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gknimixsi.sHtML

[Q58] 累计求和
来源：http://www.share.vehdjk.com/Article/details/gijcvyysp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.tarul.cn/Article/details/gadulaqji.sHtML

[Q59] 分组内累计
来源：http://baike.tarul.cn/Article/details/gmwhjabcb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.bbcook.cn/Article/details/gufdaunhv.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.vehdjk.com/Article/details/gimetlstg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.yfazqb.com/Article/details/gqvbwvgic.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.vehdjk.com/Article/details/ghrbppjjq.sHtML

[Q61] 移动平均
来源：http://www.share.vehdjk.com/Article/details/gihjhjlri.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.bbcook.cn/Article/details/gmdndmqde.sHtML

[Q62] 分组占比
来源：http://mobile.fktsv.cn/Article/details/gnfcvjhrg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gckvbgelv.sHtML

[Q63] 开启事务
来源：http://baike.vehdjk.com/Article/details/grwfvpgrf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fktsv.cn/Article/details/glomnyoja.sHtML

[Q64] 提交事务
来源：http://www.share.epnwcf.com/Article/details/gtjphiekw.sHtML

COMMIT;
来源：http://blog.bbcook.cn/Article/details/gduwyfhby.sHtML

[Q65] 回滚事务
来源：http://www.share.bbcook.cn/Article/details/gduqzuikc.sHtML

ROLLBACK;
来源：http://baike.bbcook.cn/Article/details/gfhowqgcz.sHtML

[Q66] 行锁查询
来源：http://m.share.tarul.cn/Article/details/ghyabezhv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.bbcook.cn/Article/details/ggzeaahnf.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.sjlbkw.cn/Article/details/gpoaifqyb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.bbcook.cn/Article/details/gksuhopiu.sHtML

[Q68] 保存点
来源：http://www.m.share.fktsv.cn/Article/details/gjddiqemi.sHtML

SAVEPOINT sp1;
来源：http://wap.yfazqb.com/Article/details/galhrusah.sHtML

ROLLBACK TO sp1;
来源：http://mobile.sjlbkw.cn/Article/details/gqglumlfg.sHtML

[Q69] 查看执行计划
来源：http://mobile.yfazqb.com/Article/details/gelcfvtck.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.sjlbkw.cn/Article/details/gisibnibf.sHtML

[Q70] 更新统计信息
来源：http://www.blog.sjlbkw.cn/Article/details/ghcqjggbb.sHtML

ANALYZE TABLE users;
来源：http://m.share.tarul.cn/Article/details/gbxzqnfbk.sHtML

[Q71] 查看建表语句
来源：http://mobile.yfazqb.com/Article/details/gnnzphxsc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.tarul.cn/Article/details/gqzsfckvh.sHtML

[Q72] 查看索引
来源：http://baike.bbcook.cn/Article/details/gilkxytkd.sHtML

SHOW INDEX FROM users;
来源：http://3g.bbcook.cn/Article/details/gfxhhrgom.sHtML

[Q73] 查看表状态
来源：http://baike.vehdjk.com/Article/details/gqpewvxtd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.vehdjk.com/Article/details/gtpowxlhx.sHtML

[Q74] 强制使用索引
来源：http://mobile.bbcook.cn/Article/details/ghjdwtxdg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.tarul.cn/Article/details/gjybcgcah.sHtML

[Q75] 日期格式化
来源：http://wap.fktsv.cn/Article/details/gtdncgoba.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.yfazqb.com/Article/details/ggzulwjqg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.vehdjk.com/Article/details/gbrayhlwl.sHtML

[Q76] 按天统计
来源：http://wap.bbcook.cn/Article/details/gfblcuuuh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.sjlbkw.cn/Article/details/gsvxabshd.sHtML

[Q77] 时间加减
来源：http://wap.tarul.cn/Article/details/gcpllixer.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fktsv.cn/Article/details/gotgeghtb.sHtML

[Q78] 当前时间
来源：http://wap.sjlbkw.cn/Article/details/glohshano.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.yfazqb.com/Article/details/gbyabvgka.sHtML

[Q79] 字符串拼接
来源：http://read.share.epnwcf.com/Article/details/gdwpnoxzh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.epnwcf.com/Article/details/gzbqwwnmc.sHtML

[Q80] 字符串截取
来源：http://baike.bbcook.cn/Article/details/gktugeguw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.yfazqb.com/Article/details/gvhhadyjr.sHtML

[Q81] 字符串替换
来源：http://3g.epnwcf.com/Article/details/gsmuwudpt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.yfazqb.com/Article/details/gkuthqifj.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.vehdjk.com/Article/details/glasodsdk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/galnkkecg.sHtML

[Q83] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gqwrhveaa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/gwxscwyrc.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.vehdjk.com/Article/details/gfxzpfmas.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.tarul.cn/Article/details/gvxhnhthk.sHtML

[Q85] 数值取整
来源：http://blog.vehdjk.com/Article/details/ggasfwqxg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.vehdjk.com/Article/details/gekaokbhr.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.epnwcf.com/Article/details/gfpcdrrut.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fktsv.cn/Article/details/ghxtrpqcu.sHtML

[Q87] JSON 字段做条件
来源：http://blog.epnwcf.com/Article/details/gnhvcjyil.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.epnwcf.com/Article/details/gehxiywyi.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.sjlbkw.cn/Article/details/gnwirxivr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.vehdjk.com/Article/details/gkhlxzaiz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.bbcook.cn/Article/details/gbxifcilz.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fktsv.cn/Article/details/gesymiktc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.bbcook.cn/Article/details/gcxylbvij.sHtML

[Q90] 生成序号列
来源：http://3g.epnwcf.com/Article/details/gbpgqeesw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.bbcook.cn/Article/details/giupefvij.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gzpxqsnxu.sHtML

R. Bash 专题
来源：http://wap.sjlbkw.cn/Article/details/guoccjbvu.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gbvpxwksk.sHtML

[R01] shebang 与严格模式
来源：http://baike.vehdjk.com/Article/details/gzkmgmwny.sHtML

#!/usr/bin/env bash
来源：http://blog.sjlbkw.cn/Article/details/ggqnwtmtg.sHtML

set -euo pipefail
来源：http://3g.fktsv.cn/Article/details/gidyjqtrr.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.epnwcf.com/Article/details/gpbpngbhf.sHtML

name="Tom"; echo "$name"
来源：http://baike.fktsv.cn/Article/details/gykoyxcih.sHtML

[R03] 只读变量
来源：http://m.share.sjlbkw.cn/Article/details/gsqtbesvz.sHtML

readonly PI=3.14
来源：http://www.share.fktsv.cn/Article/details/gexprcsaa.sHtML

[R04] 位置参数
来源：http://mobile.epnwcf.com/Article/details/gqamdhzss.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.vehdjk.com/Article/details/gvkgoskle.sHtML

[R05] 参数默认值
来源：http://3g.bbcook.cn/Article/details/gggprqzqh.sHtML

name="${1:-default}"
来源：http://wap.bbcook.cn/Article/details/gyvufsrhv.sHtML

[R06] 判断命令是否存在
来源：http://wap.bbcook.cn/Article/details/grkfuashj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.epnwcf.com/Article/details/gatluhlzp.sHtML

[R07] if 判断文件
来源：http://mobile.epnwcf.com/Article/details/gfehtqfiv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.bbcook.cn/Article/details/gbxdgdziq.sHtML

[R08] 数值比较
来源：http://mobile.vehdjk.com/Article/details/gvraetlth.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gswsphcbg.sHtML

[R09] 字符串比较
来源：http://baike.yfazqb.com/Article/details/gkffersqf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.epnwcf.com/Article/details/gvpcjyvzx.sHtML

[R10] 正则匹配
来源：http://wap.sjlbkw.cn/Article/details/gkdbrsgew.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.epnwcf.com/Article/details/gboauvcmm.sHtML

[R11] case 多分支
来源：http://3g.epnwcf.com/Article/details/gtvwbsyhj.sHtML

case "$1" in
来源：http://blog.fktsv.cn/Article/details/gemisrxhi.sHtML

start) echo "启动" ;;
来源：http://read.share.yfazqb.com/Article/details/gilibgtkq.sHtML

stop)  echo "停止" ;;
来源：http://blog.yfazqb.com/Article/details/giwvejpjq.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.vehdjk.com/Article/details/gxlxzujln.sHtML

esac
来源：http://www.m.share.tarul.cn/Article/details/gjyfcfmpi.sHtML

[R12] for 遍历文件
来源：http://www.share.yfazqb.com/Article/details/ghrxgkdio.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.tarul.cn/Article/details/gtsnfvrjd.sHtML

[R13] for 计数循环
来源：http://baike.bbcook.cn/Article/details/gqjivxdlh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/gfqzsgusv.sHtML

[R14] C 风格 for
来源：http://www.share.yfazqb.com/Article/details/ghabgtcgj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/gklvtacse.sHtML

[R15] while 逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gmvoqpnlp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.vehdjk.com/Article/details/gbgycuvcm.sHtML

[R16] until 等待条件
来源：http://baike.vehdjk.com/Article/details/gqctbcxpl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/gzpjhvacy.sHtML

[R17] 数组定义与取值
来源：http://read.share.tarul.cn/Article/details/gqmzftwof.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fktsv.cn/Article/details/gplyvejyc.sHtML

[R18] 遍历数组
来源：http://www.share.bbcook.cn/Article/details/gybqhljpe.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.sjlbkw.cn/Article/details/gafldjzym.sHtML

[R19] 数组长度
来源：http://blog.fktsv.cn/Article/details/gbpdwdzqj.sHtML

echo "${#arr[@]}"
来源：http://www.blog.tarul.cn/Article/details/gqcmdvcyh.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.epnwcf.com/Article/details/gtjkoeutg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gzufxovxi.sHtML

[R21] 字符串长度
来源：http://3g.bbcook.cn/Article/details/goqwrjhvm.sHtML

echo "${#s}"
来源：http://www.blog.epnwcf.com/Article/details/grjbmbqef.sHtML

[R22] 截取子串
来源：http://blog.fktsv.cn/Article/details/geoirzmrk.sHtML

echo "${s:0:5}"
来源：http://read.share.fktsv.cn/Article/details/ghhyfuicc.sHtML

[R23] 字符串替换
来源：http://3g.yfazqb.com/Article/details/ggmfbzdbm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.yfazqb.com/Article/details/guwmstuqq.sHtML

[R24] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gghjyzjkc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fktsv.cn/Article/details/ggwkyiqer.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.epnwcf.com/Article/details/gqoqzukxa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fktsv.cn/Article/details/geroakqzt.sHtML

[R26] 命令替换
来源：http://mobile.sjlbkw.cn/Article/details/gsnqvfnqw.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.epnwcf.com/Article/details/goflgobvm.sHtML

[R27] 算术展开
来源：http://www.blog.vehdjk.com/Article/details/gagctqpwh.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.vehdjk.com/Article/details/gkqdodyvq.sHtML

[R28] 浮点运算
来源：http://wap.bbcook.cn/Article/details/gtbungqdw.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.tarul.cn/Article/details/gsfstfsvl.sHtML

[R29] 定义函数
来源：http://www.blog.epnwcf.com/Article/details/gwyfszxbw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.sjlbkw.cn/Article/details/gwixfaysl.sHtML

[R30] 函数返回状态码
来源：http://m.share.tarul.cn/Article/details/garwxpmjg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fktsv.cn/Article/details/gbruiqgip.sHtML

[R31] 局部变量
来源：http://wap.sjlbkw.cn/Article/details/gejulhrzg.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.sjlbkw.cn/Article/details/gvirghcnw.sHtML

[R32] 参数个数校验
来源：http://3g.sjlbkw.cn/Article/details/gniudaztj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.yfazqb.com/Article/details/guzpzywkk.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.epnwcf.com/Article/details/gdzpnrhvq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.tarul.cn/Article/details/gtndmxebn.sHtML

[R34] 退出时清理
来源：http://wap.vehdjk.com/Article/details/ghnrpmjod.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gkrillusf.sHtML

[R35] 后台执行并等待
来源：http://mobile.vehdjk.com/Article/details/gqxmozoae.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.epnwcf.com/Article/details/ggkokjziz.sHtML

[R36] 并发执行多个任务
来源：http://read.share.vehdjk.com/Article/details/gwydzcjyd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.yfazqb.com/Article/details/gghlkhdek.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.epnwcf.com/Article/details/gpzfwxkzg.sHtML

files=$(ls -1)
来源：http://baike.epnwcf.com/Article/details/glmgddnlu.sHtML

[R38] 管道串联
来源：http://www.share.epnwcf.com/Article/details/gbqemcvnq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.bbcook.cn/Article/details/gbsjtxmsx.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.epnwcf.com/Article/details/gdzeclbbn.sHtML

cmd > out.log 2>&1
来源：http://baike.tarul.cn/Article/details/glgjvcnau.sHtML

[R40] 追加写日志
来源：http://mobile.fktsv.cn/Article/details/gzmakuyoa.sHtML

echo "log" >> out.log
来源：http://www.share.sjlbkw.cn/Article/details/gmqldljyb.sHtML

[R41] 丢弃输出
来源：http://mobile.yfazqb.com/Article/details/gtfexjpdf.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fktsv.cn/Article/details/gwukslfcz.sHtML

[R42] 输入重定向
来源：http://m.share.sjlbkw.cn/Article/details/glgzxkaum.sHtML

wc -l < a.txt
来源：http://read.share.bbcook.cn/Article/details/gxysyaomn.sHtML

[R43] 按名字查找文件
来源：http://blog.fktsv.cn/Article/details/gcxnfjfky.sHtML

find . -name "*.log" -type f
来源：http://wap.vehdjk.com/Article/details/gwykixhar.sHtML

[R44] 按修改时间查找
来源：http://mobile.fktsv.cn/Article/details/guuljbsav.sHtML

find . -mtime -7 -type f
来源：http://read.share.vehdjk.com/Article/details/gwkqtswbz.sHtML

[R45] 批量删除
来源：http://wap.yfazqb.com/Article/details/gjdobcgke.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.vehdjk.com/Article/details/gskpxqptv.sHtML

[R46] 递归替换文件内容
来源：http://baike.fktsv.cn/Article/details/gjrfpbbbi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.vehdjk.com/Article/details/gmazfyxqo.sHtML

[R47] sed 单行替换
来源：http://wap.sjlbkw.cn/Article/details/gondcgogu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.epnwcf.com/Article/details/grfmmdoiu.sHtML

[R48] awk 取指定列
来源：http://baike.yfazqb.com/Article/details/gsfsxzumk.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.sjlbkw.cn/Article/details/ghfvwvvyp.sHtML

[R49] awk 带条件
来源：http://www.blog.yfazqb.com/Article/details/gawonyizo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.sjlbkw.cn/Article/details/grayzyjbc.sHtML

[R50] awk 求和
来源：http://blog.vehdjk.com/Article/details/gcmbgfpyp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.epnwcf.com/Article/details/gefvpttey.sHtML

[R51] 排序去重取前几
来源：http://3g.fktsv.cn/Article/details/gufpguqpd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fktsv.cn/Article/details/golpyegdk.sHtML

[R52] 统计行数
来源：http://baike.fktsv.cn/Article/details/gxuggbefy.sHtML

wc -l a.txt
来源：http://baike.fktsv.cn/Article/details/gbxxvbeld.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fktsv.cn/Article/details/gyaqrrgkc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fktsv.cn/Article/details/gsrnrluwi.sHtML

[R54] 比较两个文件
来源：http://m.share.vehdjk.com/Article/details/gtdvojoup.sHtML

diff a.txt b.txt
来源：http://wap.bbcook.cn/Article/details/goaerfztz.sHtML

[R55] 压缩与解压
来源：http://3g.vehdjk.com/Article/details/gzoisdoce.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.bbcook.cn/Article/details/golgqvldp.sHtML

[R56] 远程拷贝
来源：http://www.m.share.yfazqb.com/Article/details/gudbrootw.sHtML

scp file user@host:/path/
来源：http://3g.yfazqb.com/Article/details/gkzdgmcak.sHtML

[R57] 远程执行命令
来源：http://www.blog.epnwcf.com/Article/details/grgqxadzp.sHtML

ssh user@host 'uptime'
来源：http://blog.epnwcf.com/Article/details/gxpumcppe.sHtML

[R58] 下载文件
来源：http://mobile.tarul.cn/Article/details/gytgltuie.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.sjlbkw.cn/Article/details/ggocglkxi.sHtML

[R59] 发 POST JSON
来源：http://3g.epnwcf.com/Article/details/gnhibjzae.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.vehdjk.com/Article/details/giatoqrsd.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.tarul.cn/Article/details/gykcmzbqb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fktsv.cn/Article/details/ghzbcjqbv.sHtML

[R61] 磁盘占用
来源：http://baike.epnwcf.com/Article/details/gnnhcmrvp.sHtML

df -h;  du -sh *
来源：http://www.m.share.epnwcf.com/Article/details/gdckwusfj.sHtML

[R62] 找最占空间的文件
来源：http://www.share.tarul.cn/Article/details/gfxwuzskh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.bbcook.cn/Article/details/gxplmsatf.sHtML

[R63] 内存与进程
来源：http://blog.vehdjk.com/Article/details/gkauaudjf.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.yfazqb.com/Article/details/gowyicvrt.sHtML

[R64] 结束进程
来源：http://blog.tarul.cn/Article/details/ghskqkebr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.sjlbkw.cn/Article/details/gkebuiujs.sHtML

[R65] 查看端口占用
来源：http://read.share.tarul.cn/Article/details/gzhsratfd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fktsv.cn/Article/details/gmvwktwlz.sHtML

[R66] 定时任务
来源：http://blog.sjlbkw.cn/Article/details/gkodlnzue.sHtML

crontab -e;  crontab -l
来源：http://m.share.yfazqb.com/Article/details/gvcmlhuwd.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.bbcook.cn/Article/details/gxxekikyc.sHtML

openssl rand -hex 16
来源：http://3g.bbcook.cn/Article/details/gtqzygolr.sHtML

[R68] 计算文件校验值
来源：http://m.share.sjlbkw.cn/Article/details/gjmioeehx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.tarul.cn/Article/details/gztteekma.sHtML

[R69] 生成随机密码
来源：http://www.m.share.bbcook.cn/Article/details/gygcdknwx.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.yfazqb.com/Article/details/gksmsiaav.sHtML

[R70] 时间戳与互转
来源：http://blog.sjlbkw.cn/Article/details/gcijiavij.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.yfazqb.com/Article/details/ghyeaqcaf.sHtML

[R71] 日期格式化
来源：http://www.share.yfazqb.com/Article/details/gkqcggaru.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.epnwcf.com/Article/details/gdnpjwqjl.sHtML

[R72] 等待端口就绪
来源：http://blog.fktsv.cn/Article/details/gwahxnqxw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fktsv.cn/Article/details/gpebelqgy.sHtML

[R73] 分割大日志
来源：http://mobile.sjlbkw.cn/Article/details/gbkyvpfvz.sHtML

split -l 1000 big.log part_
来源：http://wap.epnwcf.com/Article/details/gxulelcra.sHtML

[R74] 批量重命名
来源：http://read.share.yfazqb.com/Article/details/ggwqbhuhv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fktsv.cn/Article/details/gjxshlcvz.sHtML

[R75] 导出环境变量
来源：http://wap.epnwcf.com/Article/details/gqigzwlsf.sHtML


<!-- 参考信息 -->