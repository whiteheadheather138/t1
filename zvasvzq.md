代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.tarul.cn/Article/details/gdtzbhmhm.sHtML

[Q20] IN 列表
来源：http://www.m.share.fktsv.cn/Article/details/guhtqmdgz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.vehdjk.com/Article/details/gkvsfcade.sHtML

[Q21] 空值判断
来源：http://wap.yfazqb.com/Article/details/grecygtbq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.epnwcf.com/Article/details/grglohwfw.sHtML

[Q22] 排序
来源：http://wap.tarul.cn/Article/details/gsgftncem.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.yfazqb.com/Article/details/gdcjccyfo.sHtML

[Q23] 分页
来源：http://www.share.epnwcf.com/Article/details/gjdfwqxot.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.bbcook.cn/Article/details/gbtqxolhu.sHtML

[Q24] 去重
来源：http://www.blog.yfazqb.com/Article/details/gljrqzfbb.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gfpkgtwbc.sHtML

[Q25] 只取前 N 条
来源：http://m.share.tarul.cn/Article/details/gwgsodefp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fktsv.cn/Article/details/gtwplsdcw.sHtML

[Q26] 计数
来源：http://3g.fktsv.cn/Article/details/gsslbesyx.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gruynotwe.sHtML

[Q27] 条件计数
来源：http://baike.yfazqb.com/Article/details/groswqlqv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.sjlbkw.cn/Article/details/grgoqktjw.sHtML

[Q28] 求和与平均
来源：http://read.share.bbcook.cn/Article/details/grakwdlsb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.yfazqb.com/Article/details/ggnikwgef.sHtML

[Q29] 最大最小值
来源：http://www.blog.vehdjk.com/Article/details/ghohgdjws.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gmidqhcjg.sHtML

[Q30] 分组统计
来源：http://www.share.yfazqb.com/Article/details/gtzjyhmgf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.sjlbkw.cn/Article/details/glunpxfay.sHtML

[Q31] 分组后过滤
来源：http://baike.vehdjk.com/Article/details/gateanryb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.sjlbkw.cn/Article/details/gbnjesohx.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gteggwmuc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gnwdnfzvh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.yfazqb.com/Article/details/gknfpxdjq.sHtML

[Q33] 多列分组
来源：http://mobile.vehdjk.com/Article/details/gcgnhtmlt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.yfazqb.com/Article/details/guterrdcr.sHtML

[Q34] 每组取第一条
来源：http://3g.vehdjk.com/Article/details/gphoarumb.sHtML

SELECT * FROM (
来源：http://read.share.epnwcf.com/Article/details/gqrvtvrvn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.epnwcf.com/Article/details/griqxhuxs.sHtML

) t WHERE rn = 1;
来源：http://blog.tarul.cn/Article/details/gfvygvwlz.sHtML

[Q35] 内连接
来源：http://m.share.epnwcf.com/Article/details/ghksndxki.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.bbcook.cn/Article/details/gtunrtqgg.sHtML

[Q36] 左连接
来源：http://baike.bbcook.cn/Article/details/gkenatxnf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/ghllzhrmg.sHtML

[Q37] 右连接
来源：http://wap.yfazqb.com/Article/details/gnjsgjmmz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.yfazqb.com/Article/details/gfccxkpjd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.yfazqb.com/Article/details/gqygituvp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fktsv.cn/Article/details/govqeyihb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.sjlbkw.cn/Article/details/gzvbqgjkn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.bbcook.cn/Article/details/ggeympvbp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.vehdjk.com/Article/details/ghpvijynv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.bbcook.cn/Article/details/gsuvkrbgk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.yfazqb.com/Article/details/ginquukme.sHtML

[Q41] 多表连接
来源：http://m.share.epnwcf.com/Article/details/gasiqljko.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.epnwcf.com/Article/details/gliwmzkqg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.vehdjk.com/Article/details/gkmenzvou.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.tarul.cn/Article/details/grhanajxg.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.bbcook.cn/Article/details/gmafdgqhq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fktsv.cn/Article/details/gjmuidvui.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.vehdjk.com/Article/details/gqxvojizy.sHtML

[Q43] 标量子查询
来源：http://www.share.tarul.cn/Article/details/gpqwtgbak.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fktsv.cn/Article/details/gykdtdsnd.sHtML

