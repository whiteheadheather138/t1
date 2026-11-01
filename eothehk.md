代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.tarul.cn/Article/details/grpjyavao.sHtML

user_id INT NOT NULL,
来源：http://read.share.fktsv.cn/Article/details/gudciaqrq.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.bbcook.cn/Article/details/gkayssyzw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.vehdjk.com/Article/details/gmameojmq.sHtML

);
来源：http://www.blog.epnwcf.com/Article/details/gbdnfhvrv.sHtML

[Q03] 增加列
来源：http://www.share.vehdjk.com/Article/details/gucomchsh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.epnwcf.com/Article/details/glqthvnvc.sHtML

[Q04] 修改列类型
来源：http://mobile.sjlbkw.cn/Article/details/ghinauyvf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.bbcook.cn/Article/details/gocvuasyk.sHtML

[Q05] 重命名列
来源：http://blog.vehdjk.com/Article/details/gsscvxihb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.yfazqb.com/Article/details/gbsntdllj.sHtML

[Q06] 删除列
来源：http://www.m.share.tarul.cn/Article/details/gplfuglqq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.epnwcf.com/Article/details/gsiugknfe.sHtML

[Q07] 删除表
来源：http://baike.tarul.cn/Article/details/gnnyoevvr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.yfazqb.com/Article/details/gnolytpvi.sHtML

[Q08] 创建普通索引
来源：http://mobile.bbcook.cn/Article/details/gvvpzyvte.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.sjlbkw.cn/Article/details/gfahwxonx.sHtML

[Q09] 创建唯一索引
来源：http://wap.bbcook.cn/Article/details/gxcsljtqo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.vehdjk.com/Article/details/gtzjbkvxr.sHtML

[Q10] 插入单行
来源：http://mobile.sjlbkw.cn/Article/details/gweiyoqzs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.tarul.cn/Article/details/gajcmwefm.sHtML

[Q11] 一次插入多行
来源：http://read.share.tarul.cn/Article/details/gpiemcmpe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.yfazqb.com/Article/details/gzaojbzfl.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.epnwcf.com/Article/details/gjdfjceac.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.epnwcf.com/Article/details/gkqvxobak.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.yfazqb.com/Article/details/gwyjdngnm.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fktsv.cn/Article/details/grjnpfjyk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.vehdjk.com/Article/details/geseyvivt.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.yfazqb.com/Article/details/gusrkinwn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fktsv.cn/Article/details/gwvvejvce.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.yfazqb.com/Article/details/gvvkmmmnp.sHtML

[Q15] 查询全部
来源：http://read.share.fktsv.cn/Article/details/gmldackis.sHtML

SELECT * FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/grmoxstce.sHtML

[Q16] 查询指定列
来源：http://www.share.tarul.cn/Article/details/gzgsvkmdo.sHtML

SELECT id, name FROM users;
来源：http://m.share.bbcook.cn/Article/details/gshimgalh.sHtML

[Q17] 条件查询
来源：http://3g.tarul.cn/Article/details/guqgsjsnx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.tarul.cn/Article/details/ggbjqxqhr.sHtML

[Q18] 模糊匹配
来源：http://3g.tarul.cn/Article/details/grqgohtkc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.epnwcf.com/Article/details/ghxbklvur.sHtML

[Q19] 范围查询
来源：http://www.m.share.vehdjk.com/Article/details/gktpgbwxk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.epnwcf.com/Article/details/grfrcgomk.sHtML

[Q20] IN 列表
来源：http://mobile.vehdjk.com/Article/details/gwwlgpauv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.vehdjk.com/Article/details/gpznmekyr.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/gcmverfif.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.yfazqb.com/Article/details/gmprgmkhv.sHtML

[Q22] 排序
来源：http://baike.bbcook.cn/Article/details/ghsumqqdx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.bbcook.cn/Article/details/gclggldvh.sHtML

[Q23] 分页
来源：http://m.share.sjlbkw.cn/Article/details/govdqbdwv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.vehdjk.com/Article/details/gkclrfxcl.sHtML

