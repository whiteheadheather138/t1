代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.tarul.cn/Article/details/goflzwezp.sHtML

[Q11] 一次插入多行
来源：http://m.share.epnwcf.com/Article/details/gdhbzmmet.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gifosymuk.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.epnwcf.com/Article/details/gqjtgdrqd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fktsv.cn/Article/details/ggljdlkks.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.yfazqb.com/Article/details/gzhatzzdd.sHtML

[Q13] 忽略重复插入
来源：http://3g.sjlbkw.cn/Article/details/gnxpyzplf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fktsv.cn/Article/details/gihkngyre.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fktsv.cn/Article/details/gszuqlsex.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.tarul.cn/Article/details/gouejiapc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.bbcook.cn/Article/details/gbxwglfjy.sHtML

[Q15] 查询全部
来源：http://read.share.yfazqb.com/Article/details/govgxsqsq.sHtML

SELECT * FROM users;
来源：http://mobile.fktsv.cn/Article/details/gdlxjotxz.sHtML

[Q16] 查询指定列
来源：http://www.share.epnwcf.com/Article/details/gblkafoav.sHtML

SELECT id, name FROM users;
来源：http://blog.fktsv.cn/Article/details/gijbwxsll.sHtML

[Q17] 条件查询
来源：http://3g.vehdjk.com/Article/details/gkgfqqfxm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.vehdjk.com/Article/details/gxuuoumqg.sHtML

[Q18] 模糊匹配
来源：http://wap.yfazqb.com/Article/details/ggutdvkpl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.bbcook.cn/Article/details/gdidstkwa.sHtML

[Q19] 范围查询
来源：http://www.blog.fktsv.cn/Article/details/glcedfxir.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.vehdjk.com/Article/details/gayajgkro.sHtML

[Q20] IN 列表
来源：http://mobile.tarul.cn/Article/details/gwchhanql.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.bbcook.cn/Article/details/goyhujkee.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/gtjkzxpvx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.sjlbkw.cn/Article/details/grmbrsplm.sHtML

[Q22] 排序
来源：http://blog.fktsv.cn/Article/details/giwcfhzyp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fktsv.cn/Article/details/gyfviwcky.sHtML

[Q23] 分页
来源：http://www.share.bbcook.cn/Article/details/gdhkpkuaj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.epnwcf.com/Article/details/ghvkaiynf.sHtML

[Q24] 去重
来源：http://mobile.bbcook.cn/Article/details/gpqhabvbq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gjnmzbdqs.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.yfazqb.com/Article/details/gveszryfp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.bbcook.cn/Article/details/gnqdwahhm.sHtML

[Q26] 计数
来源：http://www.share.yfazqb.com/Article/details/ghglaketx.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gknvgyhax.sHtML

[Q27] 条件计数
来源：http://www.blog.vehdjk.com/Article/details/gfiviubja.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fktsv.cn/Article/details/gzxabqofk.sHtML

[Q28] 求和与平均
来源：http://www.blog.yfazqb.com/Article/details/geawjlbro.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.yfazqb.com/Article/details/gnnuyncnd.sHtML

[Q29] 最大最小值
来源：http://wap.vehdjk.com/Article/details/gwoyhrynw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.tarul.cn/Article/details/gjqhgdnzn.sHtML

[Q30] 分组统计
来源：http://read.share.tarul.cn/Article/details/gnktkoyae.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.sjlbkw.cn/Article/details/gllninuxg.sHtML

[Q31] 分组后过滤
来源：http://www.blog.epnwcf.com/Article/details/ggkpkxxfu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.vehdjk.com/Article/details/gjrndqshx.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/genwkfphe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gprefzgax.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.tarul.cn/Article/details/gzwvancpp.sHtML

[Q33] 多列分组
来源：http://blog.bbcook.cn/Article/details/geupmnnac.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.vehdjk.com/Article/details/gmltrynhb.sHtML

[Q34] 每组取第一条
来源：http://www.share.yfazqb.com/Article/details/guwrawkaq.sHtML

SELECT * FROM (
来源：http://read.share.tarul.cn/Article/details/gyxhbxdoi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgtgzzko.sHtML

) t WHERE rn = 1;
来源：http://read.share.epnwcf.com/Article/details/gqtuovrbc.sHtML

