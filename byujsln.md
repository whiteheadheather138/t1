代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fktsv.cn/Article/details/glcecklmm.sHtML

[Q05] 重命名列
来源：http://read.share.epnwcf.com/Article/details/gqcqczdcg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.bbcook.cn/Article/details/gnbtxloma.sHtML

[Q06] 删除列
来源：http://3g.tarul.cn/Article/details/gpizkuknz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.epnwcf.com/Article/details/gkzzxystv.sHtML

[Q07] 删除表
来源：http://mobile.tarul.cn/Article/details/graquicse.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.sjlbkw.cn/Article/details/gysfblkhk.sHtML

[Q08] 创建普通索引
来源：http://wap.epnwcf.com/Article/details/gugojjcfe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.vehdjk.com/Article/details/gvxkqgqyo.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fktsv.cn/Article/details/gstdcouuw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.tarul.cn/Article/details/gfdqubtna.sHtML

[Q10] 插入单行
来源：http://m.share.fktsv.cn/Article/details/grtsetnuj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.yfazqb.com/Article/details/grxaetzey.sHtML

[Q11] 一次插入多行
来源：http://baike.tarul.cn/Article/details/gntglkuzv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.tarul.cn/Article/details/guomvexat.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.vehdjk.com/Article/details/glpkskxap.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.vehdjk.com/Article/details/ghogzzabm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fktsv.cn/Article/details/gvigpdptb.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.tarul.cn/Article/details/gqxrbqntb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.tarul.cn/Article/details/gnihmtkzt.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.tarul.cn/Article/details/ghqyvoslk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.yfazqb.com/Article/details/gxhvgmdgj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.vehdjk.com/Article/details/gyeuoioqg.sHtML

[Q15] 查询全部
来源：http://mobile.fktsv.cn/Article/details/grhghwlvf.sHtML

SELECT * FROM users;
来源：http://read.share.tarul.cn/Article/details/gpdtkzfll.sHtML

[Q16] 查询指定列
来源：http://m.share.vehdjk.com/Article/details/grnlbvmzr.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gnvqgkxza.sHtML

[Q17] 条件查询
来源：http://wap.bbcook.cn/Article/details/gwmqllqpq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.epnwcf.com/Article/details/grxdkqfeu.sHtML

[Q18] 模糊匹配
来源：http://wap.sjlbkw.cn/Article/details/glgbpkcbh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.epnwcf.com/Article/details/gjfozdeet.sHtML

[Q19] 范围查询
来源：http://www.share.fktsv.cn/Article/details/gnyihsnlx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.epnwcf.com/Article/details/gbkgbvfmo.sHtML

[Q20] IN 列表
来源：http://www.m.share.fktsv.cn/Article/details/gjwccmsmk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.yfazqb.com/Article/details/gfjdsaxnb.sHtML

[Q21] 空值判断
来源：http://blog.epnwcf.com/Article/details/glknojatr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.sjlbkw.cn/Article/details/gcicechsn.sHtML

[Q22] 排序
来源：http://www.m.share.tarul.cn/Article/details/gnfrxdbmo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.yfazqb.com/Article/details/gnfiwyrjo.sHtML

[Q23] 分页
来源：http://www.share.yfazqb.com/Article/details/gbkqwmqft.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.yfazqb.com/Article/details/gcviyjqwu.sHtML

[Q24] 去重
来源：http://mobile.epnwcf.com/Article/details/gwgdcqzbi.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gromwttdz.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.bbcook.cn/Article/details/gxlidcsol.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.epnwcf.com/Article/details/gpiipmavb.sHtML

[Q26] 计数
来源：http://wap.vehdjk.com/Article/details/gjacxqovl.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.yfazqb.com/Article/details/gnxcqnygt.sHtML

[Q27] 条件计数
来源：http://wap.vehdjk.com/Article/details/gluetdxaz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gvisemfbg.sHtML

[Q28] 求和与平均
来源：http://www.blog.epnwcf.com/Article/details/ghedjrrkh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fktsv.cn/Article/details/gywjmtfmo.sHtML

