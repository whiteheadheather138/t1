代发 wailian999

SELECT * FROM users;
来源：http://baike.epnwcf.com/Article/details/glacmtgqt.sHtML

[Q16] 查询指定列
来源：http://mobile.vehdjk.com/Article/details/gepatyjvu.sHtML

SELECT id, name FROM users;
来源：http://blog.bbcook.cn/Article/details/glgpdvyhy.sHtML

[Q17] 条件查询
来源：http://3g.epnwcf.com/Article/details/gssbacmrm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gleoaeamf.sHtML

[Q18] 模糊匹配
来源：http://baike.vehdjk.com/Article/details/gzhysiveb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.epnwcf.com/Article/details/ggxedsyhy.sHtML

[Q19] 范围查询
来源：http://read.share.sjlbkw.cn/Article/details/gzeeysdzu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fktsv.cn/Article/details/gasjnlyip.sHtML

[Q20] IN 列表
来源：http://m.share.sjlbkw.cn/Article/details/gyjlawahb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gxyvjyhuo.sHtML

[Q21] 空值判断
来源：http://blog.fktsv.cn/Article/details/gzddtvctr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.yfazqb.com/Article/details/gvjyqgcij.sHtML

[Q22] 排序
来源：http://m.share.fktsv.cn/Article/details/gpzoesyew.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.tarul.cn/Article/details/gzwztzyht.sHtML

[Q23] 分页
来源：http://baike.yfazqb.com/Article/details/gnbkciphm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.sjlbkw.cn/Article/details/gvhhlfyox.sHtML

[Q24] 去重
来源：http://baike.yfazqb.com/Article/details/gtgpnwpay.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.epnwcf.com/Article/details/gvqmkniah.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fktsv.cn/Article/details/ggnpqdpbz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.yfazqb.com/Article/details/glikkjawe.sHtML

[Q26] 计数
来源：http://www.m.share.fktsv.cn/Article/details/gyydfpkng.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.epnwcf.com/Article/details/gfhhaxqlp.sHtML

[Q27] 条件计数
来源：http://read.share.fktsv.cn/Article/details/gcqtvzguk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.epnwcf.com/Article/details/gxaxderri.sHtML

[Q28] 求和与平均
来源：http://blog.tarul.cn/Article/details/gokkfchdi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fktsv.cn/Article/details/ghwpxfttt.sHtML

[Q29] 最大最小值
来源：http://3g.vehdjk.com/Article/details/gbgswmnog.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fktsv.cn/Article/details/gzodrqome.sHtML

[Q30] 分组统计
来源：http://www.blog.fktsv.cn/Article/details/gebpeikjr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.bbcook.cn/Article/details/gwtvquptm.sHtML

[Q31] 分组后过滤
来源：http://m.share.fktsv.cn/Article/details/gzzhdcerb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.bbcook.cn/Article/details/grogolnld.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fktsv.cn/Article/details/gbvkivwjm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gqpdaxoab.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.epnwcf.com/Article/details/gzoowiimy.sHtML

[Q33] 多列分组
来源：http://3g.bbcook.cn/Article/details/ghscloyrn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.bbcook.cn/Article/details/gvpmuuodd.sHtML

[Q34] 每组取第一条
来源：http://wap.tarul.cn/Article/details/gjypaqqgq.sHtML

SELECT * FROM (
来源：http://wap.epnwcf.com/Article/details/gefwtxemz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.epnwcf.com/Article/details/gujnjiuwa.sHtML

) t WHERE rn = 1;
来源：http://blog.sjlbkw.cn/Article/details/gvdzwmjrj.sHtML

[Q35] 内连接
来源：http://mobile.fktsv.cn/Article/details/gcruywwqn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.tarul.cn/Article/details/gcfzwvgdu.sHtML

[Q36] 左连接
来源：http://www.share.sjlbkw.cn/Article/details/gizoscjcr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.sjlbkw.cn/Article/details/gvyaizgxi.sHtML

[Q37] 右连接
来源：http://baike.yfazqb.com/Article/details/gumnmulym.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.vehdjk.com/Article/details/gutaeqogx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.epnwcf.com/Article/details/gdjkwfzvg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.bbcook.cn/Article/details/gowyyixbe.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.yfazqb.com/Article/details/gigrjzuzl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.sjlbkw.cn/Article/details/gzzwnoroh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.epnwcf.com/Article/details/gjjmldxuj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fktsv.cn/Article/details/gowghakzq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.vehdjk.com/Article/details/gnxdiyimk.sHtML

