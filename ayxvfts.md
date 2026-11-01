代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.share.vehdjk.com/Article/details/gjicqaafd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.vehdjk.com/Article/details/gzqjaxtat.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.yfazqb.com/Article/details/ginaaqcys.sHtML

[Q15] 查询全部
来源：http://www.blog.epnwcf.com/Article/details/guujusvtr.sHtML

SELECT * FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gltztopbf.sHtML

[Q16] 查询指定列
来源：http://mobile.epnwcf.com/Article/details/gxabiynpm.sHtML

SELECT id, name FROM users;
来源：http://mobile.yfazqb.com/Article/details/gdnyehigo.sHtML

[Q17] 条件查询
来源：http://wap.tarul.cn/Article/details/gcywooris.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.bbcook.cn/Article/details/gqvpohbot.sHtML

[Q18] 模糊匹配
来源：http://3g.yfazqb.com/Article/details/ggybxsfxz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.epnwcf.com/Article/details/gjquwdxep.sHtML

[Q19] 范围查询
来源：http://mobile.tarul.cn/Article/details/gpserjjhq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.tarul.cn/Article/details/gmydvusmx.sHtML

[Q20] IN 列表
来源：http://3g.yfazqb.com/Article/details/gkpirefqe.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.sjlbkw.cn/Article/details/ganffychj.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/gnqmqoopr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.tarul.cn/Article/details/gxhlhgonu.sHtML

[Q22] 排序
来源：http://wap.tarul.cn/Article/details/gzkgzqdwv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.bbcook.cn/Article/details/gzqsqbqfe.sHtML

[Q23] 分页
来源：http://read.share.sjlbkw.cn/Article/details/glbcsqugo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.yfazqb.com/Article/details/gcoqunvfq.sHtML

[Q24] 去重
来源：http://wap.yfazqb.com/Article/details/ggxxzlnsg.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.epnwcf.com/Article/details/gtaqfgycv.sHtML

[Q25] 只取前 N 条
来源：http://wap.epnwcf.com/Article/details/glhzauved.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.yfazqb.com/Article/details/gfdjnceok.sHtML

[Q26] 计数
来源：http://m.share.vehdjk.com/Article/details/grqogajbn.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gmtuxqmfr.sHtML

[Q27] 条件计数
来源：http://baike.fktsv.cn/Article/details/gzeftmkxc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gcahevhej.sHtML

[Q28] 求和与平均
来源：http://wap.epnwcf.com/Article/details/gwkcryqqj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fktsv.cn/Article/details/ggibjetcb.sHtML

[Q29] 最大最小值
来源：http://wap.tarul.cn/Article/details/gxuhomdms.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/glwnrbbfq.sHtML

[Q30] 分组统计
来源：http://m.share.tarul.cn/Article/details/gfltqedvj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmezcvgc.sHtML

[Q31] 分组后过滤
来源：http://blog.yfazqb.com/Article/details/gbccgkrss.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.epnwcf.com/Article/details/glqjtutzv.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gjslpmynb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/ghrcazqlj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.epnwcf.com/Article/details/gqpuyuptx.sHtML

[Q33] 多列分组
来源：http://m.share.bbcook.cn/Article/details/glonqgalx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fktsv.cn/Article/details/ghprwkqxa.sHtML

[Q34] 每组取第一条
来源：http://www.blog.sjlbkw.cn/Article/details/glctrvmdm.sHtML

SELECT * FROM (
来源：http://wap.fktsv.cn/Article/details/gtsujuumm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.tarul.cn/Article/details/ghusyavpg.sHtML

) t WHERE rn = 1;
来源：http://mobile.vehdjk.com/Article/details/ggnkkstzr.sHtML

[Q35] 内连接
来源：http://www.m.share.fktsv.cn/Article/details/gsfnjimpk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/gtphgffdi.sHtML

[Q36] 左连接
来源：http://www.blog.yfazqb.com/Article/details/gmjjtvsgc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.sjlbkw.cn/Article/details/gfnelhqng.sHtML