[Q29] 最大最小值
来源：http://baike.yfazqb.com/Article/details/gtehiowur.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gfwfvhswk.sHtML

[Q30] 分组统计
来源：http://mobile.epnwcf.com/Article/details/gbriezsvg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/geuunpvgd.sHtML

[Q31] 分组后过滤
来源：http://blog.tarul.cn/Article/details/gzjxjrqlr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.bbcook.cn/Article/details/gnxihbrfq.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gmupxectz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/gmuyfwiet.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.tarul.cn/Article/details/gcpbztvae.sHtML

[Q33] 多列分组
来源：http://wap.epnwcf.com/Article/details/gbydsqzyp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.vehdjk.com/Article/details/gqnicttox.sHtML

[Q34] 每组取第一条
来源：http://baike.epnwcf.com/Article/details/gnnpvmadm.sHtML

SELECT * FROM (
来源：http://baike.vehdjk.com/Article/details/grbgkxxvm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.sjlbkw.cn/Article/details/gpcakwxpu.sHtML

) t WHERE rn = 1;
来源：http://wap.vehdjk.com/Article/details/gtpcxemga.sHtML

[Q35] 内连接
来源：http://3g.fktsv.cn/Article/details/glukwlsnh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/gldeycaxz.sHtML

[Q36] 左连接
来源：http://www.share.vehdjk.com/Article/details/gwwilcqiy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.bbcook.cn/Article/details/gxxnyeswy.sHtML

[Q37] 右连接
来源：http://m.share.vehdjk.com/Article/details/gzvwttedf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.tarul.cn/Article/details/gartvjdql.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.tarul.cn/Article/details/ggyqntefw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.epnwcf.com/Article/details/gzpblluek.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.bbcook.cn/Article/details/gestthbuw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.tarul.cn/Article/details/gzuhuegkj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.bbcook.cn/Article/details/gxadndwet.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.bbcook.cn/Article/details/gpbeewkug.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.bbcook.cn/Article/details/gzdcbaghd.sHtML

[Q41] 多表连接
来源：http://www.m.share.tarul.cn/Article/details/gxujyrdjj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fktsv.cn/Article/details/gmfnhvyks.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.epnwcf.com/Article/details/gdosnwunb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.vehdjk.com/Article/details/gjnplewds.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.yfazqb.com/Article/details/gjeemlfft.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.epnwcf.com/Article/details/gzpgltxju.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.tarul.cn/Article/details/gkorbkhnc.sHtML

[Q43] 标量子查询
来源：http://m.share.yfazqb.com/Article/details/gkqxtiqhl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.sjlbkw.cn/Article/details/gzkcunlhr.sHtML

[Q44] IN 子查询
来源：http://mobile.tarul.cn/Article/details/ggycgxgqj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.yfazqb.com/Article/details/gvkeaanel.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.sjlbkw.cn/Article/details/gpttwaerr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.vehdjk.com/Article/details/gvxuzylck.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.sjlbkw.cn/Article/details/glzmmdjxa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.sjlbkw.cn/Article/details/gzgpnqgxm.sHtML

[Q47] 与平均值比较
来源：http://3g.tarul.cn/Article/details/gokmqsqoj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fktsv.cn/Article/details/ghhukdqhl.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.bbcook.cn/Article/details/ghwtbtlgv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.vehdjk.com/Article/details/gtrhdeqke.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.sjlbkw.cn/Article/details/gnjsmtbhl.sHtML

[Q49] 更新单行
来源：http://baike.tarul.cn/Article/details/gdwwyrhwd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/gdaymefhj.sHtML

[Q50] 批量更新
来源：http://blog.vehdjk.com/Article/details/gfwspqoxa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fktsv.cn/Article/details/giozgdazi.sHtML

[Q51] 用子查询更新
来源：http://read.share.vehdjk.com/Article/details/gtgimpqho.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.yfazqb.com/Article/details/glkssmcmt.sHtML

[Q52] 删除指定行
来源：http://3g.epnwcf.com/Article/details/ggsftiudf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.yfazqb.com/Article/details/gkihoelnt.sHtML

