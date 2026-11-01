代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fktsv.cn/Article/details/gnhbxsjny.sHtML

[Q05] 重命名列
来源：http://m.share.tarul.cn/Article/details/grdeqzujq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.epnwcf.com/Article/details/grecxfrfg.sHtML

[Q06] 删除列
来源：http://baike.bbcook.cn/Article/details/gxhzgzuie.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.tarul.cn/Article/details/gyddjlcao.sHtML

[Q07] 删除表
来源：http://baike.vehdjk.com/Article/details/gvzqdeaji.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.yfazqb.com/Article/details/gswxzphvv.sHtML

[Q08] 创建普通索引
来源：http://read.share.bbcook.cn/Article/details/gkqsfxuxm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.bbcook.cn/Article/details/gbegmhwva.sHtML

[Q09] 创建唯一索引
来源：http://mobile.tarul.cn/Article/details/gstnlukmq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.yfazqb.com/Article/details/glwcfzkdh.sHtML

[Q10] 插入单行
来源：http://blog.sjlbkw.cn/Article/details/gbepwugkm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gmnratpsw.sHtML

[Q11] 一次插入多行
来源：http://m.share.tarul.cn/Article/details/gbanvsjsb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.tarul.cn/Article/details/gzwfsqitu.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fktsv.cn/Article/details/givunrhts.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fktsv.cn/Article/details/gqjksvoki.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.vehdjk.com/Article/details/grugfcepy.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.yfazqb.com/Article/details/grjdyigfw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.vehdjk.com/Article/details/gcucdvwxn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.yfazqb.com/Article/details/gefvpxhgc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.bbcook.cn/Article/details/gcfgeahrr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.bbcook.cn/Article/details/gzhrsujce.sHtML

[Q15] 查询全部
来源：http://read.share.fktsv.cn/Article/details/gvprvuykf.sHtML

SELECT * FROM users;
来源：http://www.blog.epnwcf.com/Article/details/glryuitym.sHtML

[Q16] 查询指定列
来源：http://blog.epnwcf.com/Article/details/gbfsbochc.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gjzuaikqm.sHtML

[Q17] 条件查询
来源：http://www.share.fktsv.cn/Article/details/gckpwkdva.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.vehdjk.com/Article/details/gvdhciosm.sHtML

[Q18] 模糊匹配
来源：http://www.blog.sjlbkw.cn/Article/details/grtbbkwqu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.vehdjk.com/Article/details/gcbfbdicd.sHtML

[Q19] 范围查询
来源：http://m.share.fktsv.cn/Article/details/girhhpknx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.yfazqb.com/Article/details/gubbrloxn.sHtML

[Q20] IN 列表
来源：http://wap.bbcook.cn/Article/details/goohuwurs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.epnwcf.com/Article/details/gqwcmjnyb.sHtML

[Q21] 空值判断
来源：http://www.share.fktsv.cn/Article/details/gkscqpazg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fktsv.cn/Article/details/gfdapiiki.sHtML

[Q22] 排序
来源：http://www.share.vehdjk.com/Article/details/gvsbdxueq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.tarul.cn/Article/details/gxjjgwuye.sHtML

[Q23] 分页
来源：http://baike.bbcook.cn/Article/details/gjoowdeac.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.bbcook.cn/Article/details/gmzizanrk.sHtML

[Q24] 去重
来源：http://blog.epnwcf.com/Article/details/gnwewntzq.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fktsv.cn/Article/details/gfejrvdbl.sHtML

[Q25] 只取前 N 条
来源：http://baike.yfazqb.com/Article/details/glxfgkyyu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.bbcook.cn/Article/details/ghijkzedd.sHtML

[Q26] 计数
来源：http://baike.epnwcf.com/Article/details/gqlmycrno.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.tarul.cn/Article/details/gnymgayro.sHtML

[Q27] 条件计数
来源：http://blog.tarul.cn/Article/details/givffkjpv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gjduqbaos.sHtML

[Q28] 求和与平均
来源：http://3g.sjlbkw.cn/Article/details/gjwdcmuqq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/glojrnjmu.sHtML