[Q44] IN 子查询
来源：http://read.share.vehdjk.com/Article/details/gcfflqrsb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.yfazqb.com/Article/details/gwhpevlxl.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.bbcook.cn/Article/details/gcynhhjog.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.sjlbkw.cn/Article/details/gefhhalyv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.yfazqb.com/Article/details/gnhbrijin.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.sjlbkw.cn/Article/details/guytgiwsz.sHtML

[Q47] 与平均值比较
来源：http://wap.tarul.cn/Article/details/gnwvgnajx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.vehdjk.com/Article/details/ghatgczsz.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.vehdjk.com/Article/details/gzkwzpsxp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.bbcook.cn/Article/details/gkzxfkrlz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.tarul.cn/Article/details/gfeazrdif.sHtML

[Q49] 更新单行
来源：http://read.share.epnwcf.com/Article/details/gnrspkzqy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.yfazqb.com/Article/details/gkyikxklq.sHtML

[Q50] 批量更新
来源：http://blog.bbcook.cn/Article/details/gwghpfeop.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.vehdjk.com/Article/details/gksdtjtbe.sHtML

[Q51] 用子查询更新
来源：http://www.share.sjlbkw.cn/Article/details/gyildyfol.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.vehdjk.com/Article/details/gsvujydhy.sHtML

[Q52] 删除指定行
来源：http://m.share.tarul.cn/Article/details/glbpueoac.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fktsv.cn/Article/details/gyzubwzfb.sHtML

[Q53] 按条件删除
来源：http://blog.vehdjk.com/Article/details/gtbytttnd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fktsv.cn/Article/details/gwabartua.sHtML

[Q54] 清空表
来源：http://wap.yfazqb.com/Article/details/gjpimhplj.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fktsv.cn/Article/details/ghubzoudh.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.sjlbkw.cn/Article/details/gtxnpzryd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.epnwcf.com/Article/details/gyqhagoho.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.vehdjk.com/Article/details/glmjtmbvw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.epnwcf.com/Article/details/gzfahjzak.sHtML

[Q57] 行号
来源：http://www.m.share.vehdjk.com/Article/details/gqejjobjv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gqbbymdmu.sHtML

[Q58] 累计求和
来源：http://www.blog.fktsv.cn/Article/details/gpmpprdeb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gqyrgelpe.sHtML

[Q59] 分组内累计
来源：http://blog.fktsv.cn/Article/details/gydhxshwx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gbteaoifc.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.bbcook.cn/Article/details/gwumnzidv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.tarul.cn/Article/details/gguehfyfm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gypaqdlpi.sHtML

[Q61] 移动平均
来源：http://blog.yfazqb.com/Article/details/gbtzgxfhl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.yfazqb.com/Article/details/gfeposdxn.sHtML

[Q62] 分组占比
来源：http://www.share.yfazqb.com/Article/details/gkpidkpyj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/guohhocpb.sHtML

[Q63] 开启事务
来源：http://mobile.vehdjk.com/Article/details/geiyoceiu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.epnwcf.com/Article/details/ggbzaunwt.sHtML

[Q64] 提交事务
来源：http://baike.epnwcf.com/Article/details/gbsdlfuhh.sHtML

COMMIT;
来源：http://www.blog.bbcook.cn/Article/details/ggvgowuhr.sHtML

[Q65] 回滚事务
来源：http://www.blog.yfazqb.com/Article/details/gxsdhvypw.sHtML

ROLLBACK;
来源：http://www.share.yfazqb.com/Article/details/gmfyknmri.sHtML

[Q66] 行锁查询
来源：http://read.share.vehdjk.com/Article/details/glhwrwqvi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.sjlbkw.cn/Article/details/geiapsxgs.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.sjlbkw.cn/Article/details/gogjtmjvf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.vehdjk.com/Article/details/gfxatrcfs.sHtML

[Q68] 保存点
来源：http://3g.yfazqb.com/Article/details/gljgxtmew.sHtML

SAVEPOINT sp1;
来源：http://m.share.yfazqb.com/Article/details/guceaalms.sHtML

ROLLBACK TO sp1;
来源：http://baike.tarul.cn/Article/details/glgzlxhag.sHtML