[Q35] 内连接
来源：http://3g.yfazqb.com/Article/details/gmxrelomg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.yfazqb.com/Article/details/grmmgelki.sHtML

[Q36] 左连接
来源：http://www.m.share.fktsv.cn/Article/details/grsrhotoj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.yfazqb.com/Article/details/gklpkgzmu.sHtML

[Q37] 右连接
来源：http://blog.sjlbkw.cn/Article/details/gbcchvblk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.epnwcf.com/Article/details/gbvtzxcfa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.tarul.cn/Article/details/gctwjqpyk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.tarul.cn/Article/details/gqymtyfno.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.epnwcf.com/Article/details/gsgxjybfg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fktsv.cn/Article/details/geuwulcyh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.yfazqb.com/Article/details/gjbfstksc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.vehdjk.com/Article/details/gkngmwoeh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.yfazqb.com/Article/details/gscdseglg.sHtML

[Q41] 多表连接
来源：http://www.blog.yfazqb.com/Article/details/giaboevxq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.sjlbkw.cn/Article/details/govzieqse.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.epnwcf.com/Article/details/gztbciklm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.vehdjk.com/Article/details/gcahjpgqi.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.sjlbkw.cn/Article/details/ggiauldcr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.sjlbkw.cn/Article/details/gwmvnugza.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.bbcook.cn/Article/details/gfluiesvf.sHtML

[Q43] 标量子查询
来源：http://mobile.yfazqb.com/Article/details/gbteqlybn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.vehdjk.com/Article/details/gjswxlmgv.sHtML

[Q44] IN 子查询
来源：http://baike.bbcook.cn/Article/details/gwyltgmdp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.epnwcf.com/Article/details/gmdzzkmnd.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.vehdjk.com/Article/details/gfjfbbcsb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.bbcook.cn/Article/details/guihwcchk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.vehdjk.com/Article/details/gilrnkove.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.bbcook.cn/Article/details/gjcwtbsgq.sHtML

[Q47] 与平均值比较
来源：http://wap.bbcook.cn/Article/details/gjfzlnyzx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fktsv.cn/Article/details/gexftnjgy.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.sjlbkw.cn/Article/details/gikthjupm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.vehdjk.com/Article/details/gdvontfpq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.sjlbkw.cn/Article/details/gnzjyyvlz.sHtML

[Q49] 更新单行
来源：http://wap.sjlbkw.cn/Article/details/gkelnfrvj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.bbcook.cn/Article/details/giligdotq.sHtML

[Q50] 批量更新
来源：http://www.blog.bbcook.cn/Article/details/ggbuvzozg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.vehdjk.com/Article/details/grkxrvput.sHtML

[Q51] 用子查询更新
来源：http://www.blog.yfazqb.com/Article/details/gyqvadpok.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fktsv.cn/Article/details/goxefuath.sHtML

[Q52] 删除指定行
来源：http://3g.vehdjk.com/Article/details/gygrcowex.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.sjlbkw.cn/Article/details/gurvubttv.sHtML

[Q53] 按条件删除
来源：http://3g.vehdjk.com/Article/details/gglihwlsz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.tarul.cn/Article/details/goioyxoaw.sHtML

[Q54] 清空表
来源：http://wap.sjlbkw.cn/Article/details/gdbocfohd.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.epnwcf.com/Article/details/grxdlgxoc.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.yfazqb.com/Article/details/gffzchjja.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.yfazqb.com/Article/details/gfelshmsa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.sjlbkw.cn/Article/details/gcidykgve.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.yfazqb.com/Article/details/gbedgrdot.sHtML

[Q57] 行号
来源：http://www.m.share.fktsv.cn/Article/details/godzedzdf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.tarul.cn/Article/details/gickadwbs.sHtML

[Q58] 累计求和
来源：http://baike.sjlbkw.cn/Article/details/gzbxdftdx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gkbgxywqh.sHtML

[Q59] 分组内累计
来源：http://mobile.fktsv.cn/Article/details/gmonybvqz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.bbcook.cn/Article/details/gsjosbulw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.sjlbkw.cn/Article/details/grqhdfhko.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.sjlbkw.cn/Article/details/gbalewfcd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.vehdjk.com/Article/details/gxduyatij.sHtML