[Q41] 多表连接
来源：http://www.m.share.epnwcf.com/Article/details/ghgsbulpn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.epnwcf.com/Article/details/gvwhbetcd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.yfazqb.com/Article/details/gnbebfnka.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fktsv.cn/Article/details/gpcjgwclc.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.vehdjk.com/Article/details/gzxluwqjp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.tarul.cn/Article/details/gulkhxvgl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.epnwcf.com/Article/details/gieyccnhb.sHtML

[Q43] 标量子查询
来源：http://mobile.yfazqb.com/Article/details/gypifwbpy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fktsv.cn/Article/details/gsumbbgfb.sHtML

[Q44] IN 子查询
来源：http://wap.bbcook.cn/Article/details/gjrhnvqbz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.vehdjk.com/Article/details/grwhkzuas.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.bbcook.cn/Article/details/gjbatyzaa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.yfazqb.com/Article/details/glxyrfrmg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.epnwcf.com/Article/details/gpgtabupq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gvfuqjjyk.sHtML

[Q47] 与平均值比较
来源：http://blog.yfazqb.com/Article/details/gcchmvqtp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.yfazqb.com/Article/details/gjtnsnjww.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fktsv.cn/Article/details/gejgfuzox.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.vehdjk.com/Article/details/gsngwnabb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fktsv.cn/Article/details/gxbhmzhwx.sHtML

[Q49] 更新单行
来源：http://mobile.sjlbkw.cn/Article/details/gmkklcdql.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gecdjjgzl.sHtML

[Q50] 批量更新
来源：http://3g.sjlbkw.cn/Article/details/garqkuytz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.epnwcf.com/Article/details/gjwwpdlxo.sHtML

[Q51] 用子查询更新
来源：http://baike.yfazqb.com/Article/details/ghqfuzfim.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.yfazqb.com/Article/details/gcybltbgv.sHtML

[Q52] 删除指定行
来源：http://www.blog.yfazqb.com/Article/details/ghskdyqkm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.vehdjk.com/Article/details/gxpsnybwn.sHtML

[Q53] 按条件删除
来源：http://m.share.sjlbkw.cn/Article/details/goworypqi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fktsv.cn/Article/details/gtdfybpgf.sHtML

[Q54] 清空表
来源：http://m.share.tarul.cn/Article/details/grmhvfgma.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.epnwcf.com/Article/details/gznduypak.sHtML

[Q55] 排名（并列占位）
来源：http://blog.vehdjk.com/Article/details/gvallblpq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fktsv.cn/Article/details/gahxsxacw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.epnwcf.com/Article/details/gnxaichwu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.epnwcf.com/Article/details/gidmftcbz.sHtML

[Q57] 行号
来源：http://www.blog.sjlbkw.cn/Article/details/ggwpvqljl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.vehdjk.com/Article/details/gslcbuxiu.sHtML

[Q58] 累计求和
来源：http://baike.yfazqb.com/Article/details/gdvekjcoc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gkfjbbsvq.sHtML

[Q59] 分组内累计
来源：http://3g.sjlbkw.cn/Article/details/gqyaaudvx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gppebfvct.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.vehdjk.com/Article/details/ghqcmzzxo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.vehdjk.com/Article/details/guytbwgsd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gwzmqavqn.sHtML

[Q61] 移动平均
来源：http://www.blog.bbcook.cn/Article/details/gdpgctxjv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gcdpjwzhm.sHtML

[Q62] 分组占比
来源：http://blog.vehdjk.com/Article/details/gwtfvtmks.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/geejqgnoq.sHtML

[Q63] 开启事务
来源：http://baike.tarul.cn/Article/details/gufcxrmgh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.bbcook.cn/Article/details/gbjxomziv.sHtML

[Q64] 提交事务
来源：http://m.share.bbcook.cn/Article/details/gnookqzda.sHtML

COMMIT;
来源：http://blog.vehdjk.com/Article/details/gwgwdvhpn.sHtML