[Q24] 去重
来源：http://www.blog.bbcook.cn/Article/details/glylftnce.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.vehdjk.com/Article/details/glywdfvgh.sHtML

[Q25] 只取前 N 条
来源：http://www.share.sjlbkw.cn/Article/details/gkncmtfsg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.yfazqb.com/Article/details/gjpbzzvtt.sHtML

[Q26] 计数
来源：http://www.share.epnwcf.com/Article/details/gedfuztak.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gaqessxvm.sHtML

[Q27] 条件计数
来源：http://www.share.yfazqb.com/Article/details/ghhfvaoou.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gkcdbbnht.sHtML

[Q28] 求和与平均
来源：http://www.share.vehdjk.com/Article/details/gxhhwqmwl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.tarul.cn/Article/details/gnixhwgom.sHtML

[Q29] 最大最小值
来源：http://3g.bbcook.cn/Article/details/gcqlddkus.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.tarul.cn/Article/details/gzqzbkohr.sHtML

[Q30] 分组统计
来源：http://wap.epnwcf.com/Article/details/getgyqfoa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gahlgnqya.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fktsv.cn/Article/details/ggzjuqfso.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.tarul.cn/Article/details/gcenrrgey.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gdyzclttj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/guyphpnve.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.bbcook.cn/Article/details/gfhhqntwp.sHtML

[Q33] 多列分组
来源：http://3g.tarul.cn/Article/details/gumavzhbb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.epnwcf.com/Article/details/gtbepcfdn.sHtML

[Q34] 每组取第一条
来源：http://mobile.fktsv.cn/Article/details/gcvwruupb.sHtML

SELECT * FROM (
来源：http://mobile.tarul.cn/Article/details/gwaqsglgp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.yfazqb.com/Article/details/goclxgbol.sHtML

) t WHERE rn = 1;
来源：http://blog.epnwcf.com/Article/details/gkvfkxblz.sHtML

[Q35] 内连接
来源：http://mobile.yfazqb.com/Article/details/gufxmusdk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.bbcook.cn/Article/details/ghmfilctd.sHtML

[Q36] 左连接
来源：http://read.share.vehdjk.com/Article/details/gychyieuk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/gsfwodnrn.sHtML

[Q37] 右连接
来源：http://3g.epnwcf.com/Article/details/gaazifbky.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fktsv.cn/Article/details/gqsbgrgkm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.yfazqb.com/Article/details/gzerfbekj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.yfazqb.com/Article/details/gcbhrshhj.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.tarul.cn/Article/details/ghegalhcn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.epnwcf.com/Article/details/ggxfawbyj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.sjlbkw.cn/Article/details/gjdfffmdn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.bbcook.cn/Article/details/ggwehwavy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.sjlbkw.cn/Article/details/gzgsojklq.sHtML

[Q41] 多表连接
来源：http://read.share.tarul.cn/Article/details/gqovwxrwr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.tarul.cn/Article/details/gammtlklh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.yfazqb.com/Article/details/gfrezxkmq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.sjlbkw.cn/Article/details/gsljassac.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fktsv.cn/Article/details/gwsgsjglz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.yfazqb.com/Article/details/gfsdvvkpa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.tarul.cn/Article/details/ghbuplsbs.sHtML

[Q43] 标量子查询
来源：http://www.blog.tarul.cn/Article/details/gkhpopeko.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.bbcook.cn/Article/details/gjdnbeadl.sHtML

[Q44] IN 子查询
来源：http://blog.fktsv.cn/Article/details/gvrnjttyz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.tarul.cn/Article/details/gokjuhvdo.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.tarul.cn/Article/details/gmuriuvmc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.sjlbkw.cn/Article/details/gduxroplo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.vehdjk.com/Article/details/gvwsjhovk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.bbcook.cn/Article/details/ggtzfwgkh.sHtML

[Q47] 与平均值比较
来源：http://read.share.bbcook.cn/Article/details/gpbjhlglq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.vehdjk.com/Article/details/gezovhwxy.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.sjlbkw.cn/Article/details/gzjatmygg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.vehdjk.com/Article/details/gdstfaaxl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.epnwcf.com/Article/details/gfrlfajiw.sHtML

