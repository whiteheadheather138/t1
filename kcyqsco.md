代发 wailian999

);
来源：http://www.share.epnwcf.com/Article/details/gxnqpxyas.sHtML

[Q03] 增加列
来源：http://read.share.tarul.cn/Article/details/gaohybdai.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.bbcook.cn/Article/details/gfmvhapso.sHtML

[Q04] 修改列类型
来源：http://www.blog.vehdjk.com/Article/details/gkzvbapcp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.sjlbkw.cn/Article/details/genyuqaqy.sHtML

[Q05] 重命名列
来源：http://3g.yfazqb.com/Article/details/gdxdlsaku.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.tarul.cn/Article/details/goxsmnuhq.sHtML

[Q06] 删除列
来源：http://www.share.yfazqb.com/Article/details/gpyrtnboj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.epnwcf.com/Article/details/gemtvuoet.sHtML

[Q07] 删除表
来源：http://3g.epnwcf.com/Article/details/gzvfmabmt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.sjlbkw.cn/Article/details/gsqjmuogf.sHtML

[Q08] 创建普通索引
来源：http://read.share.tarul.cn/Article/details/gitpnavnz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.tarul.cn/Article/details/gmehhtemk.sHtML

[Q09] 创建唯一索引
来源：http://www.share.yfazqb.com/Article/details/gfznninzl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fktsv.cn/Article/details/gxqdfaznw.sHtML

[Q10] 插入单行
来源：http://mobile.bbcook.cn/Article/details/gjgavyotx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fktsv.cn/Article/details/gyfopyhgb.sHtML

[Q11] 一次插入多行
来源：http://m.share.tarul.cn/Article/details/gxczybvvq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/golyaxxer.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.bbcook.cn/Article/details/gvlufdsda.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fktsv.cn/Article/details/gokpofsbf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.bbcook.cn/Article/details/gltcitwhf.sHtML

[Q13] 忽略重复插入
来源：http://blog.fktsv.cn/Article/details/guofkocqu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.yfazqb.com/Article/details/gsbhxqigc.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.sjlbkw.cn/Article/details/guvgmmtwy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.epnwcf.com/Article/details/gyyxvrmij.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fktsv.cn/Article/details/gqyoumiip.sHtML

[Q15] 查询全部
来源：http://baike.tarul.cn/Article/details/gjrgsxwgk.sHtML

SELECT * FROM users;
来源：http://3g.tarul.cn/Article/details/glizffxpv.sHtML

[Q16] 查询指定列
来源：http://www.blog.epnwcf.com/Article/details/gdhoqixft.sHtML

SELECT id, name FROM users;
来源：http://mobile.yfazqb.com/Article/details/gkfosmcvb.sHtML

[Q17] 条件查询
来源：http://mobile.tarul.cn/Article/details/gfpccjjgi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.tarul.cn/Article/details/gvpaayowk.sHtML

[Q18] 模糊匹配
来源：http://baike.vehdjk.com/Article/details/gtahwwcig.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.sjlbkw.cn/Article/details/grrwmlqfr.sHtML

[Q19] 范围查询
来源：http://www.share.sjlbkw.cn/Article/details/grjihmdqt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.epnwcf.com/Article/details/gmhxdbuhp.sHtML

[Q20] IN 列表
来源：http://3g.fktsv.cn/Article/details/gerkjqwlz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.yfazqb.com/Article/details/gsgvocxpv.sHtML

[Q21] 空值判断
来源：http://baike.tarul.cn/Article/details/grcgtdkej.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.vehdjk.com/Article/details/guixjqmlt.sHtML

[Q22] 排序
来源：http://m.share.epnwcf.com/Article/details/glbqiwzjf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.vehdjk.com/Article/details/gtncojsje.sHtML

[Q23] 分页
来源：http://www.share.sjlbkw.cn/Article/details/gmajsoqyb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.vehdjk.com/Article/details/gqzkdpxjt.sHtML

[Q24] 去重
来源：http://www.share.bbcook.cn/Article/details/gagsvkylp.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.yfazqb.com/Article/details/gkkfrskjk.sHtML

[Q25] 只取前 N 条
来源：http://blog.tarul.cn/Article/details/gaamslvff.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.sjlbkw.cn/Article/details/gfqoeobqq.sHtML