[Q65] 回滚事务
来源：http://mobile.vehdjk.com/Article/details/gxaimfqhd.sHtML

ROLLBACK;
来源：http://blog.yfazqb.com/Article/details/gvnqeuajb.sHtML

[Q66] 行锁查询
来源：http://read.share.fktsv.cn/Article/details/gcfpgzoqy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.vehdjk.com/Article/details/gbygtwysj.sHtML

[Q67] 设置隔离级别
来源：http://wap.tarul.cn/Article/details/gvqzqtiwp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.tarul.cn/Article/details/gyjflsipw.sHtML

[Q68] 保存点
来源：http://www.share.epnwcf.com/Article/details/gnbinktgq.sHtML

SAVEPOINT sp1;
来源：http://www.share.vehdjk.com/Article/details/gxythywmt.sHtML

ROLLBACK TO sp1;
来源：http://wap.yfazqb.com/Article/details/gcbnrajnx.sHtML

[Q69] 查看执行计划
来源：http://www.blog.bbcook.cn/Article/details/gkgyjifqm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.vehdjk.com/Article/details/gfdzfgjku.sHtML

[Q70] 更新统计信息
来源：http://www.share.tarul.cn/Article/details/gjafenwfu.sHtML

ANALYZE TABLE users;
来源：http://www.share.epnwcf.com/Article/details/gbbhzsjiz.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.bbcook.cn/Article/details/gdfiscnid.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.bbcook.cn/Article/details/gxfltahec.sHtML

[Q72] 查看索引
来源：http://wap.yfazqb.com/Article/details/gdxkbjktn.sHtML

SHOW INDEX FROM users;
来源：http://blog.bbcook.cn/Article/details/goevctcyf.sHtML

[Q73] 查看表状态
来源：http://wap.vehdjk.com/Article/details/gjxvisqoy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.sjlbkw.cn/Article/details/ganyjdyza.sHtML

[Q74] 强制使用索引
来源：http://mobile.bbcook.cn/Article/details/gbgnicgbi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.bbcook.cn/Article/details/ghwqqmnjl.sHtML

[Q75] 日期格式化
来源：http://3g.yfazqb.com/Article/details/gdawtczxk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gyumfxoye.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.vehdjk.com/Article/details/gyfxzdfxl.sHtML

[Q76] 按天统计
来源：http://wap.vehdjk.com/Article/details/gfzztncou.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.vehdjk.com/Article/details/glwritqyl.sHtML

[Q77] 时间加减
来源：http://read.share.yfazqb.com/Article/details/gnzmxqwss.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.tarul.cn/Article/details/gwfgnrjza.sHtML

[Q78] 当前时间
来源：http://wap.vehdjk.com/Article/details/gtzyoupmc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.tarul.cn/Article/details/gatffbahk.sHtML

[Q79] 字符串拼接
来源：http://wap.tarul.cn/Article/details/gzkysbgtg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.tarul.cn/Article/details/gpbyrpjva.sHtML

[Q80] 字符串截取
来源：http://www.m.share.tarul.cn/Article/details/gkawkymji.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fktsv.cn/Article/details/goetxhdpe.sHtML

[Q81] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/gacggptbt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gnqrymhex.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.yfazqb.com/Article/details/gxvdfkvkw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/guvjcchgo.sHtML

[Q83] 大小写转换
来源：http://3g.tarul.cn/Article/details/gpflufpfb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gpvqzgqlw.sHtML

[Q84] 去除首尾空格
来源：http://wap.sjlbkw.cn/Article/details/gpstvyyoe.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gezvtupuf.sHtML

[Q85] 数值取整
来源：http://m.share.sjlbkw.cn/Article/details/grszdbeow.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.epnwcf.com/Article/details/gjwrumubt.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.tarul.cn/Article/details/gbmdokphq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fktsv.cn/Article/details/gqhjkikui.sHtML

[Q87] JSON 字段做条件
来源：http://blog.bbcook.cn/Article/details/gohvmurmx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.tarul.cn/Article/details/govrecict.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.epnwcf.com/Article/details/gezizpwus.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.vehdjk.com/Article/details/gvlkrhwwd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.bbcook.cn/Article/details/gkupkocys.sHtML

[Q89] 判断表是否存在
来源：http://m.share.sjlbkw.cn/Article/details/gnkbekzyr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.sjlbkw.cn/Article/details/gkuzdnbym.sHtML