[Q37] 右连接
来源：http://wap.fktsv.cn/Article/details/gvexdnyej.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.vehdjk.com/Article/details/gxgozxyfz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.yfazqb.com/Article/details/ggaurpbax.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.bbcook.cn/Article/details/gleagprwu.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.bbcook.cn/Article/details/gtvzddnwq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.epnwcf.com/Article/details/ghbmlflxa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.bbcook.cn/Article/details/guvolvmva.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.vehdjk.com/Article/details/gytielmyt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.vehdjk.com/Article/details/gsncsfffb.sHtML

[Q41] 多表连接
来源：http://blog.epnwcf.com/Article/details/gdbtydtlz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.vehdjk.com/Article/details/gnckwxboh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.tarul.cn/Article/details/gdvtankcp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.vehdjk.com/Article/details/gmlpyknjl.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fktsv.cn/Article/details/gqjjqxtlk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.sjlbkw.cn/Article/details/gfkynnnbo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.bbcook.cn/Article/details/gurrbzzux.sHtML

[Q43] 标量子查询
来源：http://mobile.bbcook.cn/Article/details/gvbxzckpy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.tarul.cn/Article/details/gqvlbjurr.sHtML

[Q44] IN 子查询
来源：http://www.share.sjlbkw.cn/Article/details/gcwppmktc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.bbcook.cn/Article/details/gokvsdtug.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.epnwcf.com/Article/details/gssrpehez.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.bbcook.cn/Article/details/grdlgjdjr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.epnwcf.com/Article/details/gqunhwjtx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.vehdjk.com/Article/details/gzanlmiry.sHtML

[Q47] 与平均值比较
来源：http://wap.yfazqb.com/Article/details/gmwxzcjto.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.tarul.cn/Article/details/gzyearzaa.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.tarul.cn/Article/details/gdqpfelse.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.bbcook.cn/Article/details/gyydttuqt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.vehdjk.com/Article/details/gnncdsrue.sHtML

[Q49] 更新单行
来源：http://www.share.fktsv.cn/Article/details/ggrmijhdr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.sjlbkw.cn/Article/details/geelxjfam.sHtML

[Q50] 批量更新
来源：http://blog.epnwcf.com/Article/details/gctipwuip.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.tarul.cn/Article/details/gxdsaqrph.sHtML

[Q51] 用子查询更新
来源：http://mobile.epnwcf.com/Article/details/grgnkvltl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.tarul.cn/Article/details/gxhjoyqmr.sHtML

[Q52] 删除指定行
来源：http://www.share.tarul.cn/Article/details/gsbckwhra.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/gtbxbeeka.sHtML

[Q53] 按条件删除
来源：http://baike.epnwcf.com/Article/details/gtritrnel.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.vehdjk.com/Article/details/gtjgnwetl.sHtML

[Q54] 清空表
来源：http://blog.epnwcf.com/Article/details/gwxxeqlzt.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fktsv.cn/Article/details/ggvpngaxf.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fktsv.cn/Article/details/gjpmpawzk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.epnwcf.com/Article/details/gwqgatzbe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.tarul.cn/Article/details/gokshxftr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.yfazqb.com/Article/details/gcrhzeduq.sHtML

[Q57] 行号
来源：http://www.blog.bbcook.cn/Article/details/gpxqtuodn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gmagnsgtz.sHtML

[Q58] 累计求和
来源：http://wap.tarul.cn/Article/details/ggyxpgywf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.tarul.cn/Article/details/gwrlfugyq.sHtML

[Q59] 分组内累计
来源：http://baike.tarul.cn/Article/details/grpaakgnf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/ghtpdeqcm.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.tarul.cn/Article/details/gspellvgx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.sjlbkw.cn/Article/details/gchonrjqs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.yfazqb.com/Article/details/glkhkluvk.sHtML

[Q61] 移动平均
来源：http://m.share.fktsv.cn/Article/details/gnydtmvvt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/grztmjzux.sHtML

[Q62] 分组占比
来源：http://www.share.bbcook.cn/Article/details/gzygswrug.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gypsytrdw.sHtML

[Q63] 开启事务
来源：http://wap.epnwcf.com/Article/details/gakabawfy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.bbcook.cn/Article/details/gwsbdzgby.sHtML

[Q64] 提交事务
来源：http://www.m.share.epnwcf.com/Article/details/gfnavkfat.sHtML