[Q69] 查看执行计划
来源：http://mobile.tarul.cn/Article/details/gkiegalpa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.yfazqb.com/Article/details/gtzzwilho.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fktsv.cn/Article/details/gdnurxzke.sHtML

ANALYZE TABLE users;
来源：http://m.share.fktsv.cn/Article/details/gtmxhevfz.sHtML

[Q71] 查看建表语句
来源：http://3g.epnwcf.com/Article/details/gadgtyjof.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.epnwcf.com/Article/details/gpewfohpb.sHtML

[Q72] 查看索引
来源：http://baike.epnwcf.com/Article/details/guzdsjwgz.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjpgebtd.sHtML

[Q73] 查看表状态
来源：http://m.share.fktsv.cn/Article/details/gduhdaekr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.tarul.cn/Article/details/gdmqszzny.sHtML

[Q74] 强制使用索引
来源：http://3g.yfazqb.com/Article/details/gciphbnli.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.tarul.cn/Article/details/guwdphxyl.sHtML

[Q75] 日期格式化
来源：http://wap.fktsv.cn/Article/details/gshkaiiyg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fktsv.cn/Article/details/ggldnysli.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.yfazqb.com/Article/details/gcythbolf.sHtML

[Q76] 按天统计
来源：http://baike.yfazqb.com/Article/details/gfzcgwinp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.bbcook.cn/Article/details/gmbnovbpo.sHtML

[Q77] 时间加减
来源：http://www.m.share.vehdjk.com/Article/details/gihaodqao.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.epnwcf.com/Article/details/gswsicvjc.sHtML

[Q78] 当前时间
来源：http://m.share.epnwcf.com/Article/details/gshlbcurf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.epnwcf.com/Article/details/gmjyqzixv.sHtML

[Q79] 字符串拼接
来源：http://baike.yfazqb.com/Article/details/ganqfydpu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fktsv.cn/Article/details/gmogveqeb.sHtML

[Q80] 字符串截取
来源：http://baike.vehdjk.com/Article/details/gttaqlkxo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fktsv.cn/Article/details/gzbybojtr.sHtML

[Q81] 字符串替换
来源：http://read.share.epnwcf.com/Article/details/ghgyguuec.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gqjoxbnzo.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.vehdjk.com/Article/details/gmswdzxnh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/gbkamnnuu.sHtML

[Q83] 大小写转换
来源：http://mobile.vehdjk.com/Article/details/gdaezivqy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gwazssbcp.sHtML

[Q84] 去除首尾空格
来源：http://baike.yfazqb.com/Article/details/golluefxr.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/goduoihqe.sHtML

[Q85] 数值取整
来源：http://3g.vehdjk.com/Article/details/geakolomj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.yfazqb.com/Article/details/gycfdloti.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.epnwcf.com/Article/details/gaqohaoga.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.epnwcf.com/Article/details/gzbkhrljb.sHtML

[Q87] JSON 字段做条件
来源：http://baike.vehdjk.com/Article/details/gfbrmtdhl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.tarul.cn/Article/details/giqegkuot.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fktsv.cn/Article/details/gqipelbnn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fktsv.cn/Article/details/gzpdrqeax.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.yfazqb.com/Article/details/gqlyenenq.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.bbcook.cn/Article/details/ghyzmrqgy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.sjlbkw.cn/Article/details/gviebtshw.sHtML

[Q90] 生成序号列
来源：http://www.blog.bbcook.cn/Article/details/gkvblkiox.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.epnwcf.com/Article/details/gwrtgouzi.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/grrnomhte.sHtML

R. Bash 专题
来源：http://wap.sjlbkw.cn/Article/details/gvgiviqiy.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ggqvaxlsh.sHtML

[R01] shebang 与严格模式
来源：http://baike.epnwcf.com/Article/details/gxmgkehhc.sHtML

#!/usr/bin/env bash
来源：http://mobile.bbcook.cn/Article/details/gnkbhbqda.sHtML

set -euo pipefail
来源：http://wap.sjlbkw.cn/Article/details/gjosexgqw.sHtML

[R02] 变量赋值与使用
来源：http://www.share.epnwcf.com/Article/details/gateibdka.sHtML