[Q26] 计数
来源：http://wap.sjlbkw.cn/Article/details/gtizqrdmj.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.epnwcf.com/Article/details/grzsongft.sHtML

[Q27] 条件计数
来源：http://www.blog.sjlbkw.cn/Article/details/gorsmwmxf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.vehdjk.com/Article/details/gbvsfiskg.sHtML

[Q28] 求和与平均
来源：http://www.share.tarul.cn/Article/details/gitlegxod.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gpmawqbns.sHtML

[Q29] 最大最小值
来源：http://mobile.bbcook.cn/Article/details/ghshpgmwx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.bbcook.cn/Article/details/gfxxjjcgk.sHtML

[Q30] 分组统计
来源：http://m.share.tarul.cn/Article/details/gnmogtxei.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gvgzcvspl.sHtML

[Q31] 分组后过滤
来源：http://baike.bbcook.cn/Article/details/ggaptiaqt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.bbcook.cn/Article/details/giknccale.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.yfazqb.com/Article/details/gsirciuzx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/gdehafayj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.vehdjk.com/Article/details/gnxtmblwm.sHtML

[Q33] 多列分组
来源：http://www.share.vehdjk.com/Article/details/gnprrcaup.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.yfazqb.com/Article/details/gcwfqsyok.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.epnwcf.com/Article/details/grsnsggzr.sHtML

SELECT * FROM (
来源：http://mobile.yfazqb.com/Article/details/gryfcgrvz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.epnwcf.com/Article/details/gnivzvhwt.sHtML

) t WHERE rn = 1;
来源：http://wap.tarul.cn/Article/details/gpkzzqjgi.sHtML

[Q35] 内连接
来源：http://www.blog.fktsv.cn/Article/details/gurxywrme.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fktsv.cn/Article/details/gasltdauy.sHtML

[Q36] 左连接
来源：http://blog.yfazqb.com/Article/details/gjttmjspk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/glrmfnmij.sHtML

[Q37] 右连接
来源：http://m.share.sjlbkw.cn/Article/details/gkyrsmkop.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.tarul.cn/Article/details/gaoqjuasp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.sjlbkw.cn/Article/details/gdygielnk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.vehdjk.com/Article/details/godyfaylc.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.sjlbkw.cn/Article/details/gqeuihluw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.epnwcf.com/Article/details/gcnjnzhww.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.epnwcf.com/Article/details/gicbfddjy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fktsv.cn/Article/details/gzgsegfjx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.sjlbkw.cn/Article/details/gsmvuavuw.sHtML

[Q41] 多表连接
来源：http://www.share.tarul.cn/Article/details/gcumkkgro.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fktsv.cn/Article/details/groxcdgrd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.yfazqb.com/Article/details/gufansddz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.tarul.cn/Article/details/gkznuving.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.tarul.cn/Article/details/ghnkynaie.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fktsv.cn/Article/details/gyznlxwlj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.vehdjk.com/Article/details/gnstgnhny.sHtML

[Q43] 标量子查询
来源：http://wap.epnwcf.com/Article/details/gpvzavnin.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.sjlbkw.cn/Article/details/gaztujrld.sHtML

[Q44] IN 子查询
来源：http://3g.vehdjk.com/Article/details/grarspazz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fktsv.cn/Article/details/gauerhaiw.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.vehdjk.com/Article/details/gpduhlllc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/gekczxfth.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.epnwcf.com/Article/details/gzksubukn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fktsv.cn/Article/details/gnbnykzom.sHtML

[Q47] 与平均值比较
来源：http://read.share.sjlbkw.cn/Article/details/gxzurjlje.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.yfazqb.com/Article/details/gkxeuvoqi.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.sjlbkw.cn/Article/details/gqldnbjnc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.bbcook.cn/Article/details/gdznhxcwi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fktsv.cn/Article/details/gtoshlxvm.sHtML

[Q49] 更新单行
来源：http://baike.bbcook.cn/Article/details/gyenkoypg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/gcsbwybgs.sHtML

[Q50] 批量更新
来源：http://3g.fktsv.cn/Article/details/glljsoyuj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.sjlbkw.cn/Article/details/guthkqwot.sHtML