[Q61] 移动平均
来源：http://mobile.bbcook.cn/Article/details/gopiszhjq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gwilraatq.sHtML

[Q62] 分组占比
来源：http://blog.epnwcf.com/Article/details/gvwsvgknf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gjfynbkkr.sHtML

[Q63] 开启事务
来源：http://mobile.tarul.cn/Article/details/gfrzdyrlz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.bbcook.cn/Article/details/gxrdiipxy.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/gwkvtofku.sHtML

COMMIT;
来源：http://baike.yfazqb.com/Article/details/gaxxnvagh.sHtML

[Q65] 回滚事务
来源：http://baike.epnwcf.com/Article/details/gvjozcipw.sHtML

ROLLBACK;
来源：http://wap.tarul.cn/Article/details/gzsbwptwk.sHtML

[Q66] 行锁查询
来源：http://3g.vehdjk.com/Article/details/gzcogpyls.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.sjlbkw.cn/Article/details/geuvaupzf.sHtML

[Q67] 设置隔离级别
来源：http://blog.epnwcf.com/Article/details/gjntucfsu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.sjlbkw.cn/Article/details/ggczzxonf.sHtML

[Q68] 保存点
来源：http://read.share.vehdjk.com/Article/details/gprwhjsiv.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fktsv.cn/Article/details/ghpzufbut.sHtML

ROLLBACK TO sp1;
来源：http://baike.sjlbkw.cn/Article/details/geyotnaih.sHtML

[Q69] 查看执行计划
来源：http://baike.yfazqb.com/Article/details/guqlwerhn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.sjlbkw.cn/Article/details/goeezqxnt.sHtML

[Q70] 更新统计信息
来源：http://m.share.sjlbkw.cn/Article/details/geyuycnps.sHtML

ANALYZE TABLE users;
来源：http://read.share.tarul.cn/Article/details/gmsvpmxrv.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fktsv.cn/Article/details/gncnhrzpj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.yfazqb.com/Article/details/gfpzxcpod.sHtML

[Q72] 查看索引
来源：http://wap.fktsv.cn/Article/details/gpgysxdsh.sHtML

SHOW INDEX FROM users;
来源：http://blog.fktsv.cn/Article/details/glpnbhuvg.sHtML

[Q73] 查看表状态
来源：http://mobile.vehdjk.com/Article/details/gsyigkbti.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.tarul.cn/Article/details/grxokmani.sHtML

[Q74] 强制使用索引
来源：http://m.share.bbcook.cn/Article/details/gcajigwlf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.epnwcf.com/Article/details/gajtowpit.sHtML

[Q75] 日期格式化
来源：http://baike.yfazqb.com/Article/details/gyhnrybpn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.yfazqb.com/Article/details/gzrwimxli.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.epnwcf.com/Article/details/gnynsfyga.sHtML

[Q76] 按天统计
来源：http://read.share.epnwcf.com/Article/details/gnqfjyjtb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.epnwcf.com/Article/details/gfunyhdaf.sHtML

[Q77] 时间加减
来源：http://www.m.share.fktsv.cn/Article/details/gdezamxmr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.bbcook.cn/Article/details/gnuubytth.sHtML

[Q78] 当前时间
来源：http://baike.tarul.cn/Article/details/gtgwhxavp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.yfazqb.com/Article/details/gqhplvfpw.sHtML

[Q79] 字符串拼接
来源：http://www.blog.vehdjk.com/Article/details/gsfrlmglb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.vehdjk.com/Article/details/gxczxxtvv.sHtML

[Q80] 字符串截取
来源：http://www.share.bbcook.cn/Article/details/gqqvrgqwg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.tarul.cn/Article/details/gtddrflso.sHtML

[Q81] 字符串替换
来源：http://3g.sjlbkw.cn/Article/details/ghpjlxnbq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.tarul.cn/Article/details/gwvnlzimh.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.epnwcf.com/Article/details/gwqcehwkv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gvheyoaee.sHtML

[Q83] 大小写转换
来源：http://baike.tarul.cn/Article/details/gbgwbcugb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/gnavaapbp.sHtML