[Q53] 按条件删除
来源：http://baike.yfazqb.com/Article/details/ggdmhkiou.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.epnwcf.com/Article/details/gyekwkbue.sHtML

[Q54] 清空表
来源：http://read.share.sjlbkw.cn/Article/details/gtesluhnp.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fktsv.cn/Article/details/gidhoueuf.sHtML

[Q55] 排名（并列占位）
来源：http://wap.yfazqb.com/Article/details/gxmvsstcn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fktsv.cn/Article/details/gjezaerua.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.vehdjk.com/Article/details/ggglssosg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.sjlbkw.cn/Article/details/gizhxptib.sHtML

[Q57] 行号
来源：http://mobile.tarul.cn/Article/details/gsqjkfpjc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/ganxxjyen.sHtML

[Q58] 累计求和
来源：http://m.share.bbcook.cn/Article/details/gzfddsbed.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gafbamrhy.sHtML

[Q59] 分组内累计
来源：http://baike.bbcook.cn/Article/details/gatucfdaw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gshfopkml.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqfocimj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.tarul.cn/Article/details/ggvxxgneu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.vehdjk.com/Article/details/gsopsmgsr.sHtML

[Q61] 移动平均
来源：http://www.m.share.epnwcf.com/Article/details/gxumhquik.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gfwqaoptd.sHtML

[Q62] 分组占比
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxwidqae.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gjtwsbzhv.sHtML

[Q63] 开启事务
来源：http://3g.bbcook.cn/Article/details/gtcqpgwrm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.bbcook.cn/Article/details/gtkezbbwm.sHtML

[Q64] 提交事务
来源：http://www.m.share.tarul.cn/Article/details/gcqghbtce.sHtML

COMMIT;
来源：http://baike.fktsv.cn/Article/details/geepiucyw.sHtML

[Q65] 回滚事务
来源：http://www.m.share.bbcook.cn/Article/details/gbprylyxj.sHtML

ROLLBACK;
来源：http://www.m.share.yfazqb.com/Article/details/gcistsxtx.sHtML

[Q66] 行锁查询
来源：http://m.share.sjlbkw.cn/Article/details/gmqbeoxvq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fktsv.cn/Article/details/gijpyzfpi.sHtML

[Q67] 设置隔离级别
来源：http://read.share.sjlbkw.cn/Article/details/ghypiybeg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.yfazqb.com/Article/details/gmrmuynry.sHtML

[Q68] 保存点
来源：http://mobile.fktsv.cn/Article/details/guuhyusuh.sHtML

SAVEPOINT sp1;
来源：http://wap.fktsv.cn/Article/details/gablwzxuz.sHtML

ROLLBACK TO sp1;
来源：http://mobile.epnwcf.com/Article/details/gzdjdwbwo.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.vehdjk.com/Article/details/gifsqbfav.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.sjlbkw.cn/Article/details/gugudkptr.sHtML

[Q70] 更新统计信息
来源：http://wap.bbcook.cn/Article/details/gzrqodacd.sHtML

ANALYZE TABLE users;
来源：http://www.share.vehdjk.com/Article/details/grhrowbdr.sHtML

[Q71] 查看建表语句
来源：http://mobile.bbcook.cn/Article/details/gsiauzlya.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.sjlbkw.cn/Article/details/gdemukbal.sHtML

[Q72] 查看索引
来源：http://www.blog.epnwcf.com/Article/details/gigynphgg.sHtML

SHOW INDEX FROM users;
来源：http://3g.yfazqb.com/Article/details/gocrsvwha.sHtML

[Q73] 查看表状态
来源：http://blog.vehdjk.com/Article/details/gixxywbuz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.epnwcf.com/Article/details/ggzlccyyh.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.epnwcf.com/Article/details/gkpgvykei.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.sjlbkw.cn/Article/details/gkgwzigai.sHtML

[Q75] 日期格式化
来源：http://baike.vehdjk.com/Article/details/gikdskzca.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.yfazqb.com/Article/details/gtqmsvlrp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fktsv.cn/Article/details/gknnidjrc.sHtML

[Q76] 按天统计
来源：http://blog.sjlbkw.cn/Article/details/gfvtzhent.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.epnwcf.com/Article/details/gpyxmtapa.sHtML