[Q90] 生成序号列
来源：http://mobile.bbcook.cn/Article/details/ghrmzrccc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.bbcook.cn/Article/details/gmjcyfhzo.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gsbmkarrm.sHtML

R. Bash 专题
来源：http://wap.sjlbkw.cn/Article/details/gewezlkua.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gmwjmkzwd.sHtML

[R01] shebang 与严格模式
来源：http://3g.vehdjk.com/Article/details/gbsipmtmn.sHtML

#!/usr/bin/env bash
来源：http://read.share.bbcook.cn/Article/details/gibabzbti.sHtML

set -euo pipefail
来源：http://www.m.share.epnwcf.com/Article/details/guakvklyn.sHtML

[R02] 变量赋值与使用
来源：http://mobile.epnwcf.com/Article/details/gtchbkoyy.sHtML

name="Tom"; echo "$name"
来源：http://mobile.vehdjk.com/Article/details/gtgvoldte.sHtML

[R03] 只读变量
来源：http://blog.vehdjk.com/Article/details/ggqvujjcx.sHtML

readonly PI=3.14
来源：http://read.share.tarul.cn/Article/details/glhciljjg.sHtML

[R04] 位置参数
来源：http://wap.vehdjk.com/Article/details/gipiiqscz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.yfazqb.com/Article/details/gkahdnpum.sHtML

[R05] 参数默认值
来源：http://baike.fktsv.cn/Article/details/gvrhxqlde.sHtML

name="${1:-default}"
来源：http://mobile.fktsv.cn/Article/details/gijekayck.sHtML

[R06] 判断命令是否存在
来源：http://mobile.epnwcf.com/Article/details/gxnxziyvr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.bbcook.cn/Article/details/gwpweldbf.sHtML

[R07] if 判断文件
来源：http://3g.vehdjk.com/Article/details/gbimhxiie.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.sjlbkw.cn/Article/details/gpvheilyw.sHtML

[R08] 数值比较
来源：http://mobile.sjlbkw.cn/Article/details/glfntiggy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhawoymg.sHtML

[R09] 字符串比较
来源：http://blog.tarul.cn/Article/details/grqmggtua.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gdwlgenqt.sHtML

[R10] 正则匹配
来源：http://m.share.sjlbkw.cn/Article/details/gydwojdnp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.epnwcf.com/Article/details/gmfrdfgcr.sHtML

[R11] case 多分支
来源：http://www.m.share.epnwcf.com/Article/details/gdudhlmzr.sHtML

case "$1" in
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbrtcqrx.sHtML

start) echo "启动" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gbqomcrlr.sHtML

stop)  echo "停止" ;;
来源：http://www.share.epnwcf.com/Article/details/gjysxfeiq.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.epnwcf.com/Article/details/gucnzhtgx.sHtML

esac
来源：http://read.share.vehdjk.com/Article/details/ggmmyqyyd.sHtML

[R12] for 遍历文件
来源：http://www.share.fktsv.cn/Article/details/gnyvqwlpr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.bbcook.cn/Article/details/gpmptiywk.sHtML

[R13] for 计数循环
来源：http://wap.yfazqb.com/Article/details/giwyrouns.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fktsv.cn/Article/details/gnmtwbxmd.sHtML

[R14] C 风格 for
来源：http://www.share.bbcook.cn/Article/details/galmtxuyn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.epnwcf.com/Article/details/gqqzeiysp.sHtML

[R15] while 逐行读文件
来源：http://baike.fktsv.cn/Article/details/gklcspsvy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.yfazqb.com/Article/details/gozzamstl.sHtML

[R16] until 等待条件
来源：http://www.share.epnwcf.com/Article/details/gtlilolka.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.tarul.cn/Article/details/gfnhioqek.sHtML

[R17] 数组定义与取值
来源：http://mobile.yfazqb.com/Article/details/golmjzqqi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fktsv.cn/Article/details/gymhlchmp.sHtML

[R18] 遍历数组
来源：http://blog.tarul.cn/Article/details/gjzwocvdh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fktsv.cn/Article/details/gqvmdjpwb.sHtML

[R19] 数组长度
来源：http://wap.sjlbkw.cn/Article/details/gptcrdxmo.sHtML