[Q51] 用子查询更新
来源：http://www.blog.bbcook.cn/Article/details/grdcfbrah.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.bbcook.cn/Article/details/gcckjbsaa.sHtML

[Q52] 删除指定行
来源：http://www.blog.fktsv.cn/Article/details/gcadoooih.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gtfdwekue.sHtML

[Q53] 按条件删除
来源：http://wap.fktsv.cn/Article/details/gehbtykjc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fktsv.cn/Article/details/gqyzsdksm.sHtML

[Q54] 清空表
来源：http://www.blog.tarul.cn/Article/details/gieivvfkc.sHtML

TRUNCATE TABLE logs;
来源：http://blog.bbcook.cn/Article/details/gbgsmszdu.sHtML

[Q55] 排名（并列占位）
来源：http://3g.tarul.cn/Article/details/gdtzzphtk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fktsv.cn/Article/details/gfpwmuggx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.vehdjk.com/Article/details/goaowdeaj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.sjlbkw.cn/Article/details/gdyqmtwza.sHtML

[Q57] 行号
来源：http://baike.bbcook.cn/Article/details/gnxbiuqjg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.sjlbkw.cn/Article/details/ggamuvgse.sHtML

[Q58] 累计求和
来源：http://read.share.vehdjk.com/Article/details/glheaxvtj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gzewwmptv.sHtML

[Q59] 分组内累计
来源：http://wap.fktsv.cn/Article/details/gduddagcz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.bbcook.cn/Article/details/ggsbsugsx.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.bbcook.cn/Article/details/gkneblnac.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.epnwcf.com/Article/details/gjmfmzglp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gdjxwgrso.sHtML

[Q61] 移动平均
来源：http://baike.epnwcf.com/Article/details/gjzgtxkzx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.tarul.cn/Article/details/gwlozjkrp.sHtML

[Q62] 分组占比
来源：http://read.share.bbcook.cn/Article/details/giegrgulk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.sjlbkw.cn/Article/details/gfiruaary.sHtML

[Q63] 开启事务
来源：http://3g.vehdjk.com/Article/details/gsnfccont.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.yfazqb.com/Article/details/ghzvxjxxb.sHtML

[Q64] 提交事务
来源：http://read.share.yfazqb.com/Article/details/ggyzflkxc.sHtML

COMMIT;
来源：http://www.share.fktsv.cn/Article/details/gwoofivpj.sHtML

[Q65] 回滚事务
来源：http://3g.epnwcf.com/Article/details/gdxilxgin.sHtML

ROLLBACK;
来源：http://3g.bbcook.cn/Article/details/gsxabhbqb.sHtML

[Q66] 行锁查询
来源：http://read.share.vehdjk.com/Article/details/gxzysnoyb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.epnwcf.com/Article/details/gmmtqfqce.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fktsv.cn/Article/details/gnkqkobyy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.vehdjk.com/Article/details/gzcbchmaw.sHtML

[Q68] 保存点
来源：http://mobile.vehdjk.com/Article/details/grzyxqqqc.sHtML

SAVEPOINT sp1;
来源：http://blog.tarul.cn/Article/details/gegdoxegg.sHtML

ROLLBACK TO sp1;
来源：http://baike.bbcook.cn/Article/details/ganijcwhv.sHtML

[Q69] 查看执行计划
来源：http://baike.sjlbkw.cn/Article/details/gpyubkrga.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.bbcook.cn/Article/details/ggyzkgpev.sHtML

[Q70] 更新统计信息
来源：http://wap.yfazqb.com/Article/details/gczvrddfb.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.vehdjk.com/Article/details/gmsfnegvf.sHtML

[Q71] 查看建表语句
来源：http://m.share.tarul.cn/Article/details/gatsqbtue.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.vehdjk.com/Article/details/gyioizzvz.sHtML

[Q72] 查看索引
来源：http://www.share.tarul.cn/Article/details/gqnooyirf.sHtML

SHOW INDEX FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gvvawvrfp.sHtML

[Q73] 查看表状态
来源：http://baike.bbcook.cn/Article/details/gdrjygxeo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.yfazqb.com/Article/details/gxmqbwugj.sHtML