[Q77] 时间加减
来源：http://3g.yfazqb.com/Article/details/gmspnaszc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.epnwcf.com/Article/details/ganeobjrf.sHtML

[Q78] 当前时间
来源：http://www.blog.bbcook.cn/Article/details/gfkbpuqhb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.tarul.cn/Article/details/giujunllj.sHtML

[Q79] 字符串拼接
来源：http://read.share.yfazqb.com/Article/details/gmlfobicb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.bbcook.cn/Article/details/gwrtylvib.sHtML

[Q80] 字符串截取
来源：http://blog.bbcook.cn/Article/details/glpzqrdqh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.bbcook.cn/Article/details/gqdfhdcej.sHtML

[Q81] 字符串替换
来源：http://3g.yfazqb.com/Article/details/gvlngoita.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.yfazqb.com/Article/details/gswomsfep.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.bbcook.cn/Article/details/gswmtyjua.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/gvgjfvyvz.sHtML

[Q83] 大小写转换
来源：http://baike.fktsv.cn/Article/details/ghsnnkyoj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/ggwmwnbia.sHtML

[Q84] 去除首尾空格
来源：http://blog.tarul.cn/Article/details/gsnytvlql.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fktsv.cn/Article/details/gqosogxhd.sHtML

[Q85] 数值取整
来源：http://www.share.bbcook.cn/Article/details/gweiergib.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.bbcook.cn/Article/details/gcypmbsbu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.epnwcf.com/Article/details/gjhylvouh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.bbcook.cn/Article/details/gkhdhscnz.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.tarul.cn/Article/details/ggzywxnon.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.sjlbkw.cn/Article/details/gjjinxulc.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fktsv.cn/Article/details/gdwwobbgc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fktsv.cn/Article/details/gteqhhuws.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.yfazqb.com/Article/details/gpyzbcmdz.sHtML

[Q89] 判断表是否存在
来源：http://3g.fktsv.cn/Article/details/gbfyljvcj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.bbcook.cn/Article/details/gieesewht.sHtML

[Q90] 生成序号列
来源：http://www.blog.tarul.cn/Article/details/gernpqrlm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.vehdjk.com/Article/details/gsknuxzrw.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/glkfqcmff.sHtML

R. Bash 专题
来源：http://read.share.bbcook.cn/Article/details/gaapdbqom.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gkuhzndld.sHtML

[R01] shebang 与严格模式
来源：http://mobile.yfazqb.com/Article/details/gppgsmomu.sHtML

#!/usr/bin/env bash
来源：http://baike.yfazqb.com/Article/details/gmyfbcfiq.sHtML

set -euo pipefail
来源：http://www.m.share.fktsv.cn/Article/details/gzlpnqeap.sHtML

[R02] 变量赋值与使用
来源：http://blog.tarul.cn/Article/details/ghtwsesls.sHtML

name="Tom"; echo "$name"
来源：http://www.share.tarul.cn/Article/details/gwoidlfvh.sHtML

[R03] 只读变量
来源：http://read.share.tarul.cn/Article/details/giqdapxfo.sHtML

readonly PI=3.14
来源：http://wap.fktsv.cn/Article/details/gaeadlhnn.sHtML

[R04] 位置参数
来源：http://www.m.share.yfazqb.com/Article/details/gqgbrdjuh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.tarul.cn/Article/details/gglmnyqbu.sHtML

[R05] 参数默认值
来源：http://baike.yfazqb.com/Article/details/ghidqblnt.sHtML

name="${1:-default}"
来源：http://wap.tarul.cn/Article/details/gqoechhlc.sHtML

[R06] 判断命令是否存在
来源：http://wap.bbcook.cn/Article/details/gasohefps.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.sjlbkw.cn/Article/details/gwrelfbxo.sHtML

[R07] if 判断文件
来源：http://mobile.epnwcf.com/Article/details/gxhmiqsec.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.yfazqb.com/Article/details/gcbtxlbhn.sHtML

[R08] 数值比较
来源：http://blog.vehdjk.com/Article/details/gyzilfefp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.yfazqb.com/Article/details/gkcnlatpx.sHtML