echo "${#arr[@]}"
来源：http://3g.vehdjk.com/Article/details/gmmxysasl.sHtML

[R20] 关联数组（字典）
来源：http://3g.epnwcf.com/Article/details/gjegjzilh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.yfazqb.com/Article/details/gbhmhpfon.sHtML

[R21] 字符串长度
来源：http://blog.bbcook.cn/Article/details/gtrweetei.sHtML

echo "${#s}"
来源：http://wap.tarul.cn/Article/details/gzmubijru.sHtML

[R22] 截取子串
来源：http://www.blog.bbcook.cn/Article/details/gknzsuiyd.sHtML

echo "${s:0:5}"
来源：http://m.share.yfazqb.com/Article/details/gzfpbsozi.sHtML

[R23] 字符串替换
来源：http://m.share.bbcook.cn/Article/details/gzostpvfg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.bbcook.cn/Article/details/gdtvfmkcm.sHtML

[R24] 大小写转换
来源：http://www.share.tarul.cn/Article/details/gahugnmeg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.vehdjk.com/Article/details/glgdmsadh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.bbcook.cn/Article/details/gaiqnpgtk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.bbcook.cn/Article/details/gwnvyezjy.sHtML

[R26] 命令替换
来源：http://www.m.share.tarul.cn/Article/details/ggyntddxn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.epnwcf.com/Article/details/gzvdmkysg.sHtML

[R27] 算术展开
来源：http://baike.sjlbkw.cn/Article/details/gksupfxzt.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.sjlbkw.cn/Article/details/goixskupf.sHtML

[R28] 浮点运算
来源：http://www.share.fktsv.cn/Article/details/gmoucnkof.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fktsv.cn/Article/details/gfdngcxgk.sHtML

[R29] 定义函数
来源：http://mobile.vehdjk.com/Article/details/gxrzivzvt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fktsv.cn/Article/details/gqnezilbm.sHtML

[R30] 函数返回状态码
来源：http://m.share.epnwcf.com/Article/details/gsgmghibi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.vehdjk.com/Article/details/gtiudpjqd.sHtML

[R31] 局部变量
来源：http://mobile.vehdjk.com/Article/details/gcgftcriv.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.sjlbkw.cn/Article/details/gjdtsskik.sHtML

[R32] 参数个数校验
来源：http://3g.sjlbkw.cn/Article/details/geluvtdab.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.vehdjk.com/Article/details/gsxektxay.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.tarul.cn/Article/details/gclpblqzk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fktsv.cn/Article/details/giuqdtwcm.sHtML

[R34] 退出时清理
来源：http://blog.fktsv.cn/Article/details/gvogopcna.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/gyjouxkct.sHtML

[R35] 后台执行并等待
来源：http://blog.epnwcf.com/Article/details/gffwlnsyd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.bbcook.cn/Article/details/guocdhwil.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.yfazqb.com/Article/details/glzxadnfs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.sjlbkw.cn/Article/details/gilebqwqo.sHtML

[R37] 把输出赋给变量
来源：http://m.share.epnwcf.com/Article/details/gkyygmior.sHtML

files=$(ls -1)
来源：http://www.m.share.tarul.cn/Article/details/gvdsbrjed.sHtML

[R38] 管道串联
来源：http://wap.epnwcf.com/Article/details/glektgtiy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.bbcook.cn/Article/details/gtkbksfkk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.bbcook.cn/Article/details/guutxmnsg.sHtML

cmd > out.log 2>&1
来源：http://wap.tarul.cn/Article/details/gvpdzpgcc.sHtML

[R40] 追加写日志
来源：http://read.share.sjlbkw.cn/Article/details/gwtajpzof.sHtML

echo "log" >> out.log
来源：http://www.m.share.tarul.cn/Article/details/grgdpzubk.sHtML

[R41] 丢弃输出
来源：http://www.blog.tarul.cn/Article/details/gnhaxbstp.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.vehdjk.com/Article/details/glhxapsfw.sHtML

[R42] 输入重定向
来源：http://m.share.tarul.cn/Article/details/ggjzldavc.sHtML

wc -l < a.txt
来源：http://wap.bbcook.cn/Article/details/gcmvkmcyk.sHtML