[Q49] 更新单行
来源：http://3g.sjlbkw.cn/Article/details/gfknxpedd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fktsv.cn/Article/details/gdqwnhmqv.sHtML

[Q50] 批量更新
来源：http://read.share.yfazqb.com/Article/details/gfvoyehij.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.tarul.cn/Article/details/gtavuuwjz.sHtML

[Q51] 用子查询更新
来源：http://blog.bbcook.cn/Article/details/gvbcylbvw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.tarul.cn/Article/details/gswyokbsz.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fktsv.cn/Article/details/gpmgbnncw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.tarul.cn/Article/details/gearbafhs.sHtML

[Q53] 按条件删除
来源：http://3g.yfazqb.com/Article/details/gvuitfgcr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.epnwcf.com/Article/details/grnnfrzzi.sHtML

[Q54] 清空表
来源：http://read.share.tarul.cn/Article/details/gplucetij.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.tarul.cn/Article/details/gjotrkift.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fktsv.cn/Article/details/gwsheqawp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.tarul.cn/Article/details/gysoifdta.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.sjlbkw.cn/Article/details/gbjqylzyt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.vehdjk.com/Article/details/gpdxsnchl.sHtML

[Q57] 行号
来源：http://m.share.fktsv.cn/Article/details/gqcuvgffy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.yfazqb.com/Article/details/gmizbeexl.sHtML

[Q58] 累计求和
来源：http://m.share.fktsv.cn/Article/details/gcfeoyoec.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.tarul.cn/Article/details/gwinjyqss.sHtML

[Q59] 分组内累计
来源：http://www.share.vehdjk.com/Article/details/gcwkajmem.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/guaoyvumb.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.epnwcf.com/Article/details/garzwfqtz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.sjlbkw.cn/Article/details/gyhfqbros.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gmlsveoqe.sHtML

[Q61] 移动平均
来源：http://blog.vehdjk.com/Article/details/gdsjuqizn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gsxryioxb.sHtML

[Q62] 分组占比
来源：http://wap.vehdjk.com/Article/details/gepxvgmst.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/guhuelmoe.sHtML

[Q63] 开启事务
来源：http://blog.epnwcf.com/Article/details/ggpzwhkto.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.vehdjk.com/Article/details/glduqbewx.sHtML

[Q64] 提交事务
来源：http://baike.bbcook.cn/Article/details/gejabhqtb.sHtML

COMMIT;
来源：http://blog.bbcook.cn/Article/details/gttiyaboj.sHtML

[Q65] 回滚事务
来源：http://www.m.share.yfazqb.com/Article/details/gctptdplz.sHtML

ROLLBACK;
来源：http://read.share.yfazqb.com/Article/details/gluoskvzu.sHtML

[Q66] 行锁查询
来源：http://www.share.yfazqb.com/Article/details/grcktjexd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.epnwcf.com/Article/details/ghnilwgfk.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.sjlbkw.cn/Article/details/gvbxpkggq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.sjlbkw.cn/Article/details/gpxnagmfh.sHtML

[Q68] 保存点
来源：http://wap.yfazqb.com/Article/details/gjsvrpzyn.sHtML

SAVEPOINT sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/gsrghijnv.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.vehdjk.com/Article/details/gmmyhjecp.sHtML

[Q69] 查看执行计划
来源：http://read.share.epnwcf.com/Article/details/gopeprtvu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.sjlbkw.cn/Article/details/gdtmvlyjf.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fktsv.cn/Article/details/gmniveils.sHtML

ANALYZE TABLE users;
来源：http://3g.epnwcf.com/Article/details/gdjwhrndb.sHtML

[Q71] 查看建表语句
来源：http://3g.yfazqb.com/Article/details/gwkxdzfnb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fktsv.cn/Article/details/gfsjwvdhn.sHtML

[Q72] 查看索引
来源：http://m.share.vehdjk.com/Article/details/gbostzqmz.sHtML