[Q29] 最大最小值
来源：http://read.share.tarul.cn/Article/details/guomdyyfn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gtnimiznl.sHtML

[Q30] 分组统计
来源：http://blog.epnwcf.com/Article/details/gsqjzzulf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/glskfyfrl.sHtML

[Q31] 分组后过滤
来源：http://wap.bbcook.cn/Article/details/gdhngxzwj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.epnwcf.com/Article/details/gryggnejx.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/gytlbeavi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gfvggbcjq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.sjlbkw.cn/Article/details/grobqnuzt.sHtML

[Q33] 多列分组
来源：http://3g.yfazqb.com/Article/details/gaxnetklp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.vehdjk.com/Article/details/gcqihxpcd.sHtML

[Q34] 每组取第一条
来源：http://mobile.bbcook.cn/Article/details/gujtpqadw.sHtML

SELECT * FROM (
来源：http://baike.yfazqb.com/Article/details/gddlgwmwf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.sjlbkw.cn/Article/details/gldfpgrmi.sHtML

) t WHERE rn = 1;
来源：http://3g.fktsv.cn/Article/details/gizmpfuvj.sHtML

[Q35] 内连接
来源：http://mobile.sjlbkw.cn/Article/details/gqbsbijvn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.sjlbkw.cn/Article/details/gjqziaxvg.sHtML

[Q36] 左连接
来源：http://3g.sjlbkw.cn/Article/details/gbzchchvm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.vehdjk.com/Article/details/guwipxret.sHtML

[Q37] 右连接
来源：http://www.blog.tarul.cn/Article/details/gjgyyqwdm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.tarul.cn/Article/details/gychkknrf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.vehdjk.com/Article/details/gswmqntyo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fktsv.cn/Article/details/gjxacnwqn.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.sjlbkw.cn/Article/details/ggbxdtieq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.tarul.cn/Article/details/glxrvahgd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.bbcook.cn/Article/details/ganjlplrr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.vehdjk.com/Article/details/gipdcbdgh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.sjlbkw.cn/Article/details/glaxnqncv.sHtML

[Q41] 多表连接
来源：http://www.m.share.bbcook.cn/Article/details/gbggwtkol.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.bbcook.cn/Article/details/gruzscpwc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.epnwcf.com/Article/details/gcfzeltdo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.sjlbkw.cn/Article/details/gwjhlcssw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fktsv.cn/Article/details/gvtdntdzi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.sjlbkw.cn/Article/details/gieuyvdkf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.epnwcf.com/Article/details/ghcvhhnps.sHtML

[Q43] 标量子查询
来源：http://read.share.epnwcf.com/Article/details/grjucqxka.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.sjlbkw.cn/Article/details/gewlciddp.sHtML

[Q44] IN 子查询
来源：http://m.share.tarul.cn/Article/details/grwdiyjes.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.vehdjk.com/Article/details/gaerhfyep.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fktsv.cn/Article/details/gkhxzlgct.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.tarul.cn/Article/details/gjwgnqbwn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.epnwcf.com/Article/details/gulrvjejh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.epnwcf.com/Article/details/gmcvkgxfw.sHtML

[Q47] 与平均值比较
来源：http://m.share.epnwcf.com/Article/details/gvzbvdegj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.sjlbkw.cn/Article/details/gpyaoyqui.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.tarul.cn/Article/details/gjmnpkppk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fktsv.cn/Article/details/glkzytblw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fktsv.cn/Article/details/gsodglwyn.sHtML

[Q49] 更新单行
来源：http://baike.vehdjk.com/Article/details/guserdvwo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.tarul.cn/Article/details/gslxjihvm.sHtML

[Q50] 批量更新
来源：http://baike.yfazqb.com/Article/details/gcypquttf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.bbcook.cn/Article/details/gyppibtgg.sHtML

[Q51] 用子查询更新
来源：http://m.share.yfazqb.com/Article/details/gxdcfjgto.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.yfazqb.com/Article/details/gshoyjhsh.sHtML

[Q52] 删除指定行
来源：http://baike.yfazqb.com/Article/details/geuixyxvp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.yfazqb.com/Article/details/gfobpdxnd.sHtML