[Q74] 强制使用索引
来源：http://read.share.vehdjk.com/Article/details/gdanlxtba.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.vehdjk.com/Article/details/getfnwrzy.sHtML

[Q75] 日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gqdwmhzvf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gsoxtqeie.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.bbcook.cn/Article/details/gmfwfihoa.sHtML

[Q76] 按天统计
来源：http://baike.sjlbkw.cn/Article/details/gajaatnto.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.yfazqb.com/Article/details/gxiwmhdjs.sHtML

[Q77] 时间加减
来源：http://blog.fktsv.cn/Article/details/grqkyuqgs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.tarul.cn/Article/details/gjpvlfits.sHtML

[Q78] 当前时间
来源：http://read.share.bbcook.cn/Article/details/glzbqcprk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.bbcook.cn/Article/details/gmrnjzagr.sHtML

[Q79] 字符串拼接
来源：http://3g.bbcook.cn/Article/details/gqwjbopth.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.tarul.cn/Article/details/gpjfisrkj.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fktsv.cn/Article/details/glanszvvs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/glpttsnuc.sHtML

[Q81] 字符串替换
来源：http://www.share.sjlbkw.cn/Article/details/gybbbnzaq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gtglywupr.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.tarul.cn/Article/details/gprdcciev.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gnogbgbun.sHtML

[Q83] 大小写转换
来源：http://baike.epnwcf.com/Article/details/gvyafdwum.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/ghnxjxgtl.sHtML

[Q84] 去除首尾空格
来源：http://m.share.bbcook.cn/Article/details/gqvoxpkjy.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gvdvecdey.sHtML

[Q85] 数值取整
来源：http://mobile.tarul.cn/Article/details/gtdgbqxbi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.vehdjk.com/Article/details/gzfddtgnc.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fktsv.cn/Article/details/grswpzqqk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.vehdjk.com/Article/details/gvxblbtoo.sHtML

[Q87] JSON 字段做条件
来源：http://blog.vehdjk.com/Article/details/gcxazdqzb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.tarul.cn/Article/details/gemfaubow.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.bbcook.cn/Article/details/grizdjrah.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.bbcook.cn/Article/details/gwdxbepdh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fktsv.cn/Article/details/ghvyfgepd.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.tarul.cn/Article/details/gcvmugxpj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.vehdjk.com/Article/details/gejeiowsh.sHtML

[Q90] 生成序号列
来源：http://read.share.bbcook.cn/Article/details/glnyubqya.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.sjlbkw.cn/Article/details/gkqrwmwnu.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gkdwqqtlp.sHtML

R. Bash 专题
来源：http://www.share.vehdjk.com/Article/details/gpyfeukyo.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gsggdmgnx.sHtML

[R01] shebang 与严格模式
来源：http://baike.yfazqb.com/Article/details/getgcnytn.sHtML

#!/usr/bin/env bash
来源：http://m.share.yfazqb.com/Article/details/gkcvmuwky.sHtML

set -euo pipefail
来源：http://3g.yfazqb.com/Article/details/guqvlnqcf.sHtML

[R02] 变量赋值与使用
来源：http://wap.sjlbkw.cn/Article/details/gpylxhtst.sHtML

name="Tom"; echo "$name"
来源：http://wap.epnwcf.com/Article/details/ganjtohol.sHtML

[R03] 只读变量
来源：http://blog.fktsv.cn/Article/details/gtkrxadsp.sHtML

readonly PI=3.14
来源：http://blog.epnwcf.com/Article/details/glinzmdxr.sHtML

[R04] 位置参数
来源：http://www.m.share.bbcook.cn/Article/details/gtnaxffev.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.epnwcf.com/Article/details/glwjvvlop.sHtML

[R05] 参数默认值
来源：http://read.share.tarul.cn/Article/details/grmaddbin.sHtML

name="${1:-default}"
来源：http://www.blog.fktsv.cn/Article/details/gfvpkqqtk.sHtML

[R06] 判断命令是否存在
来源：http://wap.bbcook.cn/Article/details/gblhtcydz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.tarul.cn/Article/details/gdahekmoo.sHtML

[R07] if 判断文件
来源：http://3g.yfazqb.com/Article/details/gwtljqwam.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.vehdjk.com/Article/details/goikvzbbw.sHtML