COMMIT;
来源：http://m.share.tarul.cn/Article/details/glbkdfwkt.sHtML

[Q65] 回滚事务
来源：http://blog.vehdjk.com/Article/details/gnfdsqrok.sHtML

ROLLBACK;
来源：http://www.m.share.vehdjk.com/Article/details/gmfqocjfl.sHtML

[Q66] 行锁查询
来源：http://baike.sjlbkw.cn/Article/details/gtpjvqddm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.vehdjk.com/Article/details/gzrdctvro.sHtML

[Q67] 设置隔离级别
来源：http://mobile.yfazqb.com/Article/details/gdeqaskth.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.tarul.cn/Article/details/gfujuvsnk.sHtML

[Q68] 保存点
来源：http://blog.epnwcf.com/Article/details/ghksszazj.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.vehdjk.com/Article/details/gkrlahjtu.sHtML

ROLLBACK TO sp1;
来源：http://baike.yfazqb.com/Article/details/gcrgipmvu.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fktsv.cn/Article/details/gyvrerqnw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fktsv.cn/Article/details/gwlizohqc.sHtML

[Q70] 更新统计信息
来源：http://mobile.tarul.cn/Article/details/gewelptpx.sHtML

ANALYZE TABLE users;
来源：http://www.blog.bbcook.cn/Article/details/gkeogwqgp.sHtML

[Q71] 查看建表语句
来源：http://wap.fktsv.cn/Article/details/gjfpzeakz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.tarul.cn/Article/details/gtrwguyti.sHtML

[Q72] 查看索引
来源：http://m.share.vehdjk.com/Article/details/grupeufmd.sHtML

SHOW INDEX FROM users;
来源：http://baike.sjlbkw.cn/Article/details/ggjhzqqkq.sHtML

[Q73] 查看表状态
来源：http://wap.fktsv.cn/Article/details/gwkigothr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.yfazqb.com/Article/details/gxwmcftfo.sHtML

[Q74] 强制使用索引
来源：http://wap.sjlbkw.cn/Article/details/gerujsmlg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.tarul.cn/Article/details/gbdklzxkq.sHtML

[Q75] 日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/grypoumqb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gjylyxmvu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fktsv.cn/Article/details/gywvkwlqm.sHtML

[Q76] 按天统计
来源：http://www.share.tarul.cn/Article/details/ggapmsyti.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.epnwcf.com/Article/details/guwwqkubu.sHtML

[Q77] 时间加减
来源：http://www.m.share.tarul.cn/Article/details/guqgmfyeb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.bbcook.cn/Article/details/gjtsrjdxo.sHtML

[Q78] 当前时间
来源：http://read.share.tarul.cn/Article/details/graeerlnz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.tarul.cn/Article/details/guhifiyfa.sHtML

[Q79] 字符串拼接
来源：http://www.blog.tarul.cn/Article/details/gpnygypch.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.bbcook.cn/Article/details/gvtthiyfk.sHtML

[Q80] 字符串截取
来源：http://wap.vehdjk.com/Article/details/gdbhbvasv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.vehdjk.com/Article/details/gekczscpv.sHtML

[Q81] 字符串替换
来源：http://www.share.tarul.cn/Article/details/gyiwtvwac.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.yfazqb.com/Article/details/gdstrbhra.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fktsv.cn/Article/details/gsoegppjx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gukemdtfx.sHtML

[Q83] 大小写转换
来源：http://blog.tarul.cn/Article/details/gwwpztwsi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gkpvrsrjt.sHtML

[Q84] 去除首尾空格
来源：http://wap.tarul.cn/Article/details/gbfibkkol.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gphjpfyfi.sHtML

[Q85] 数值取整
来源：http://blog.sjlbkw.cn/Article/details/graxaksiy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.bbcook.cn/Article/details/goalfqluv.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.bbcook.cn/Article/details/gvukxszqr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.tarul.cn/Article/details/gtyqagemw.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.tarul.cn/Article/details/gpolsyzlw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.tarul.cn/Article/details/gafudwelr.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.sjlbkw.cn/Article/details/gszvddamh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.tarul.cn/Article/details/gwgizraex.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gjnqgkbcc.sHtML