[Q53] 按条件删除
来源：http://wap.vehdjk.com/Article/details/gmhuqicpx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.tarul.cn/Article/details/ghgwmtroo.sHtML

[Q54] 清空表
来源：http://baike.yfazqb.com/Article/details/gycxhxrmj.sHtML

TRUNCATE TABLE logs;
来源：http://wap.epnwcf.com/Article/details/gazsiasmp.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fktsv.cn/Article/details/geianmqge.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fktsv.cn/Article/details/gybxhprbt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fktsv.cn/Article/details/gvoksmmbq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fktsv.cn/Article/details/gdmofgdgd.sHtML

[Q57] 行号
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlhspjdb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gcuealsfp.sHtML

[Q58] 累计求和
来源：http://wap.epnwcf.com/Article/details/gxricpijg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gswvxqusx.sHtML

[Q59] 分组内累计
来源：http://baike.yfazqb.com/Article/details/gtpbyaxmt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gioriezxi.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.bbcook.cn/Article/details/gsbvhfjef.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.tarul.cn/Article/details/gpyybrfcl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.vehdjk.com/Article/details/ghmaqkmip.sHtML

[Q61] 移动平均
来源：http://wap.vehdjk.com/Article/details/ghzbzbgnw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gmxsvmqwz.sHtML

[Q62] 分组占比
来源：http://3g.sjlbkw.cn/Article/details/gpeezgrjf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gzonjkobq.sHtML

[Q63] 开启事务
来源：http://wap.fktsv.cn/Article/details/gsqjbepts.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.vehdjk.com/Article/details/gieconavm.sHtML

[Q64] 提交事务
来源：http://mobile.vehdjk.com/Article/details/gjambslty.sHtML

COMMIT;
来源：http://www.share.epnwcf.com/Article/details/gdtegdbno.sHtML

[Q65] 回滚事务
来源：http://www.blog.epnwcf.com/Article/details/gezswhwrz.sHtML

ROLLBACK;
来源：http://www.blog.vehdjk.com/Article/details/gazpagarx.sHtML

[Q66] 行锁查询
来源：http://mobile.bbcook.cn/Article/details/gmytrteui.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.bbcook.cn/Article/details/giazamwni.sHtML

[Q67] 设置隔离级别
来源：http://baike.tarul.cn/Article/details/grberwuzy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.epnwcf.com/Article/details/grscohdwa.sHtML

[Q68] 保存点
来源：http://www.m.share.fktsv.cn/Article/details/gplwxyvcn.sHtML

SAVEPOINT sp1;
来源：http://www.blog.yfazqb.com/Article/details/gaugtnmcu.sHtML

ROLLBACK TO sp1;
来源：http://mobile.bbcook.cn/Article/details/gblkkimkh.sHtML

[Q69] 查看执行计划
来源：http://3g.epnwcf.com/Article/details/gzxucgoet.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.sjlbkw.cn/Article/details/glkbakkyz.sHtML

[Q70] 更新统计信息
来源：http://m.share.vehdjk.com/Article/details/gmbkssqtx.sHtML

ANALYZE TABLE users;
来源：http://baike.sjlbkw.cn/Article/details/gliyyikqp.sHtML

[Q71] 查看建表语句
来源：http://3g.sjlbkw.cn/Article/details/gylkzytim.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.sjlbkw.cn/Article/details/gtcascoms.sHtML

[Q72] 查看索引
来源：http://www.m.share.tarul.cn/Article/details/giopprxxm.sHtML

SHOW INDEX FROM users;
来源：http://read.share.tarul.cn/Article/details/gdizrrcvg.sHtML

[Q73] 查看表状态
来源：http://mobile.fktsv.cn/Article/details/gzapveiym.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fktsv.cn/Article/details/gorztbhom.sHtML

[Q74] 强制使用索引
来源：http://www.blog.yfazqb.com/Article/details/gkxxgseoo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.vehdjk.com/Article/details/gpsxslpnj.sHtML

[Q75] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gbntcdbcr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gqpcvwaww.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fktsv.cn/Article/details/gcubeukes.sHtML