[R08] 数值比较
来源：http://baike.sjlbkw.cn/Article/details/ggnmegkjd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.vehdjk.com/Article/details/gvqsmtzom.sHtML

[R09] 字符串比较
来源：http://m.share.fktsv.cn/Article/details/giksobaiw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.yfazqb.com/Article/details/geuisldxy.sHtML

[R10] 正则匹配
来源：http://m.share.tarul.cn/Article/details/ggiprqgny.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gfvtlxbtf.sHtML

[R11] case 多分支
来源：http://wap.tarul.cn/Article/details/gasywpjxp.sHtML

case "$1" in
来源：http://wap.yfazqb.com/Article/details/gftmzzuql.sHtML

start) echo "启动" ;;
来源：http://mobile.sjlbkw.cn/Article/details/gjuxtldbl.sHtML

stop)  echo "停止" ;;
来源：http://3g.sjlbkw.cn/Article/details/gyhfmwrkt.sHtML

*)     echo "未知命令" ;;
来源：http://baike.yfazqb.com/Article/details/gnsqekpao.sHtML

esac
来源：http://www.m.share.vehdjk.com/Article/details/glgevkcyx.sHtML

[R12] for 遍历文件
来源：http://baike.vehdjk.com/Article/details/glhcmkitp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.sjlbkw.cn/Article/details/grbgbkcca.sHtML

[R13] for 计数循环
来源：http://baike.tarul.cn/Article/details/gxxjusrmb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.tarul.cn/Article/details/gliegtvoh.sHtML

[R14] C 风格 for
来源：http://www.share.vehdjk.com/Article/details/gpjodhoxb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.bbcook.cn/Article/details/gnhjhzbyb.sHtML

[R15] while 逐行读文件
来源：http://baike.bbcook.cn/Article/details/geftakzjw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.bbcook.cn/Article/details/gaatubila.sHtML

[R16] until 等待条件
来源：http://3g.vehdjk.com/Article/details/golcbhfnd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/gtssrywfe.sHtML

[R17] 数组定义与取值
来源：http://read.share.tarul.cn/Article/details/ghpiukfpp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.yfazqb.com/Article/details/gmichqnmt.sHtML

[R18] 遍历数组
来源：http://3g.epnwcf.com/Article/details/gvcechisq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.epnwcf.com/Article/details/gjmbrkntj.sHtML

[R19] 数组长度
来源：http://baike.vehdjk.com/Article/details/guangwqcz.sHtML

echo "${#arr[@]}"
来源：http://read.share.bbcook.cn/Article/details/glloaappd.sHtML

[R20] 关联数组（字典）
来源：http://read.share.yfazqb.com/Article/details/gjvaxgesm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.sjlbkw.cn/Article/details/grihnxvrn.sHtML

[R21] 字符串长度
来源：http://wap.vehdjk.com/Article/details/gvpgacwmt.sHtML

echo "${#s}"
来源：http://baike.sjlbkw.cn/Article/details/gcoarbymv.sHtML

[R22] 截取子串
来源：http://mobile.fktsv.cn/Article/details/gzyruwolf.sHtML

echo "${s:0:5}"
来源：http://mobile.epnwcf.com/Article/details/gvtfbmplr.sHtML

[R23] 字符串替换
来源：http://blog.tarul.cn/Article/details/gsmbhqryb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.sjlbkw.cn/Article/details/gkduqmwhg.sHtML

[R24] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/grcdjhboh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.tarul.cn/Article/details/gocdsdbrf.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.sjlbkw.cn/Article/details/grawacuph.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.vehdjk.com/Article/details/gbhjjsuyk.sHtML

[R26] 命令替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gntspgqsy.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fktsv.cn/Article/details/gbqyucwoa.sHtML

[R27] 算术展开
来源：http://mobile.epnwcf.com/Article/details/ghfajhbkh.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.yfazqb.com/Article/details/gshrqxtqy.sHtML

[R28] 浮点运算
来源：http://baike.epnwcf.com/Article/details/gejmfglui.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.sjlbkw.cn/Article/details/gmpcoykpl.sHtML