SHOW INDEX FROM users;
来源：http://m.share.bbcook.cn/Article/details/gxwnyzcbo.sHtML

[Q73] 查看表状态
来源：http://www.m.share.vehdjk.com/Article/details/gvvemruvp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.vehdjk.com/Article/details/gqjdlfbnb.sHtML

[Q74] 强制使用索引
来源：http://baike.yfazqb.com/Article/details/gxtnkiuux.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.yfazqb.com/Article/details/gnyemtgfa.sHtML

[Q75] 日期格式化
来源：http://www.share.yfazqb.com/Article/details/gkfhrklpv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.bbcook.cn/Article/details/gqffbrgwv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.tarul.cn/Article/details/gsvzsswzg.sHtML

[Q76] 按天统计
来源：http://wap.bbcook.cn/Article/details/gjizsxubq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.epnwcf.com/Article/details/gfdlxklhr.sHtML

[Q77] 时间加减
来源：http://read.share.sjlbkw.cn/Article/details/gnfunnpdr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.bbcook.cn/Article/details/gxdojwazm.sHtML

[Q78] 当前时间
来源：http://baike.epnwcf.com/Article/details/gdmkcudkv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.bbcook.cn/Article/details/gxuezgoqa.sHtML

[Q79] 字符串拼接
来源：http://wap.tarul.cn/Article/details/gcuakalcu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.epnwcf.com/Article/details/gudtnfhth.sHtML

[Q80] 字符串截取
来源：http://www.share.bbcook.cn/Article/details/glvgrsjxk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gfvdyhsyu.sHtML

[Q81] 字符串替换
来源：http://m.share.fktsv.cn/Article/details/ghvkzopgb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.bbcook.cn/Article/details/gzphjlvve.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.tarul.cn/Article/details/gvvjbdugo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gzffszsni.sHtML

[Q83] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/giknypsas.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gifrjtzfe.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fktsv.cn/Article/details/gscnifpie.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gfxteschk.sHtML

[Q85] 数值取整
来源：http://blog.vehdjk.com/Article/details/gdoggtoxg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.bbcook.cn/Article/details/gkhxfjqel.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.yfazqb.com/Article/details/gxfklfybx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fktsv.cn/Article/details/gwtjjfimb.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.bbcook.cn/Article/details/gdfxrugmk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.bbcook.cn/Article/details/gyydfroha.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.sjlbkw.cn/Article/details/gzbuikgdn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.tarul.cn/Article/details/gilbfbris.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gooeuqmvn.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.bbcook.cn/Article/details/gmkcqakzx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.epnwcf.com/Article/details/gyyjiauqc.sHtML

[Q90] 生成序号列
来源：http://wap.bbcook.cn/Article/details/gjtyvgczd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.yfazqb.com/Article/details/gekxqzszw.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gyqprxgtb.sHtML

R. Bash 专题
来源：http://wap.epnwcf.com/Article/details/gtkiyqmiu.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gihzlcqyj.sHtML

[R01] shebang 与严格模式
来源：http://m.share.sjlbkw.cn/Article/details/ghhdymacp.sHtML

#!/usr/bin/env bash
来源：http://read.share.tarul.cn/Article/details/gdtlyqlen.sHtML

set -euo pipefail
来源：http://www.share.yfazqb.com/Article/details/gxhxosxux.sHtML

[R02] 变量赋值与使用
来源：http://blog.vehdjk.com/Article/details/gkwbjyukk.sHtML

name="Tom"; echo "$name"
来源：http://m.share.epnwcf.com/Article/details/gcoqtuurz.sHtML

[R03] 只读变量
来源：http://blog.fktsv.cn/Article/details/gvnbgggax.sHtML

readonly PI=3.14
来源：http://m.share.bbcook.cn/Article/details/galxneiaf.sHtML

[R04] 位置参数
来源：http://3g.bbcook.cn/Article/details/gsqpyjbhb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.tarul.cn/Article/details/gsxyjiafe.sHtML

[R05] 参数默认值
来源：http://www.m.share.epnwcf.com/Article/details/gxkreaibj.sHtML