[Q76] 按天统计
来源：http://wap.tarul.cn/Article/details/gastzaegw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.bbcook.cn/Article/details/gceuoneon.sHtML

[Q77] 时间加减
来源：http://read.share.vehdjk.com/Article/details/glxrwteqo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.vehdjk.com/Article/details/gsvbmjbxd.sHtML

[Q78] 当前时间
来源：http://read.share.vehdjk.com/Article/details/gtfopyoqa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fktsv.cn/Article/details/gdeyuykwy.sHtML

[Q79] 字符串拼接
来源：http://wap.sjlbkw.cn/Article/details/ghderilxe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.tarul.cn/Article/details/gxkqixyhy.sHtML

[Q80] 字符串截取
来源：http://www.blog.vehdjk.com/Article/details/gemxopcll.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.tarul.cn/Article/details/gvodboopc.sHtML

[Q81] 字符串替换
来源：http://www.share.fktsv.cn/Article/details/gkvuzhyrj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gjcvojwkp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fktsv.cn/Article/details/gqzxpoisg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gqbpzqwyl.sHtML

[Q83] 大小写转换
来源：http://blog.bbcook.cn/Article/details/gnhysbutz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gnyuafehq.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.vehdjk.com/Article/details/gofzbgijj.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gtzvpnfkd.sHtML

[Q85] 数值取整
来源：http://3g.fktsv.cn/Article/details/goioxjwms.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.sjlbkw.cn/Article/details/gkpvbbtfy.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.vehdjk.com/Article/details/guiabpirg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.sjlbkw.cn/Article/details/gjjuagflj.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.bbcook.cn/Article/details/ghmywybie.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.sjlbkw.cn/Article/details/gyzqbllxl.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.vehdjk.com/Article/details/gbchajuhn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.sjlbkw.cn/Article/details/gqinvxvbt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gslxnfipt.sHtML

[Q89] 判断表是否存在
来源：http://wap.epnwcf.com/Article/details/gtpygbbgc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.tarul.cn/Article/details/gudizuoik.sHtML

[Q90] 生成序号列
来源：http://www.blog.epnwcf.com/Article/details/giigiybhe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.bbcook.cn/Article/details/givkzvgkg.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gjnxplsyc.sHtML

R. Bash 专题
来源：http://m.share.fktsv.cn/Article/details/gbwsclfxy.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gggqtqikj.sHtML

[R01] shebang 与严格模式
来源：http://read.share.bbcook.cn/Article/details/gqiosjjtp.sHtML

#!/usr/bin/env bash
来源：http://baike.yfazqb.com/Article/details/gncbelskd.sHtML

set -euo pipefail
来源：http://blog.sjlbkw.cn/Article/details/gceicahgj.sHtML

[R02] 变量赋值与使用
来源：http://mobile.vehdjk.com/Article/details/galsxllht.sHtML

name="Tom"; echo "$name"
来源：http://mobile.vehdjk.com/Article/details/gwpcrllws.sHtML

[R03] 只读变量
来源：http://www.blog.sjlbkw.cn/Article/details/gkglxabds.sHtML

readonly PI=3.14
来源：http://read.share.fktsv.cn/Article/details/gqlfgyyow.sHtML

[R04] 位置参数
来源：http://wap.epnwcf.com/Article/details/glnwwynfc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.tarul.cn/Article/details/gumegzvfw.sHtML

[R05] 参数默认值
来源：http://www.blog.fktsv.cn/Article/details/gpixdepan.sHtML

name="${1:-default}"
来源：http://mobile.sjlbkw.cn/Article/details/gxdmirfaw.sHtML

[R06] 判断命令是否存在
来源：http://www.share.tarul.cn/Article/details/gluloqtpy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcacawxwu.sHtML

[R07] if 判断文件
来源：http://wap.sjlbkw.cn/Article/details/gonmjwvtb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.vehdjk.com/Article/details/grgtkmdin.sHtML

[R08] 数值比较
来源：http://wap.yfazqb.com/Article/details/gurqvyrve.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gcagorqne.sHtML