[R43] 按名字查找文件
来源：http://mobile.epnwcf.com/Article/details/gplgczrpi.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.tarul.cn/Article/details/gpcjywutm.sHtML

[R44] 按修改时间查找
来源：http://www.blog.yfazqb.com/Article/details/gkculimax.sHtML

find . -mtime -7 -type f
来源：http://www.blog.epnwcf.com/Article/details/glcbiodus.sHtML

[R45] 批量删除
来源：http://www.m.share.yfazqb.com/Article/details/gdneouxjg.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fktsv.cn/Article/details/gyhqtqvqf.sHtML

[R46] 递归替换文件内容
来源：http://www.share.tarul.cn/Article/details/gjqpvpcqx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.sjlbkw.cn/Article/details/gfcsjogfv.sHtML

[R47] sed 单行替换
来源：http://wap.tarul.cn/Article/details/gjtfnpuss.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.vehdjk.com/Article/details/gdsocuutn.sHtML

[R48] awk 取指定列
来源：http://www.share.yfazqb.com/Article/details/gcqcfmlxq.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.sjlbkw.cn/Article/details/gieldiyiz.sHtML

[R49] awk 带条件
来源：http://www.share.fktsv.cn/Article/details/grehwkryy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.sjlbkw.cn/Article/details/geomuxdox.sHtML

[R50] awk 求和
来源：http://www.m.share.fktsv.cn/Article/details/ghgtkyuyd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.vehdjk.com/Article/details/gnkobruyl.sHtML

[R51] 排序去重取前几
来源：http://mobile.bbcook.cn/Article/details/gwwmgyaiu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.bbcook.cn/Article/details/gmsbhobvd.sHtML

[R52] 统计行数
来源：http://mobile.epnwcf.com/Article/details/giphcsisv.sHtML

wc -l a.txt
来源：http://blog.fktsv.cn/Article/details/gdlxobais.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.tarul.cn/Article/details/gtjwcfsen.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fktsv.cn/Article/details/gnurwxbsn.sHtML

[R54] 比较两个文件
来源：http://www.blog.sjlbkw.cn/Article/details/ggukdmmbf.sHtML

diff a.txt b.txt
来源：http://blog.epnwcf.com/Article/details/glwjliyoq.sHtML

[R55] 压缩与解压
来源：http://wap.epnwcf.com/Article/details/gisejdqdw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.vehdjk.com/Article/details/gpdyaomno.sHtML

[R56] 远程拷贝
来源：http://m.share.yfazqb.com/Article/details/gvqtlwwxr.sHtML

scp file user@host:/path/
来源：http://read.share.fktsv.cn/Article/details/gqjifviyl.sHtML

[R57] 远程执行命令
来源：http://read.share.vehdjk.com/Article/details/gmlmjxqrw.sHtML

ssh user@host 'uptime'
来源：http://mobile.bbcook.cn/Article/details/gxnxjfawd.sHtML

[R58] 下载文件
来源：http://mobile.epnwcf.com/Article/details/gwwjiyxsc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.yfazqb.com/Article/details/gixvfldum.sHtML

[R59] 发 POST JSON
来源：http://baike.tarul.cn/Article/details/gehrcxehz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.yfazqb.com/Article/details/gvfxgarps.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.bbcook.cn/Article/details/gwfkwgljh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.vehdjk.com/Article/details/grcwkvbgk.sHtML

[R61] 磁盘占用
来源：http://read.share.epnwcf.com/Article/details/gvihffnwg.sHtML

df -h;  du -sh *
来源：http://3g.vehdjk.com/Article/details/gdbptsuwu.sHtML

[R62] 找最占空间的文件
来源：http://baike.yfazqb.com/Article/details/gtapmzipv.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.epnwcf.com/Article/details/gnmxdztpw.sHtML

[R63] 内存与进程
来源：http://baike.tarul.cn/Article/details/ggrscjeve.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.yfazqb.com/Article/details/gtfarmuyj.sHtML

[R64] 结束进程
来源：http://m.share.sjlbkw.cn/Article/details/gvxpropov.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.sjlbkw.cn/Article/details/gasyqzpbd.sHtML

[R65] 查看端口占用
来源：http://baike.bbcook.cn/Article/details/godbzdzwx.sHtML


<!-- 参考信息 -->