[R29] 定义函数
来源：http://m.share.yfazqb.com/Article/details/gagogzskb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fktsv.cn/Article/details/gqlzrddbf.sHtML

[R30] 函数返回状态码
来源：http://www.blog.bbcook.cn/Article/details/gjnsgsvht.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.epnwcf.com/Article/details/goqvassuk.sHtML

[R31] 局部变量
来源：http://www.m.share.yfazqb.com/Article/details/gxlkumgob.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.sjlbkw.cn/Article/details/gcdltpyyj.sHtML

[R32] 参数个数校验
来源：http://www.blog.sjlbkw.cn/Article/details/gwbetywxn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.tarul.cn/Article/details/geisczpac.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.vehdjk.com/Article/details/grrnypxmt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.vehdjk.com/Article/details/gxrjykeht.sHtML

[R34] 退出时清理
来源：http://www.share.tarul.cn/Article/details/goloorjzg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gmodtgnsw.sHtML

[R35] 后台执行并等待
来源：http://read.share.vehdjk.com/Article/details/gjfmzlegw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.bbcook.cn/Article/details/grwahuvfs.sHtML

[R36] 并发执行多个任务
来源：http://blog.epnwcf.com/Article/details/gbxasvemu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.vehdjk.com/Article/details/gaddxzjyg.sHtML

[R37] 把输出赋给变量
来源：http://mobile.yfazqb.com/Article/details/gyoilildz.sHtML

files=$(ls -1)
来源：http://mobile.bbcook.cn/Article/details/gpbiwfllg.sHtML

[R38] 管道串联
来源：http://mobile.tarul.cn/Article/details/gsrvlwdir.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.sjlbkw.cn/Article/details/guzwdsrcd.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.tarul.cn/Article/details/gbkfrremh.sHtML

cmd > out.log 2>&1
来源：http://blog.sjlbkw.cn/Article/details/gwsizkotb.sHtML

[R40] 追加写日志
来源：http://mobile.tarul.cn/Article/details/gvolxleds.sHtML

echo "log" >> out.log
来源：http://www.blog.tarul.cn/Article/details/gpjytfqvj.sHtML

[R41] 丢弃输出
来源：http://www.share.tarul.cn/Article/details/giyjbhnpt.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.epnwcf.com/Article/details/gyrfuaagg.sHtML

[R42] 输入重定向
来源：http://www.blog.fktsv.cn/Article/details/gzovxqksp.sHtML

wc -l < a.txt
来源：http://m.share.yfazqb.com/Article/details/gosrvuyxr.sHtML

[R43] 按名字查找文件
来源：http://www.blog.tarul.cn/Article/details/geqjcfwlt.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.epnwcf.com/Article/details/guuoaalvl.sHtML

[R44] 按修改时间查找
来源：http://www.blog.sjlbkw.cn/Article/details/gmfbuxonb.sHtML

find . -mtime -7 -type f
来源：http://www.share.bbcook.cn/Article/details/gpauvtjft.sHtML

[R45] 批量删除
来源：http://www.m.share.epnwcf.com/Article/details/gvpbpvhtq.sHtML

find . -name "*.tmp" -delete
来源：http://blog.epnwcf.com/Article/details/gylmgkknh.sHtML

[R46] 递归替换文件内容
来源：http://www.share.sjlbkw.cn/Article/details/gcjibnrqo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.yfazqb.com/Article/details/gvhwaxfsl.sHtML

[R47] sed 单行替换
来源：http://baike.bbcook.cn/Article/details/gadjzzbps.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.vehdjk.com/Article/details/gvpnbauqa.sHtML

[R48] awk 取指定列
来源：http://read.share.yfazqb.com/Article/details/gppvwcgwi.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.sjlbkw.cn/Article/details/gocqrilch.sHtML

[R49] awk 带条件
来源：http://www.blog.tarul.cn/Article/details/gttuntfjy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.epnwcf.com/Article/details/grrqftnwq.sHtML

[R50] awk 求和
来源：http://blog.yfazqb.com/Article/details/gnpgaeliv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.sjlbkw.cn/Article/details/gttrzicvb.sHtML

[R51] 排序去重取前几
来源：http://read.share.yfazqb.com/Article/details/gbbzdoeen.sHtML


<!-- 参考信息 -->