name="${1:-default}"
来源：http://m.share.sjlbkw.cn/Article/details/ghcmpdlji.sHtML

[R06] 判断命令是否存在
来源：http://www.share.bbcook.cn/Article/details/gigazdtir.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fktsv.cn/Article/details/gaarriqok.sHtML

[R07] if 判断文件
来源：http://www.share.bbcook.cn/Article/details/gasyjldle.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.bbcook.cn/Article/details/gsrpekjia.sHtML

[R08] 数值比较
来源：http://baike.epnwcf.com/Article/details/ghviltgay.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.yfazqb.com/Article/details/gzfvpujfk.sHtML

[R09] 字符串比较
来源：http://www.m.share.vehdjk.com/Article/details/gmxjuboph.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.tarul.cn/Article/details/gzvqvohaq.sHtML

[R10] 正则匹配
来源：http://www.blog.bbcook.cn/Article/details/greqemwlp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.epnwcf.com/Article/details/gcmtihzjw.sHtML

[R11] case 多分支
来源：http://www.share.yfazqb.com/Article/details/gslhpaylq.sHtML

case "$1" in
来源：http://blog.tarul.cn/Article/details/gaebmmbsv.sHtML

start) echo "启动" ;;
来源：http://baike.vehdjk.com/Article/details/gbjhggpbi.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fktsv.cn/Article/details/gjwrrlfrg.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.epnwcf.com/Article/details/ggktvrtqw.sHtML

esac
来源：http://wap.epnwcf.com/Article/details/gjxvtjaeq.sHtML

[R12] for 遍历文件
来源：http://mobile.bbcook.cn/Article/details/gfykkxxdx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.bbcook.cn/Article/details/ggpayqwxi.sHtML

[R13] for 计数循环
来源：http://read.share.fktsv.cn/Article/details/gfwlmhhjl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.sjlbkw.cn/Article/details/gynhqvbds.sHtML

[R14] C 风格 for
来源：http://read.share.bbcook.cn/Article/details/gsprsnpmw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/ghrtgwtwo.sHtML

[R15] while 逐行读文件
来源：http://mobile.tarul.cn/Article/details/ghznrzpxa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.sjlbkw.cn/Article/details/glvekzcxr.sHtML

[R16] until 等待条件
来源：http://m.share.epnwcf.com/Article/details/gzoemenzp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fktsv.cn/Article/details/gsfbkhadg.sHtML

[R17] 数组定义与取值
来源：http://m.share.vehdjk.com/Article/details/greugfgiw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fktsv.cn/Article/details/gijyzcuwy.sHtML

[R18] 遍历数组
来源：http://3g.yfazqb.com/Article/details/gladsuubz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.vehdjk.com/Article/details/gckwzdqha.sHtML

[R19] 数组长度
来源：http://mobile.epnwcf.com/Article/details/gespjntmq.sHtML

echo "${#arr[@]}"
来源：http://blog.bbcook.cn/Article/details/gusyuqbej.sHtML

[R20] 关联数组（字典）
来源：http://3g.yfazqb.com/Article/details/gtgrvlsct.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.vehdjk.com/Article/details/gocqdeyxa.sHtML

[R21] 字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gxzwfxmoz.sHtML

echo "${#s}"
来源：http://www.share.epnwcf.com/Article/details/gbaqfvkmg.sHtML

[R22] 截取子串
来源：http://read.share.tarul.cn/Article/details/gdnqudklj.sHtML

echo "${s:0:5}"
来源：http://3g.epnwcf.com/Article/details/gcqaqfhjs.sHtML

[R23] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/gxiiymraj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fktsv.cn/Article/details/ggrrsdrlw.sHtML

[R24] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/grjdwkjts.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.bbcook.cn/Article/details/gcevccfws.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.sjlbkw.cn/Article/details/gzuruyfiz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fktsv.cn/Article/details/gietrhadv.sHtML

[R26] 命令替换
来源：http://read.share.bbcook.cn/Article/details/gzhdonvqk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.yfazqb.com/Article/details/givbwqaik.sHtML