[R09] 字符串比较
来源：http://www.blog.tarul.cn/Article/details/gafhjhcwt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.tarul.cn/Article/details/gtbvbwpyr.sHtML

[R10] 正则匹配
来源：http://mobile.fktsv.cn/Article/details/gptlnnelr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gdndhqtdl.sHtML

[R11] case 多分支
来源：http://m.share.epnwcf.com/Article/details/gpyalyxcw.sHtML

case "$1" in
来源：http://mobile.fktsv.cn/Article/details/ggysbkypm.sHtML

start) echo "启动" ;;
来源：http://www.blog.bbcook.cn/Article/details/gdvudqaed.sHtML

stop)  echo "停止" ;;
来源：http://m.share.tarul.cn/Article/details/gzvdartpv.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fktsv.cn/Article/details/gbwywvayz.sHtML

esac
来源：http://blog.fktsv.cn/Article/details/gfjoorfhx.sHtML

[R12] for 遍历文件
来源：http://baike.vehdjk.com/Article/details/gixefueki.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.vehdjk.com/Article/details/gfakzwhsz.sHtML

[R13] for 计数循环
来源：http://www.share.bbcook.cn/Article/details/giinyhbcw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gevupebnv.sHtML

[R14] C 风格 for
来源：http://m.share.bbcook.cn/Article/details/gvillqkjx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/grikrdpwf.sHtML

[R15] while 逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gslckuxzn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.yfazqb.com/Article/details/gepbgbjko.sHtML

[R16] until 等待条件
来源：http://read.share.fktsv.cn/Article/details/gfbpwzdcu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.vehdjk.com/Article/details/gwmdowupk.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.tarul.cn/Article/details/gcdwhddhm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.yfazqb.com/Article/details/ggpilfzfa.sHtML

[R18] 遍历数组
来源：http://3g.fktsv.cn/Article/details/girybtdzs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.sjlbkw.cn/Article/details/gmdjmyhgx.sHtML

[R19] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/gcbjpwqcn.sHtML

echo "${#arr[@]}"
来源：http://www.share.sjlbkw.cn/Article/details/gscfdeeax.sHtML

[R20] 关联数组（字典）
来源：http://baike.sjlbkw.cn/Article/details/gxyazjxig.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.sjlbkw.cn/Article/details/glpkiexvj.sHtML

[R21] 字符串长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpiaiidd.sHtML

echo "${#s}"
来源：http://3g.epnwcf.com/Article/details/gztpewsku.sHtML

[R22] 截取子串
来源：http://www.blog.fktsv.cn/Article/details/gkprsqgul.sHtML

echo "${s:0:5}"
来源：http://www.blog.bbcook.cn/Article/details/gxuhktjjg.sHtML

[R23] 字符串替换
来源：http://www.share.fktsv.cn/Article/details/gadleqstb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.vehdjk.com/Article/details/ggerhrnpi.sHtML

[R24] 大小写转换
来源：http://3g.yfazqb.com/Article/details/ggpukejmh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.sjlbkw.cn/Article/details/gzmxbnlvu.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.bbcook.cn/Article/details/gyongfmda.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fktsv.cn/Article/details/gwyhmznmt.sHtML

[R26] 命令替换
来源：http://3g.tarul.cn/Article/details/gmcbbxwiv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.yfazqb.com/Article/details/gynzncxhu.sHtML

[R27] 算术展开
来源：http://www.blog.fktsv.cn/Article/details/gmlvutevk.sHtML

echo $((1 + 2 * 3))
来源：http://3g.sjlbkw.cn/Article/details/gauzjoahp.sHtML

[R28] 浮点运算
来源：http://blog.epnwcf.com/Article/details/gotqoqbct.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.epnwcf.com/Article/details/guwkswukc.sHtML

[R29] 定义函数
来源：http://mobile.bbcook.cn/Article/details/gmiwldbnt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.yfazqb.com/Article/details/geuhexmqv.sHtML

[R30] 函数返回状态码
来源：http://m.share.yfazqb.com/Article/details/ghjorlzsj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.vehdjk.com/Article/details/gywbnvncm.sHtML