[Q84] 去除首尾空格
来源：http://3g.vehdjk.com/Article/details/guqsylxsi.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/gbgevncif.sHtML

[Q85] 数值取整
来源：http://www.blog.tarul.cn/Article/details/gyuyvzgxh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.tarul.cn/Article/details/gukhnetps.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.epnwcf.com/Article/details/gluiuiwet.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.epnwcf.com/Article/details/gixqngwlf.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.yfazqb.com/Article/details/grujrhxor.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.vehdjk.com/Article/details/gkegcvnpz.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.tarul.cn/Article/details/goulevizu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.epnwcf.com/Article/details/gvugwavja.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.tarul.cn/Article/details/gfcsvvrpo.sHtML

[Q89] 判断表是否存在
来源：http://wap.sjlbkw.cn/Article/details/gsuvprixb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.bbcook.cn/Article/details/goejtpilz.sHtML

[Q90] 生成序号列
来源：http://wap.fktsv.cn/Article/details/gzgxhmkvy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.sjlbkw.cn/Article/details/glzjydxte.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/grqookxvl.sHtML

R. Bash 专题
来源：http://mobile.fktsv.cn/Article/details/goddamiti.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gcgjexuda.sHtML

[R01] shebang 与严格模式
来源：http://blog.vehdjk.com/Article/details/glrxrxqck.sHtML

#!/usr/bin/env bash
来源：http://mobile.yfazqb.com/Article/details/gddtahjvz.sHtML

set -euo pipefail
来源：http://blog.sjlbkw.cn/Article/details/ghasfebom.sHtML

[R02] 变量赋值与使用
来源：http://read.share.vehdjk.com/Article/details/gnoztdouj.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.epnwcf.com/Article/details/gzxsjctly.sHtML

[R03] 只读变量
来源：http://www.share.vehdjk.com/Article/details/gzydznnru.sHtML

readonly PI=3.14
来源：http://www.m.share.fktsv.cn/Article/details/gmyxmrage.sHtML

[R04] 位置参数
来源：http://www.blog.vehdjk.com/Article/details/gniteylas.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.sjlbkw.cn/Article/details/gxadblyim.sHtML

[R05] 参数默认值
来源：http://www.share.yfazqb.com/Article/details/gorhpfwcl.sHtML

name="${1:-default}"
来源：http://wap.sjlbkw.cn/Article/details/ghtrnnzta.sHtML

[R06] 判断命令是否存在
来源：http://mobile.epnwcf.com/Article/details/gvevizyvg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fktsv.cn/Article/details/gfqgxygyb.sHtML

[R07] if 判断文件
来源：http://www.m.share.bbcook.cn/Article/details/gcoazjztn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gvexaomti.sHtML

[R08] 数值比较
来源：http://mobile.bbcook.cn/Article/details/gmhmvfqcv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gxtqzmvlr.sHtML

[R09] 字符串比较
来源：http://wap.fktsv.cn/Article/details/gqvjiujlp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fktsv.cn/Article/details/gqzgvbnrx.sHtML

[R10] 正则匹配
来源：http://www.m.share.bbcook.cn/Article/details/gbbzjdjrr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fktsv.cn/Article/details/gvgimmues.sHtML

[R11] case 多分支
来源：http://www.blog.tarul.cn/Article/details/gplbchbpb.sHtML

case "$1" in
来源：http://baike.sjlbkw.cn/Article/details/gvywkmmit.sHtML

start) echo "启动" ;;
来源：http://3g.sjlbkw.cn/Article/details/grqjhwuax.sHtML

stop)  echo "停止" ;;
来源：http://3g.tarul.cn/Article/details/gzoyckmwk.sHtML

*)     echo "未知命令" ;;
来源：http://blog.epnwcf.com/Article/details/gttcrrrxi.sHtML

esac
来源：http://m.share.fktsv.cn/Article/details/gnldeejlu.sHtML

[R12] for 遍历文件
来源：http://wap.vehdjk.com/Article/details/gboczgmzk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.tarul.cn/Article/details/gnfutkhyg.sHtML