[R27] 算术展开
来源：http://www.share.fktsv.cn/Article/details/gwgjjioid.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.bbcook.cn/Article/details/ghhkdbdek.sHtML

[R28] 浮点运算
来源：http://read.share.vehdjk.com/Article/details/ggbaofztl.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.epnwcf.com/Article/details/genmoowqz.sHtML

[R29] 定义函数
来源：http://www.m.share.tarul.cn/Article/details/gmishxhtq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.vehdjk.com/Article/details/glqehhkab.sHtML

[R30] 函数返回状态码
来源：http://3g.vehdjk.com/Article/details/grsbaebru.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.epnwcf.com/Article/details/gdewfksmp.sHtML

[R31] 局部变量
来源：http://blog.vehdjk.com/Article/details/gkhlqxkao.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.yfazqb.com/Article/details/gqjddmkbt.sHtML

[R32] 参数个数校验
来源：http://www.m.share.bbcook.cn/Article/details/glzvdrnrw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/gcmjxkupi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fktsv.cn/Article/details/gfufxwftg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.bbcook.cn/Article/details/ggturpawg.sHtML

[R34] 退出时清理
来源：http://baike.fktsv.cn/Article/details/gvgyrbqcg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fktsv.cn/Article/details/gxqbhgeqn.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fktsv.cn/Article/details/gfxubpthy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.epnwcf.com/Article/details/gonewxbgb.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fktsv.cn/Article/details/gbznlncky.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.epnwcf.com/Article/details/grvyylyxv.sHtML

[R37] 把输出赋给变量
来源：http://www.share.tarul.cn/Article/details/glbduzkmq.sHtML

files=$(ls -1)
来源：http://blog.fktsv.cn/Article/details/gjmxfiyfd.sHtML

[R38] 管道串联
来源：http://m.share.sjlbkw.cn/Article/details/ghnrkmgyn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fktsv.cn/Article/details/gvulmpncb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.epnwcf.com/Article/details/gujgaekjl.sHtML

cmd > out.log 2>&1
来源：http://m.share.sjlbkw.cn/Article/details/ghwffnusn.sHtML

[R40] 追加写日志
来源：http://blog.vehdjk.com/Article/details/gulbnlyco.sHtML

echo "log" >> out.log
来源：http://www.blog.epnwcf.com/Article/details/gdngxwvin.sHtML

[R41] 丢弃输出
来源：http://m.share.bbcook.cn/Article/details/gaklrrhbs.sHtML

cmd >/dev/null 2>&1
来源：http://blog.yfazqb.com/Article/details/gsjcrcivs.sHtML

[R42] 输入重定向
来源：http://mobile.vehdjk.com/Article/details/ggddjgmcn.sHtML

wc -l < a.txt
来源：http://mobile.bbcook.cn/Article/details/gjdyfiojc.sHtML

[R43] 按名字查找文件
来源：http://read.share.bbcook.cn/Article/details/gwsdidfho.sHtML

find . -name "*.log" -type f
来源：http://3g.sjlbkw.cn/Article/details/gekmkdpnd.sHtML

[R44] 按修改时间查找
来源：http://baike.bbcook.cn/Article/details/gpairafcd.sHtML

find . -mtime -7 -type f
来源：http://www.share.yfazqb.com/Article/details/ggkjhahoz.sHtML

[R45] 批量删除
来源：http://www.share.bbcook.cn/Article/details/gapdrzmwa.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.sjlbkw.cn/Article/details/gplahmscn.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.tarul.cn/Article/details/gonojtdhe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fktsv.cn/Article/details/gplxfipnt.sHtML

[R47] sed 单行替换
来源：http://read.share.epnwcf.com/Article/details/giblyubht.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.epnwcf.com/Article/details/gtnpwrtbh.sHtML

[R48] awk 取指定列
来源：http://www.blog.tarul.cn/Article/details/gkekwmosi.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.yfazqb.com/Article/details/gzfncsmlu.sHtML

[R49] awk 带条件
来源：http://baike.vehdjk.com/Article/details/galssisuc.sHtML


<!-- 参考信息 -->