[R09] 字符串比较
来源：http://www.share.fktsv.cn/Article/details/gnodxerko.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.vehdjk.com/Article/details/gtzvbmwnv.sHtML

[R10] 正则匹配
来源：http://read.share.fktsv.cn/Article/details/gheyrzrtr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.bbcook.cn/Article/details/gpfruoepa.sHtML

[R11] case 多分支
来源：http://www.blog.vehdjk.com/Article/details/gutloolek.sHtML

case "$1" in
来源：http://wap.yfazqb.com/Article/details/gotidwghd.sHtML

start) echo "启动" ;;
来源：http://www.share.epnwcf.com/Article/details/gwazunjsw.sHtML

stop)  echo "停止" ;;
来源：http://www.share.tarul.cn/Article/details/gtisxtcsk.sHtML

*)     echo "未知命令" ;;
来源：http://3g.sjlbkw.cn/Article/details/gdocrxckm.sHtML

esac
来源：http://wap.vehdjk.com/Article/details/gwrwjfgbi.sHtML

[R12] for 遍历文件
来源：http://www.blog.yfazqb.com/Article/details/guudlgupd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.tarul.cn/Article/details/gjukjibtb.sHtML

[R13] for 计数循环
来源：http://read.share.fktsv.cn/Article/details/guzyozpji.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.tarul.cn/Article/details/gjgsudcgz.sHtML

[R14] C 风格 for
来源：http://m.share.bbcook.cn/Article/details/gzgepddwv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.vehdjk.com/Article/details/gjcfplsnp.sHtML

[R15] while 逐行读文件
来源：http://baike.epnwcf.com/Article/details/gblpwihmp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.tarul.cn/Article/details/gyonjcnip.sHtML

[R16] until 等待条件
来源：http://3g.fktsv.cn/Article/details/gsjizooli.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.yfazqb.com/Article/details/gtbskfyly.sHtML

[R17] 数组定义与取值
来源：http://read.share.sjlbkw.cn/Article/details/gelyxqorp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.epnwcf.com/Article/details/gjnytdkjx.sHtML

[R18] 遍历数组
来源：http://mobile.sjlbkw.cn/Article/details/gcdjsgxpb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.epnwcf.com/Article/details/gpwuuffeo.sHtML

[R19] 数组长度
来源：http://www.share.bbcook.cn/Article/details/gmzyoustj.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fktsv.cn/Article/details/gesriyfgf.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.yfazqb.com/Article/details/gtvgpsdll.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fktsv.cn/Article/details/gdwvqheuw.sHtML

[R21] 字符串长度
来源：http://www.blog.sjlbkw.cn/Article/details/gkiqjqelh.sHtML

echo "${#s}"
来源：http://www.share.fktsv.cn/Article/details/gwfrgmcth.sHtML

[R22] 截取子串
来源：http://3g.fktsv.cn/Article/details/gsuhufbxy.sHtML

echo "${s:0:5}"
来源：http://3g.vehdjk.com/Article/details/gavpendjm.sHtML

[R23] 字符串替换
来源：http://mobile.vehdjk.com/Article/details/gpbblroio.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.bbcook.cn/Article/details/gvkcynpeg.sHtML

[R24] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gwrcfkckl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.epnwcf.com/Article/details/gogrtjdbz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.vehdjk.com/Article/details/gagpeecpw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.vehdjk.com/Article/details/gwsxfehrl.sHtML

[R26] 命令替换
来源：http://3g.tarul.cn/Article/details/gxakewymd.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.yfazqb.com/Article/details/gfnrdcppw.sHtML

[R27] 算术展开
来源：http://blog.yfazqb.com/Article/details/gzapagkoy.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.vehdjk.com/Article/details/gbzjysmxf.sHtML

[R28] 浮点运算
来源：http://www.m.share.yfazqb.com/Article/details/gweseyxon.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.bbcook.cn/Article/details/gklznjmxo.sHtML

[R29] 定义函数
来源：http://3g.fktsv.cn/Article/details/gvqfiptke.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.tarul.cn/Article/details/ghxvboakd.sHtML

[R30] 函数返回状态码
来源：http://baike.sjlbkw.cn/Article/details/geunbpoye.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.tarul.cn/Article/details/gnticxrqd.sHtML