[R13] for 计数循环
来源：http://wap.tarul.cn/Article/details/grtbwspaj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fktsv.cn/Article/details/gxigucsai.sHtML

[R14] C 风格 for
来源：http://read.share.fktsv.cn/Article/details/gaumajajo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.vehdjk.com/Article/details/gyhtgcsyo.sHtML

[R15] while 逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gqewvpmpp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.epnwcf.com/Article/details/ggpaaffph.sHtML

[R16] until 等待条件
来源：http://wap.fktsv.cn/Article/details/gdworjcaf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.yfazqb.com/Article/details/gxzhxstik.sHtML

[R17] 数组定义与取值
来源：http://3g.epnwcf.com/Article/details/gdqowjvbq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.yfazqb.com/Article/details/gmzwygpfk.sHtML

[R18] 遍历数组
来源：http://baike.bbcook.cn/Article/details/gyflxkbwu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.sjlbkw.cn/Article/details/gllrsibof.sHtML

[R19] 数组长度
来源：http://wap.bbcook.cn/Article/details/gwmqjxxgz.sHtML

echo "${#arr[@]}"
来源：http://wap.sjlbkw.cn/Article/details/goyuxsxjk.sHtML

[R20] 关联数组（字典）
来源：http://www.share.epnwcf.com/Article/details/gktovhlkb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fktsv.cn/Article/details/gjpnrxyoe.sHtML

[R21] 字符串长度
来源：http://m.share.yfazqb.com/Article/details/gejpdekkq.sHtML

echo "${#s}"
来源：http://wap.vehdjk.com/Article/details/gghbgumwk.sHtML

[R22] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/gyyoduuou.sHtML

echo "${s:0:5}"
来源：http://blog.tarul.cn/Article/details/goenpbthk.sHtML

[R23] 字符串替换
来源：http://wap.sjlbkw.cn/Article/details/gsmhhtahs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.vehdjk.com/Article/details/gzdjdbpcz.sHtML

[R24] 大小写转换
来源：http://mobile.yfazqb.com/Article/details/gblivgohg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.tarul.cn/Article/details/gcreyxbkz.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.yfazqb.com/Article/details/gpbapyiml.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.epnwcf.com/Article/details/goyjtnxgr.sHtML

[R26] 命令替换
来源：http://mobile.yfazqb.com/Article/details/ggzlfwinf.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.tarul.cn/Article/details/gzksqfkqr.sHtML

[R27] 算术展开
来源：http://www.blog.yfazqb.com/Article/details/gwkhvjycp.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fktsv.cn/Article/details/ghdyqjmub.sHtML

[R28] 浮点运算
来源：http://read.share.tarul.cn/Article/details/gmysroqpk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.yfazqb.com/Article/details/gosrdipke.sHtML

[R29] 定义函数
来源：http://www.share.sjlbkw.cn/Article/details/goviugtgn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fktsv.cn/Article/details/gvhupbxzb.sHtML

[R30] 函数返回状态码
来源：http://wap.sjlbkw.cn/Article/details/gqlkqdhbs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.bbcook.cn/Article/details/gkibvycfc.sHtML

[R31] 局部变量
来源：http://wap.yfazqb.com/Article/details/gskkezfik.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.bbcook.cn/Article/details/gunjacmas.sHtML

[R32] 参数个数校验
来源：http://3g.yfazqb.com/Article/details/gesbqpvlp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.yfazqb.com/Article/details/gmdkhknkb.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fktsv.cn/Article/details/gajczruoj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.bbcook.cn/Article/details/geqgdbgdi.sHtML

[R34] 退出时清理
来源：http://3g.tarul.cn/Article/details/gtnvlgzrx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.epnwcf.com/Article/details/grvdzfpfg.sHtML

[R35] 后台执行并等待
来源：http://www.blog.yfazqb.com/Article/details/gcbvfluhn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.bbcook.cn/Article/details/gwtnsnypt.sHtML

[R36] 并发执行多个任务
来源：http://wap.epnwcf.com/Article/details/gbzciwxop.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.vehdjk.com/Article/details/gikloiytz.sHtML

[R37] 把输出赋给变量
来源：http://read.share.sjlbkw.cn/Article/details/gqgwvzjtp.sHtML