name="Tom"; echo "$name"
来源：http://mobile.vehdjk.com/Article/details/ggfxxzyeb.sHtML

[R03] 只读变量
来源：http://blog.tarul.cn/Article/details/goctafdko.sHtML

readonly PI=3.14
来源：http://m.share.sjlbkw.cn/Article/details/gtoikkabo.sHtML

[R04] 位置参数
来源：http://wap.tarul.cn/Article/details/gihmtauaq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.sjlbkw.cn/Article/details/gaintubaz.sHtML

[R05] 参数默认值
来源：http://m.share.epnwcf.com/Article/details/gjxpttopy.sHtML

name="${1:-default}"
来源：http://m.share.sjlbkw.cn/Article/details/gulzpskmq.sHtML

[R06] 判断命令是否存在
来源：http://baike.bbcook.cn/Article/details/ghumezlcd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.yfazqb.com/Article/details/gyvfjumww.sHtML

[R07] if 判断文件
来源：http://www.blog.fktsv.cn/Article/details/gcnczgucf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.epnwcf.com/Article/details/gbppfmoky.sHtML

[R08] 数值比较
来源：http://blog.tarul.cn/Article/details/gpghehwgf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.vehdjk.com/Article/details/grzzrxici.sHtML

[R09] 字符串比较
来源：http://www.share.epnwcf.com/Article/details/gvpcyubvg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gtxbmzzpu.sHtML

[R10] 正则匹配
来源：http://wap.yfazqb.com/Article/details/gyfkmzcbo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.epnwcf.com/Article/details/gucpmhxyh.sHtML

[R11] case 多分支
来源：http://mobile.bbcook.cn/Article/details/gxkmmhcrd.sHtML

case "$1" in
来源：http://m.share.sjlbkw.cn/Article/details/gllhpbzyw.sHtML

start) echo "启动" ;;
来源：http://m.share.fktsv.cn/Article/details/gwkqdtnmc.sHtML

stop)  echo "停止" ;;
来源：http://blog.vehdjk.com/Article/details/gqsmxannn.sHtML

*)     echo "未知命令" ;;
来源：http://baike.vehdjk.com/Article/details/gauynqviy.sHtML

esac
来源：http://read.share.tarul.cn/Article/details/gsasgkaib.sHtML

[R12] for 遍历文件
来源：http://read.share.epnwcf.com/Article/details/gropyzcem.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.bbcook.cn/Article/details/gsjlprivj.sHtML

[R13] for 计数循环
来源：http://read.share.sjlbkw.cn/Article/details/gyukehvri.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fktsv.cn/Article/details/ghdyfkehi.sHtML

[R14] C 风格 for
来源：http://read.share.vehdjk.com/Article/details/ggxemyeuy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fktsv.cn/Article/details/gznyplnth.sHtML

[R15] while 逐行读文件
来源：http://3g.vehdjk.com/Article/details/gtzdfusfg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlgoiwtd.sHtML

[R16] until 等待条件
来源：http://blog.epnwcf.com/Article/details/gqtckjhqy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.sjlbkw.cn/Article/details/gipmvfyhc.sHtML

[R17] 数组定义与取值
来源：http://m.share.epnwcf.com/Article/details/gjtpuhgwp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.yfazqb.com/Article/details/gnpifgtpd.sHtML

[R18] 遍历数组
来源：http://www.m.share.tarul.cn/Article/details/ghbgrbdep.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.sjlbkw.cn/Article/details/gzvnweffo.sHtML

[R19] 数组长度
来源：http://baike.epnwcf.com/Article/details/gfnuexatn.sHtML

echo "${#arr[@]}"
来源：http://m.share.epnwcf.com/Article/details/gmltfenaz.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fktsv.cn/Article/details/glnvinymk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.tarul.cn/Article/details/gmqxjtluy.sHtML

[R21] 字符串长度
来源：http://m.share.bbcook.cn/Article/details/gmxqtelal.sHtML

echo "${#s}"
来源：http://wap.epnwcf.com/Article/details/ghpdtchzn.sHtML

[R22] 截取子串
来源：http://wap.tarul.cn/Article/details/gakfnzofb.sHtML

echo "${s:0:5}"
来源：http://3g.tarul.cn/Article/details/gbweabffg.sHtML