[Q89] 判断表是否存在
来源：http://baike.sjlbkw.cn/Article/details/gyrsngveh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fktsv.cn/Article/details/gffbuefzq.sHtML

[Q90] 生成序号列
来源：http://read.share.sjlbkw.cn/Article/details/gqgpkbadn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.epnwcf.com/Article/details/gcjsqcxdv.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gvvibnfay.sHtML

R. Bash 专题
来源：http://baike.yfazqb.com/Article/details/gokyfsjqa.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gxqbqvdhq.sHtML

[R01] shebang 与严格模式
来源：http://read.share.yfazqb.com/Article/details/gutzrcwah.sHtML

#!/usr/bin/env bash
来源：http://www.blog.sjlbkw.cn/Article/details/gmpgpankt.sHtML

set -euo pipefail
来源：http://blog.bbcook.cn/Article/details/gdqioultw.sHtML

[R02] 变量赋值与使用
来源：http://www.share.vehdjk.com/Article/details/gpuisvziq.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.epnwcf.com/Article/details/glsdhkedo.sHtML

[R03] 只读变量
来源：http://www.m.share.fktsv.cn/Article/details/gtyythuzh.sHtML

readonly PI=3.14
来源：http://3g.tarul.cn/Article/details/gzqsgmzcb.sHtML

[R04] 位置参数
来源：http://www.blog.bbcook.cn/Article/details/gvjnptjpy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.tarul.cn/Article/details/gyhrtceof.sHtML

[R05] 参数默认值
来源：http://baike.epnwcf.com/Article/details/ghbokvzln.sHtML

name="${1:-default}"
来源：http://www.m.share.vehdjk.com/Article/details/gvsdjwhpb.sHtML

[R06] 判断命令是否存在
来源：http://3g.vehdjk.com/Article/details/grjzslsxt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.tarul.cn/Article/details/gyiggvzsx.sHtML

[R07] if 判断文件
来源：http://m.share.tarul.cn/Article/details/ghqrvrvaw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.tarul.cn/Article/details/gmthkmnkr.sHtML

[R08] 数值比较
来源：http://www.share.fktsv.cn/Article/details/gpnwercoy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.yfazqb.com/Article/details/gxyfnhzqj.sHtML

[R09] 字符串比较
来源：http://wap.yfazqb.com/Article/details/gousiobxg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.epnwcf.com/Article/details/gupyqgihm.sHtML

[R10] 正则匹配
来源：http://mobile.yfazqb.com/Article/details/geapypouz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gevbxvufr.sHtML

[R11] case 多分支
来源：http://www.share.fktsv.cn/Article/details/gbbdjboyy.sHtML

case "$1" in
来源：http://m.share.fktsv.cn/Article/details/gsqewfmlq.sHtML

start) echo "启动" ;;
来源：http://www.m.share.epnwcf.com/Article/details/grhjaadmi.sHtML

stop)  echo "停止" ;;
来源：http://3g.tarul.cn/Article/details/gbqwequih.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.yfazqb.com/Article/details/gclsdvccl.sHtML

esac
来源：http://www.m.share.bbcook.cn/Article/details/gvreobleh.sHtML

[R12] for 遍历文件
来源：http://www.m.share.vehdjk.com/Article/details/gcdbkflav.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.tarul.cn/Article/details/gkoixwneq.sHtML

[R13] for 计数循环
来源：http://www.blog.sjlbkw.cn/Article/details/gwjvizrmx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.vehdjk.com/Article/details/gasfndvfp.sHtML

[R14] C 风格 for
来源：http://3g.sjlbkw.cn/Article/details/gostuhkis.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fktsv.cn/Article/details/gxkyvscum.sHtML

[R15] while 逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gwwhjvoto.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.yfazqb.com/Article/details/goutuvjku.sHtML

[R16] until 等待条件
来源：http://www.blog.tarul.cn/Article/details/gqaapptjy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.sjlbkw.cn/Article/details/gapjdkgng.sHtML

[R17] 数组定义与取值
来源：http://m.share.fktsv.cn/Article/details/goonzjgph.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.epnwcf.com/Article/details/gihgznwnr.sHtML