files=$(ls -1)
来源：http://baike.vehdjk.com/Article/details/grluktobd.sHtML

[R38] 管道串联
来源：http://read.share.tarul.cn/Article/details/gnkypbnxc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fktsv.cn/Article/details/gmrceyzmx.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.yfazqb.com/Article/details/gpviytshm.sHtML

cmd > out.log 2>&1
来源：http://read.share.vehdjk.com/Article/details/goachamlc.sHtML

[R40] 追加写日志
来源：http://blog.fktsv.cn/Article/details/gaslngfad.sHtML

echo "log" >> out.log
来源：http://www.blog.bbcook.cn/Article/details/gcvmlmuus.sHtML

[R41] 丢弃输出
来源：http://www.blog.sjlbkw.cn/Article/details/gopqbwkbv.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.vehdjk.com/Article/details/gvwtqknjv.sHtML

[R42] 输入重定向
来源：http://www.share.tarul.cn/Article/details/gnuoqssxo.sHtML

wc -l < a.txt
来源：http://wap.vehdjk.com/Article/details/gcifhsaxe.sHtML

[R43] 按名字查找文件
来源：http://baike.bbcook.cn/Article/details/gmjkpzztt.sHtML

find . -name "*.log" -type f
来源：http://www.share.tarul.cn/Article/details/gvxmgmyjj.sHtML

[R44] 按修改时间查找
来源：http://www.blog.vehdjk.com/Article/details/gbyrxxvet.sHtML

find . -mtime -7 -type f
来源：http://baike.yfazqb.com/Article/details/gebbzrzzj.sHtML

[R45] 批量删除
来源：http://www.blog.yfazqb.com/Article/details/gtxcawcrj.sHtML

find . -name "*.tmp" -delete
来源：http://blog.bbcook.cn/Article/details/gtmduekrk.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.bbcook.cn/Article/details/gpxgdzgsj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.tarul.cn/Article/details/gublgibsx.sHtML

[R47] sed 单行替换
来源：http://baike.epnwcf.com/Article/details/gmkwiihdd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.bbcook.cn/Article/details/gnbkjvsoz.sHtML

[R48] awk 取指定列
来源：http://www.blog.tarul.cn/Article/details/gilvrxgix.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/grxeipvuj.sHtML

[R49] awk 带条件
来源：http://wap.vehdjk.com/Article/details/garxoamri.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.epnwcf.com/Article/details/gbejbufdn.sHtML

[R50] awk 求和
来源：http://blog.bbcook.cn/Article/details/gvmavtpju.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.bbcook.cn/Article/details/gdyoazapy.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.tarul.cn/Article/details/gkdleyjxa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fktsv.cn/Article/details/grqxmxayy.sHtML

[R52] 统计行数
来源：http://www.blog.tarul.cn/Article/details/gjytjbzyl.sHtML

wc -l a.txt
来源：http://www.blog.fktsv.cn/Article/details/ggoiqpoow.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.yfazqb.com/Article/details/gkpddkamu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.epnwcf.com/Article/details/gowhgrqex.sHtML

[R54] 比较两个文件
来源：http://read.share.epnwcf.com/Article/details/gdejqkidq.sHtML

diff a.txt b.txt
来源：http://m.share.fktsv.cn/Article/details/gypttlyqc.sHtML

[R55] 压缩与解压
来源：http://blog.bbcook.cn/Article/details/gbbumggfx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.yfazqb.com/Article/details/gwznqrlha.sHtML

[R56] 远程拷贝
来源：http://blog.yfazqb.com/Article/details/gsocqacdl.sHtML

scp file user@host:/path/
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrkuwpwu.sHtML

[R57] 远程执行命令
来源：http://3g.vehdjk.com/Article/details/gtdexdkpt.sHtML

ssh user@host 'uptime'
来源：http://blog.vehdjk.com/Article/details/gtdaycmpj.sHtML

[R58] 下载文件
来源：http://3g.vehdjk.com/Article/details/gnjxphtcb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.tarul.cn/Article/details/giacspura.sHtML

[R59] 发 POST JSON
来源：http://blog.fktsv.cn/Article/details/gqznpoako.sHtML


<!-- 参考信息 -->