[R23] 字符串替换
来源：http://blog.tarul.cn/Article/details/gbxdeetzj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.epnwcf.com/Article/details/gctczpize.sHtML

[R24] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/gnnbpsjha.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.tarul.cn/Article/details/gxzcvjvpb.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.sjlbkw.cn/Article/details/gcqcmwedd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.vehdjk.com/Article/details/gebfsjknf.sHtML

[R26] 命令替换
来源：http://www.blog.bbcook.cn/Article/details/gmptqjvwg.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.bbcook.cn/Article/details/ghmtaxqzu.sHtML

[R27] 算术展开
来源：http://mobile.vehdjk.com/Article/details/gmqhxemjt.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.sjlbkw.cn/Article/details/gnwqzkogt.sHtML

[R28] 浮点运算
来源：http://blog.vehdjk.com/Article/details/gerxcczau.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fktsv.cn/Article/details/gkmwrenns.sHtML

[R29] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/gyrsijjpq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.tarul.cn/Article/details/gyrryrlvk.sHtML

[R30] 函数返回状态码
来源：http://baike.sjlbkw.cn/Article/details/gcswuurqo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.vehdjk.com/Article/details/gxbufwxqe.sHtML

[R31] 局部变量
来源：http://www.blog.tarul.cn/Article/details/gbcvanqgb.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fktsv.cn/Article/details/giwawgyrq.sHtML

[R32] 参数个数校验
来源：http://www.m.share.yfazqb.com/Article/details/gzvoazztm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fktsv.cn/Article/details/gqchmsgaa.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.bbcook.cn/Article/details/gpsozehap.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.tarul.cn/Article/details/gxnmroevs.sHtML

[R34] 退出时清理
来源：http://blog.bbcook.cn/Article/details/gxbykabkx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.tarul.cn/Article/details/ggbnpjwla.sHtML

[R35] 后台执行并等待
来源：http://www.blog.yfazqb.com/Article/details/gwdvbsukt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.tarul.cn/Article/details/gjsktyszq.sHtML

[R36] 并发执行多个任务
来源：http://blog.tarul.cn/Article/details/gowkxscdh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.bbcook.cn/Article/details/gfkgvdmgb.sHtML

[R37] 把输出赋给变量
来源：http://3g.bbcook.cn/Article/details/gntjspuzx.sHtML

files=$(ls -1)
来源：http://www.share.yfazqb.com/Article/details/gnnwqvhzv.sHtML

[R38] 管道串联
来源：http://wap.tarul.cn/Article/details/ggjsxvygq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.epnwcf.com/Article/details/gjbfmzyzb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.tarul.cn/Article/details/gyftnoszn.sHtML

cmd > out.log 2>&1
来源：http://baike.tarul.cn/Article/details/gxbcfgrjj.sHtML

[R40] 追加写日志
来源：http://blog.sjlbkw.cn/Article/details/gpnnnkvrp.sHtML

echo "log" >> out.log
来源：http://read.share.yfazqb.com/Article/details/ghjktywod.sHtML

[R41] 丢弃输出
来源：http://read.share.tarul.cn/Article/details/ghpnibsrp.sHtML

cmd >/dev/null 2>&1
来源：http://baike.yfazqb.com/Article/details/guqeogzpj.sHtML

[R42] 输入重定向
来源：http://www.blog.vehdjk.com/Article/details/ghbcgnmxj.sHtML

wc -l < a.txt
来源：http://mobile.tarul.cn/Article/details/gocrguuhe.sHtML

[R43] 按名字查找文件
来源：http://mobile.tarul.cn/Article/details/gyrxtrdvc.sHtML

find . -name "*.log" -type f
来源：http://www.blog.sjlbkw.cn/Article/details/gowltwqip.sHtML

[R44] 按修改时间查找
来源：http://www.share.bbcook.cn/Article/details/grhpklgtj.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwvrgajd.sHtML

[R45] 批量删除
来源：http://mobile.tarul.cn/Article/details/gjuwmmsdc.sHtML

find . -name "*.tmp" -delete
来源：http://baike.sjlbkw.cn/Article/details/gytdfmvdu.sHtML