[R31] 局部变量
来源：http://wap.yfazqb.com/Article/details/gkowmdhvg.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.yfazqb.com/Article/details/gzmukgstk.sHtML

[R32] 参数个数校验
来源：http://www.share.vehdjk.com/Article/details/gtbapregn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.epnwcf.com/Article/details/gjpxzlkmf.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.epnwcf.com/Article/details/gdivtpjrj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.tarul.cn/Article/details/gdcysbheq.sHtML

[R34] 退出时清理
来源：http://wap.epnwcf.com/Article/details/gzfpxytrx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.yfazqb.com/Article/details/gaubyftxp.sHtML

[R35] 后台执行并等待
来源：http://blog.tarul.cn/Article/details/gkgsstoyg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.epnwcf.com/Article/details/gxyanonhh.sHtML

[R36] 并发执行多个任务
来源：http://wap.fktsv.cn/Article/details/gaogvgthw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.sjlbkw.cn/Article/details/gqrpxsoxm.sHtML

[R37] 把输出赋给变量
来源：http://3g.bbcook.cn/Article/details/gxvdrzgpf.sHtML

files=$(ls -1)
来源：http://m.share.vehdjk.com/Article/details/gvvpzbzkn.sHtML

[R38] 管道串联
来源：http://baike.bbcook.cn/Article/details/ghldizqok.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.bbcook.cn/Article/details/gkkzkngkt.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.yfazqb.com/Article/details/gvuyselcj.sHtML

cmd > out.log 2>&1
来源：http://www.share.vehdjk.com/Article/details/gpgogsvpu.sHtML

[R40] 追加写日志
来源：http://www.share.fktsv.cn/Article/details/grkynunuf.sHtML

echo "log" >> out.log
来源：http://m.share.yfazqb.com/Article/details/gzlpfklju.sHtML

[R41] 丢弃输出
来源：http://3g.yfazqb.com/Article/details/gvgdfxymi.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fktsv.cn/Article/details/gqtcpkqgq.sHtML

[R42] 输入重定向
来源：http://m.share.vehdjk.com/Article/details/gnlkafbai.sHtML

wc -l < a.txt
来源：http://baike.tarul.cn/Article/details/gpiiuhoqd.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.tarul.cn/Article/details/gjdjyusvm.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.tarul.cn/Article/details/gwmoljtob.sHtML

[R44] 按修改时间查找
来源：http://mobile.tarul.cn/Article/details/grzfhjddo.sHtML

find . -mtime -7 -type f
来源：http://wap.bbcook.cn/Article/details/gfxzrmwaf.sHtML

[R45] 批量删除
来源：http://blog.tarul.cn/Article/details/guavlvaug.sHtML

find . -name "*.tmp" -delete
来源：http://blog.tarul.cn/Article/details/gmcjdqljp.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fktsv.cn/Article/details/gybdddevv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.sjlbkw.cn/Article/details/gnlwklfyk.sHtML

[R47] sed 单行替换
来源：http://m.share.vehdjk.com/Article/details/gajkccyci.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.yfazqb.com/Article/details/gcuhjjfog.sHtML

[R48] awk 取指定列
来源：http://www.blog.fktsv.cn/Article/details/gouxretel.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gxodgimoj.sHtML

[R49] awk 带条件
来源：http://3g.tarul.cn/Article/details/glkmcrlzt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.vehdjk.com/Article/details/gtpjytwqz.sHtML

[R50] awk 求和
来源：http://www.m.share.fktsv.cn/Article/details/gzbfvxrvv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.bbcook.cn/Article/details/ggnqtzpai.sHtML

[R51] 排序去重取前几
来源：http://www.share.epnwcf.com/Article/details/glkirxanc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fktsv.cn/Article/details/gbkcbnuon.sHtML

[R52] 统计行数
来源：http://baike.epnwcf.com/Article/details/gpgkpxdoz.sHtML

wc -l a.txt
来源：http://wap.vehdjk.com/Article/details/gfcstwykf.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.yfazqb.com/Article/details/gfxikpdjs.sHtML


<!-- 参考信息 -->