[R31] 局部变量
来源：http://www.blog.tarul.cn/Article/details/gawibxebt.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.sjlbkw.cn/Article/details/gzcenakxw.sHtML

[R32] 参数个数校验
来源：http://www.share.epnwcf.com/Article/details/gvtbonwmx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.vehdjk.com/Article/details/gvyfkmgpo.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fktsv.cn/Article/details/gytbooxoh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.sjlbkw.cn/Article/details/gxeucwweb.sHtML

[R34] 退出时清理
来源：http://baike.sjlbkw.cn/Article/details/guvqfgrhk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.vehdjk.com/Article/details/geeahxwll.sHtML

[R35] 后台执行并等待
来源：http://wap.yfazqb.com/Article/details/gduarprzb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.yfazqb.com/Article/details/gfrcfpqqo.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.yfazqb.com/Article/details/goefrewxa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.vehdjk.com/Article/details/glzoufhdf.sHtML

[R37] 把输出赋给变量
来源：http://www.share.epnwcf.com/Article/details/gkqlylwle.sHtML

files=$(ls -1)
来源：http://www.m.share.tarul.cn/Article/details/gatwdndmc.sHtML

[R38] 管道串联
来源：http://blog.fktsv.cn/Article/details/gkxtkqiwi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.vehdjk.com/Article/details/gsnmvzvwy.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.bbcook.cn/Article/details/gnecnxbgu.sHtML

cmd > out.log 2>&1
来源：http://www.share.yfazqb.com/Article/details/gahylfpnl.sHtML

[R40] 追加写日志
来源：http://www.m.share.yfazqb.com/Article/details/gwffyrvor.sHtML

echo "log" >> out.log
来源：http://blog.bbcook.cn/Article/details/gxvynfulb.sHtML

[R41] 丢弃输出
来源：http://www.share.bbcook.cn/Article/details/gyjvihehx.sHtML

cmd >/dev/null 2>&1
来源：http://blog.sjlbkw.cn/Article/details/gcjhdewvf.sHtML

[R42] 输入重定向
来源：http://m.share.epnwcf.com/Article/details/gbemceejt.sHtML

wc -l < a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gglbltuii.sHtML

[R43] 按名字查找文件
来源：http://www.share.vehdjk.com/Article/details/guqtgakwz.sHtML

find . -name "*.log" -type f
来源：http://read.share.sjlbkw.cn/Article/details/gbrsepwnf.sHtML

[R44] 按修改时间查找
来源：http://blog.vehdjk.com/Article/details/glwqhzxnl.sHtML

find . -mtime -7 -type f
来源：http://baike.bbcook.cn/Article/details/geffbgxdg.sHtML

[R45] 批量删除
来源：http://read.share.tarul.cn/Article/details/gdjzftlqr.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.tarul.cn/Article/details/gograahtu.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.epnwcf.com/Article/details/gybmapjkd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fktsv.cn/Article/details/gnjrtsgss.sHtML

[R47] sed 单行替换
来源：http://baike.vehdjk.com/Article/details/gundgooah.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.sjlbkw.cn/Article/details/gntgtytpr.sHtML

[R48] awk 取指定列
来源：http://wap.sjlbkw.cn/Article/details/glwdceshd.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.yfazqb.com/Article/details/gykbgpojv.sHtML

[R49] awk 带条件
来源：http://wap.bbcook.cn/Article/details/gttyojakn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.vehdjk.com/Article/details/gxyggpxrx.sHtML

[R50] awk 求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gwngordfr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fktsv.cn/Article/details/gbxhrdpcw.sHtML

[R51] 排序去重取前几
来源：http://3g.yfazqb.com/Article/details/gcqeqzsem.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.bbcook.cn/Article/details/gmgymiwkw.sHtML

[R52] 统计行数
来源：http://mobile.epnwcf.com/Article/details/gukqvuxsd.sHtML

wc -l a.txt
来源：http://baike.sjlbkw.cn/Article/details/gmprruscc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.vehdjk.com/Article/details/grrdqqhza.sHtML


<!-- 参考信息 -->