[R46] 递归替换文件内容
来源：http://3g.tarul.cn/Article/details/gvlbwxkwi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.vehdjk.com/Article/details/gvxtimbis.sHtML

[R47] sed 单行替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpahufcs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.tarul.cn/Article/details/gekckufij.sHtML

[R48] awk 取指定列
来源：http://wap.sjlbkw.cn/Article/details/gkgewjjcq.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fktsv.cn/Article/details/gqiuoeseu.sHtML

[R49] awk 带条件
来源：http://read.share.epnwcf.com/Article/details/grdvbfuro.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.bbcook.cn/Article/details/gkpnxyscz.sHtML

[R50] awk 求和
来源：http://baike.tarul.cn/Article/details/gtrjbpjrz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gdkzssqeg.sHtML

[R51] 排序去重取前几
来源：http://m.share.vehdjk.com/Article/details/gffuompqc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.yfazqb.com/Article/details/gxbglhpzz.sHtML

[R52] 统计行数
来源：http://baike.fktsv.cn/Article/details/govkaqsxh.sHtML

wc -l a.txt
来源：http://wap.fktsv.cn/Article/details/gttmjqivu.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.bbcook.cn/Article/details/gkjsagxuw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.sjlbkw.cn/Article/details/glsugeuza.sHtML

[R54] 比较两个文件
来源：http://baike.tarul.cn/Article/details/glrqibxcm.sHtML

diff a.txt b.txt
来源：http://blog.epnwcf.com/Article/details/gdluorcio.sHtML

[R55] 压缩与解压
来源：http://blog.fktsv.cn/Article/details/gsoghxiiq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.yfazqb.com/Article/details/gtgjnkszu.sHtML

[R56] 远程拷贝
来源：http://read.share.yfazqb.com/Article/details/gqtirnzqf.sHtML

scp file user@host:/path/
来源：http://www.share.bbcook.cn/Article/details/gabaeqxgt.sHtML

[R57] 远程执行命令
来源：http://baike.sjlbkw.cn/Article/details/gibqdhujx.sHtML

ssh user@host 'uptime'
来源：http://wap.yfazqb.com/Article/details/gggeeyohq.sHtML

[R58] 下载文件
来源：http://blog.vehdjk.com/Article/details/gzipbnifu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.bbcook.cn/Article/details/gdlpprska.sHtML

[R59] 发 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gnxqlzcep.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.yfazqb.com/Article/details/gkuyyzlmn.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.tarul.cn/Article/details/gbtltvliw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fktsv.cn/Article/details/gzkelnior.sHtML

[R61] 磁盘占用
来源：http://blog.bbcook.cn/Article/details/glyjiuwav.sHtML

df -h;  du -sh *
来源：http://baike.sjlbkw.cn/Article/details/gqnhrrcgm.sHtML

[R62] 找最占空间的文件
来源：http://blog.yfazqb.com/Article/details/gxdsfglrj.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.epnwcf.com/Article/details/gdlhewdpz.sHtML

[R63] 内存与进程
来源：http://www.blog.vehdjk.com/Article/details/gbojzbvuw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.bbcook.cn/Article/details/gmandlsyq.sHtML

[R64] 结束进程
来源：http://read.share.tarul.cn/Article/details/gnbtsyaya.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.epnwcf.com/Article/details/gcsxssqbz.sHtML

[R65] 查看端口占用
来源：http://blog.bbcook.cn/Article/details/gtnurgnni.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.vehdjk.com/Article/details/gvxsnobeb.sHtML

[R66] 定时任务
来源：http://www.blog.vehdjk.com/Article/details/grbvsrwux.sHtML

crontab -e;  crontab -l
来源：http://wap.sjlbkw.cn/Article/details/guqailfbl.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.sjlbkw.cn/Article/details/ghfzejjqt.sHtML

openssl rand -hex 16
来源：http://blog.epnwcf.com/Article/details/ggcqfkrfw.sHtML

[R68] 计算文件校验值
来源：http://m.share.fktsv.cn/Article/details/gkswwibpe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fktsv.cn/Article/details/gwovyrwxh.sHtML

[R69] 生成随机密码
来源：http://read.share.vehdjk.com/Article/details/gukcwgrga.sHtML


<!-- 参考信息 -->