[R18] 遍历数组
来源：http://baike.yfazqb.com/Article/details/gtrcclvbz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.vehdjk.com/Article/details/ggqqoqjqf.sHtML

[R19] 数组长度
来源：http://www.blog.yfazqb.com/Article/details/gsnjrgtnd.sHtML

echo "${#arr[@]}"
来源：http://m.share.sjlbkw.cn/Article/details/gvnkvqypd.sHtML

[R20] 关联数组（字典）
来源：http://read.share.sjlbkw.cn/Article/details/gccdpptib.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fktsv.cn/Article/details/gsttqkvik.sHtML

[R21] 字符串长度
来源：http://wap.sjlbkw.cn/Article/details/gxldrqnvw.sHtML

echo "${#s}"
来源：http://read.share.yfazqb.com/Article/details/gpefcessk.sHtML

[R22] 截取子串
来源：http://mobile.bbcook.cn/Article/details/gonjwiqol.sHtML

echo "${s:0:5}"
来源：http://blog.bbcook.cn/Article/details/gpfsgbtkm.sHtML

[R23] 字符串替换
来源：http://www.m.share.vehdjk.com/Article/details/gargexbyx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.yfazqb.com/Article/details/ggmzhuayw.sHtML

[R24] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/ghkagutwa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.tarul.cn/Article/details/grfpkjhub.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.vehdjk.com/Article/details/gawdlkyao.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.tarul.cn/Article/details/gfqmyorla.sHtML

[R26] 命令替换
来源：http://www.m.share.yfazqb.com/Article/details/gybwicqug.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.epnwcf.com/Article/details/gvkcsvlsb.sHtML

[R27] 算术展开
来源：http://blog.yfazqb.com/Article/details/gfwpydkyi.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.bbcook.cn/Article/details/gpacvfolw.sHtML

[R28] 浮点运算
来源：http://www.blog.fktsv.cn/Article/details/gpicfatwl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.yfazqb.com/Article/details/gnaqdqveg.sHtML

[R29] 定义函数
来源：http://read.share.tarul.cn/Article/details/gbnefsvqp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.vehdjk.com/Article/details/gvlyljols.sHtML

[R30] 函数返回状态码
来源：http://www.share.vehdjk.com/Article/details/gqbtzjdwm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.sjlbkw.cn/Article/details/gehshigzz.sHtML

[R31] 局部变量
来源：http://wap.fktsv.cn/Article/details/gunucemnz.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.vehdjk.com/Article/details/gqrywsxci.sHtML

[R32] 参数个数校验
来源：http://wap.sjlbkw.cn/Article/details/gehvhxgwg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/guzlidwge.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.tarul.cn/Article/details/gpigkvvsz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.vehdjk.com/Article/details/gwgfdjblq.sHtML

[R34] 退出时清理
来源：http://www.blog.bbcook.cn/Article/details/giqhxpdft.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gtnzaznme.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.yfazqb.com/Article/details/ghwateztt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.sjlbkw.cn/Article/details/glpaishys.sHtML

[R36] 并发执行多个任务
来源：http://baike.yfazqb.com/Article/details/ghifqnghw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fktsv.cn/Article/details/gmfmjouxk.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.bbcook.cn/Article/details/geosfeihp.sHtML

files=$(ls -1)
来源：http://mobile.tarul.cn/Article/details/gjyzzkbcu.sHtML

[R38] 管道串联
来源：http://www.m.share.sjlbkw.cn/Article/details/geqaxvrtd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.tarul.cn/Article/details/ghvvtzhsl.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fktsv.cn/Article/details/gjnupwfew.sHtML

cmd > out.log 2>&1
来源：http://www.share.vehdjk.com/Article/details/gbuvjqzmb.sHtML

[R40] 追加写日志
来源：http://wap.yfazqb.com/Article/details/gwesgfqja.sHtML

echo "log" >> out.log
来源：http://www.blog.fktsv.cn/Article/details/gufqlwena.sHtML

[R41] 丢弃输出
来源：http://m.share.fktsv.cn/Article/details/grotyaooy.sHtML

cmd >/dev/null 2>&1
来源：http://blog.yfazqb.com/Article/details/gnxeqkhmf.sHtML

[R42] 输入重定向
来源：http://3g.yfazqb.com/Article/details/gbtzpkcsg.sHtML

wc -l < a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gwpcgvyrj.sHtML

[R43] 按名字查找文件
来源：http://www.blog.yfazqb.com/Article/details/gcpgigywi.sHtML

find . -name "*.log" -type f
来源：http://www.share.vehdjk.com/Article/details/ggwfksyvq.sHtML

[R44] 按修改时间查找
来源：http://m.share.sjlbkw.cn/Article/details/gfdbhcxzz.sHtML

find . -mtime -7 -type f
来源：http://www.share.bbcook.cn/Article/details/gkofpaupg.sHtML

[R45] 批量删除
来源：http://www.share.yfazqb.com/Article/details/gnzjgqowe.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.vehdjk.com/Article/details/gzhcxlhbn.sHtML

[R46] 递归替换文件内容
来源：http://blog.epnwcf.com/Article/details/gujlqxjnh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.tarul.cn/Article/details/glnpbirms.sHtML

[R47] sed 单行替换
来源：http://www.m.share.epnwcf.com/Article/details/gzaawtzed.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.vehdjk.com/Article/details/gbraqbgqr.sHtML

[R48] awk 取指定列
来源：http://www.m.share.tarul.cn/Article/details/gwdcnkktt.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/ggmuqwusj.sHtML

[R49] awk 带条件
来源：http://mobile.sjlbkw.cn/Article/details/gpzpsevfk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.tarul.cn/Article/details/gcumukvpr.sHtML

[R50] awk 求和
来源：http://www.blog.yfazqb.com/Article/details/gerbjzfiw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.tarul.cn/Article/details/gsjwrwnqe.sHtML

[R51] 排序去重取前几
来源：http://www.blog.epnwcf.com/Article/details/ghhaiwlwn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.sjlbkw.cn/Article/details/ggklrhldy.sHtML

[R52] 统计行数
来源：http://3g.epnwcf.com/Article/details/gekqkzjfw.sHtML

wc -l a.txt
来源：http://read.share.fktsv.cn/Article/details/gngskcfqu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.yfazqb.com/Article/details/gclhbjmtk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.yfazqb.com/Article/details/gzxndwpey.sHtML

[R54] 比较两个文件
来源：http://mobile.epnwcf.com/Article/details/gjiwmfvdd.sHtML

diff a.txt b.txt
来源：http://wap.epnwcf.com/Article/details/guwqbplne.sHtML

[R55] 压缩与解压
来源：http://read.share.epnwcf.com/Article/details/gqiaekmsq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.sjlbkw.cn/Article/details/gqyhcictc.sHtML

[R56] 远程拷贝
来源：http://baike.tarul.cn/Article/details/geedpclql.sHtML

scp file user@host:/path/
来源：http://mobile.sjlbkw.cn/Article/details/gecmibtor.sHtML

[R57] 远程执行命令
来源：http://read.share.epnwcf.com/Article/details/gtzlupvny.sHtML

ssh user@host 'uptime'
来源：http://www.share.epnwcf.com/Article/details/gnutqeqfr.sHtML

[R58] 下载文件
来源：http://mobile.tarul.cn/Article/details/gnrqziwyu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.epnwcf.com/Article/details/gbclreboy.sHtML

[R59] 发 POST JSON
来源：http://www.share.epnwcf.com/Article/details/gdnyolytu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.yfazqb.com/Article/details/guaizjobm.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.epnwcf.com/Article/details/gahinzkje.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.bbcook.cn/Article/details/gzuxcqmlt.sHtML

[R61] 磁盘占用
来源：http://3g.epnwcf.com/Article/details/ggcclxwov.sHtML

df -h;  du -sh *
来源：http://blog.tarul.cn/Article/details/gemdeoxta.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.yfazqb.com/Article/details/gpitxnflc.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.epnwcf.com/Article/details/gwtwkontn.sHtML

[R63] 内存与进程
来源：http://baike.fktsv.cn/Article/details/gkfvkbjqc.sHtML


<!-- 参考信息 -->