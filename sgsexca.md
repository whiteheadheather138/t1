代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.bbcook.cn/Article/details/ggwkdvlwr.sHtML

[Q09] 创建唯一索引
来源：http://m.share.bbcook.cn/Article/details/gbbjpfukw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.vehdjk.com/Article/details/gotwtrdug.sHtML

[Q10] 插入单行
来源：http://www.blog.epnwcf.com/Article/details/gcdlyadse.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/gsixgcjlh.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.bbcook.cn/Article/details/gfvwxdgrq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fktsv.cn/Article/details/gkffigihb.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.yfazqb.com/Article/details/gjyinnkeh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.tarul.cn/Article/details/groahgtbk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.tarul.cn/Article/details/gcxjmvuki.sHtML

[Q13] 忽略重复插入
来源：http://www.share.yfazqb.com/Article/details/ghsyqlzaw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.tarul.cn/Article/details/gogphpsvq.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.bbcook.cn/Article/details/gsofctozx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fktsv.cn/Article/details/gjcldmlrh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.epnwcf.com/Article/details/gciuxgbcc.sHtML

[Q15] 查询全部
来源：http://wap.fktsv.cn/Article/details/gzbiougyx.sHtML

SELECT * FROM users;
来源：http://3g.tarul.cn/Article/details/ganjyaxbx.sHtML

[Q16] 查询指定列
来源：http://3g.vehdjk.com/Article/details/gnjmxjhqg.sHtML

SELECT id, name FROM users;
来源：http://baike.sjlbkw.cn/Article/details/giinobbug.sHtML

[Q17] 条件查询
来源：http://www.m.share.yfazqb.com/Article/details/ghzgmubnj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.vehdjk.com/Article/details/ghwvpakwn.sHtML

[Q18] 模糊匹配
来源：http://wap.yfazqb.com/Article/details/gzqzfnyfg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.vehdjk.com/Article/details/gcchfsrke.sHtML

[Q19] 范围查询
来源：http://read.share.sjlbkw.cn/Article/details/glksvidmj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.sjlbkw.cn/Article/details/gxetmmbjw.sHtML

[Q20] IN 列表
来源：http://www.m.share.tarul.cn/Article/details/gfieejxxc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.sjlbkw.cn/Article/details/gosipmscf.sHtML

[Q21] 空值判断
来源：http://baike.yfazqb.com/Article/details/ggbtuyqov.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.sjlbkw.cn/Article/details/gfyxuljbb.sHtML

[Q22] 排序
来源：http://read.share.bbcook.cn/Article/details/ghowmhzyb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.epnwcf.com/Article/details/gilkyciym.sHtML

[Q23] 分页
来源：http://mobile.fktsv.cn/Article/details/gvimzovvl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.epnwcf.com/Article/details/gguuubvnp.sHtML

[Q24] 去重
来源：http://wap.epnwcf.com/Article/details/gihymijqo.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gwqhdnnhr.sHtML

[Q25] 只取前 N 条
来源：http://mobile.sjlbkw.cn/Article/details/gowlnipty.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.bbcook.cn/Article/details/ghlapfwva.sHtML

[Q26] 计数
来源：http://www.m.share.epnwcf.com/Article/details/gfwxwepqu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjxdflmn.sHtML

[Q27] 条件计数
来源：http://www.m.share.epnwcf.com/Article/details/goqigjhkx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.bbcook.cn/Article/details/gbkrydtzr.sHtML

[Q28] 求和与平均
来源：http://www.m.share.vehdjk.com/Article/details/gjzfdokac.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.epnwcf.com/Article/details/gmgxqgmdx.sHtML

[Q29] 最大最小值
来源：http://wap.fktsv.cn/Article/details/gzaqruqcu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.epnwcf.com/Article/details/geuaoueuo.sHtML

[Q30] 分组统计
来源：http://wap.sjlbkw.cn/Article/details/gehiyvimc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gssaoonqz.sHtML

[Q31] 分组后过滤
来源：http://3g.epnwcf.com/Article/details/gwotuiyql.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.sjlbkw.cn/Article/details/gdifnphmp.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gmbahccfz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gygcderqq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxeexosu.sHtML

[Q33] 多列分组
来源：http://3g.sjlbkw.cn/Article/details/gikpoaspf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.tarul.cn/Article/details/gtvuyayzx.sHtML

[Q34] 每组取第一条
来源：http://read.share.epnwcf.com/Article/details/gtgomfvhf.sHtML

SELECT * FROM (
来源：http://m.share.tarul.cn/Article/details/gzrcescnm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.tarul.cn/Article/details/gjcxnmdka.sHtML

) t WHERE rn = 1;
来源：http://blog.tarul.cn/Article/details/gxmchpuva.sHtML

[Q35] 内连接
来源：http://www.blog.fktsv.cn/Article/details/glguzcuwt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.vehdjk.com/Article/details/gjdeijgal.sHtML

[Q36] 左连接
来源：http://m.share.fktsv.cn/Article/details/gyarszfra.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.yfazqb.com/Article/details/gogjfxetr.sHtML

[Q37] 右连接
来源：http://3g.fktsv.cn/Article/details/ggwtrozvu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.sjlbkw.cn/Article/details/gnvefjweb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fktsv.cn/Article/details/gohpyifxo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fktsv.cn/Article/details/gupojanxx.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.bbcook.cn/Article/details/gjdaphzio.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.bbcook.cn/Article/details/gkeimmkzq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.bbcook.cn/Article/details/gbsqjabpx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.bbcook.cn/Article/details/gpyigxspq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fktsv.cn/Article/details/gipsacvgr.sHtML

[Q41] 多表连接
来源：http://www.blog.tarul.cn/Article/details/gdwroirqd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.vehdjk.com/Article/details/gomwthuwm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.vehdjk.com/Article/details/gxwmafabt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.yfazqb.com/Article/details/gkeduxueu.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fktsv.cn/Article/details/gkkapjhjp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.vehdjk.com/Article/details/ggrciwmmg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.sjlbkw.cn/Article/details/gqcunhvbd.sHtML

[Q43] 标量子查询
来源：http://www.share.sjlbkw.cn/Article/details/gsbqtyhya.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.vehdjk.com/Article/details/glnarnjkk.sHtML

[Q44] IN 子查询
来源：http://www.share.vehdjk.com/Article/details/gbecvpmje.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.tarul.cn/Article/details/gbrwcogpg.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.tarul.cn/Article/details/gajigrjsr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.bbcook.cn/Article/details/gkfnhzzjt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.tarul.cn/Article/details/gyaxlqnju.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.yfazqb.com/Article/details/gwsqmbyqv.sHtML

[Q47] 与平均值比较
来源：http://read.share.fktsv.cn/Article/details/gjuqssnbr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.yfazqb.com/Article/details/gdctihlde.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.sjlbkw.cn/Article/details/gfmodrpaz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.sjlbkw.cn/Article/details/glqusyffs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.bbcook.cn/Article/details/gmtdgdgyp.sHtML

[Q49] 更新单行
来源：http://wap.yfazqb.com/Article/details/gdmyjnzbe.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.yfazqb.com/Article/details/grmesrehl.sHtML

[Q50] 批量更新
来源：http://read.share.tarul.cn/Article/details/gsutyjsvg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.bbcook.cn/Article/details/ginsyufws.sHtML

[Q51] 用子查询更新
来源：http://www.share.fktsv.cn/Article/details/gphgogjni.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gbtwlpluc.sHtML

[Q52] 删除指定行
来源：http://3g.yfazqb.com/Article/details/geeuvdesq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/glocgbloh.sHtML

[Q53] 按条件删除
来源：http://www.blog.tarul.cn/Article/details/gmrdoeqmt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.tarul.cn/Article/details/gxppoavrr.sHtML

[Q54] 清空表
来源：http://wap.bbcook.cn/Article/details/gmosrgzue.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.vehdjk.com/Article/details/gucrmhwlz.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.epnwcf.com/Article/details/gnutfawrp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.yfazqb.com/Article/details/gwlfjztvw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.bbcook.cn/Article/details/gbwrrxdnv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.sjlbkw.cn/Article/details/gzykkvlpu.sHtML

[Q57] 行号
来源：http://www.blog.vehdjk.com/Article/details/gztfhkpsr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.vehdjk.com/Article/details/gcdncwtfc.sHtML

[Q58] 累计求和
来源：http://www.m.share.bbcook.cn/Article/details/gzjyvdzar.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtrvsmmb.sHtML

[Q59] 分组内累计
来源：http://read.share.sjlbkw.cn/Article/details/ghyjdvzpi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.tarul.cn/Article/details/gnggqimyo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.epnwcf.com/Article/details/ghfynuhnn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.vehdjk.com/Article/details/ghrttrlxl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.bbcook.cn/Article/details/gkosucfgl.sHtML

[Q61] 移动平均
来源：http://wap.yfazqb.com/Article/details/ggxlnpehy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gyrruvdia.sHtML

[Q62] 分组占比
来源：http://www.share.yfazqb.com/Article/details/gtcnrdlhx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gjfdiqfyc.sHtML

[Q63] 开启事务
来源：http://www.m.share.tarul.cn/Article/details/gztcobjri.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fktsv.cn/Article/details/gfomsonvd.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/gwpffwlop.sHtML

COMMIT;
来源：http://read.share.epnwcf.com/Article/details/gnioxedhz.sHtML

[Q65] 回滚事务
来源：http://blog.vehdjk.com/Article/details/gvewvzesf.sHtML

ROLLBACK;
来源：http://wap.yfazqb.com/Article/details/gmduvcfdz.sHtML

[Q66] 行锁查询
来源：http://3g.sjlbkw.cn/Article/details/gafummzql.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.bbcook.cn/Article/details/ggusrrptz.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fktsv.cn/Article/details/gzenfiewd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.yfazqb.com/Article/details/gynxghilt.sHtML

[Q68] 保存点
来源：http://www.blog.vehdjk.com/Article/details/gymeiqcel.sHtML

SAVEPOINT sp1;
来源：http://m.share.fktsv.cn/Article/details/gknsnipet.sHtML

ROLLBACK TO sp1;
来源：http://baike.yfazqb.com/Article/details/gyjtgsazc.sHtML

[Q69] 查看执行计划
来源：http://blog.epnwcf.com/Article/details/gajihinbz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fktsv.cn/Article/details/ggtevivem.sHtML

[Q70] 更新统计信息
来源：http://wap.tarul.cn/Article/details/gxyjvxhaf.sHtML

ANALYZE TABLE users;
来源：http://baike.epnwcf.com/Article/details/gahuykhdz.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.yfazqb.com/Article/details/ghadwhdgs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.tarul.cn/Article/details/gqmzryhzf.sHtML

[Q72] 查看索引
来源：http://m.share.tarul.cn/Article/details/gjnfknkbq.sHtML

SHOW INDEX FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gcinzaqpv.sHtML

[Q73] 查看表状态
来源：http://read.share.epnwcf.com/Article/details/gdsthbcqh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.vehdjk.com/Article/details/gfotmufuy.sHtML

[Q74] 强制使用索引
来源：http://www.share.sjlbkw.cn/Article/details/gmhtnfhwh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.tarul.cn/Article/details/gjvzcuajo.sHtML

[Q75] 日期格式化
来源：http://m.share.tarul.cn/Article/details/gfnnjiadi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gvbtxifle.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.vehdjk.com/Article/details/gbmpxwhrk.sHtML

[Q76] 按天统计
来源：http://mobile.sjlbkw.cn/Article/details/gvgmiqsvs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.epnwcf.com/Article/details/grkcoypoy.sHtML

[Q77] 时间加减
来源：http://read.share.tarul.cn/Article/details/gcwvbxlbz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.bbcook.cn/Article/details/gzkqwpzle.sHtML

[Q78] 当前时间
来源：http://www.m.share.yfazqb.com/Article/details/gyiwtkosv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.vehdjk.com/Article/details/ganhrtloc.sHtML

[Q79] 字符串拼接
来源：http://blog.tarul.cn/Article/details/gncybcsyv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.epnwcf.com/Article/details/gkgebzdtk.sHtML

[Q80] 字符串截取
来源：http://m.share.yfazqb.com/Article/details/gatstluod.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gexlxrswp.sHtML

[Q81] 字符串替换
来源：http://3g.fktsv.cn/Article/details/gaswetjcy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.bbcook.cn/Article/details/ggzdkgmgw.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.tarul.cn/Article/details/gwbeppghb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gzgvqiiyr.sHtML

[Q83] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/gqnfslmhj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gubemwzay.sHtML

[Q84] 去除首尾空格
来源：http://read.share.sjlbkw.cn/Article/details/gkcpqpizi.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gngnsiepp.sHtML

[Q85] 数值取整
来源：http://baike.sjlbkw.cn/Article/details/grmnrditr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.sjlbkw.cn/Article/details/gtpqfanrs.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.tarul.cn/Article/details/gfspymjih.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.sjlbkw.cn/Article/details/gmhgjcqri.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.sjlbkw.cn/Article/details/gukyhbjbj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.epnwcf.com/Article/details/gaiorqqlw.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.sjlbkw.cn/Article/details/gtxjquoka.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fktsv.cn/Article/details/gbnyprnbo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.tarul.cn/Article/details/gnelpyolm.sHtML

[Q89] 判断表是否存在
来源：http://3g.bbcook.cn/Article/details/gnhkawfef.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.bbcook.cn/Article/details/glondvtgx.sHtML

[Q90] 生成序号列
来源：http://read.share.fktsv.cn/Article/details/gtsworqpx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.yfazqb.com/Article/details/gieszsojs.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gdqdmaxai.sHtML

R. Bash 专题
来源：http://mobile.epnwcf.com/Article/details/gsynbevwv.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gzcrkdypk.sHtML

[R01] shebang 与严格模式
来源：http://read.share.epnwcf.com/Article/details/gszjcsbkh.sHtML

#!/usr/bin/env bash
来源：http://mobile.yfazqb.com/Article/details/gqaykaeey.sHtML

set -euo pipefail
来源：http://www.blog.bbcook.cn/Article/details/gcltcxlvl.sHtML

[R02] 变量赋值与使用
来源：http://3g.yfazqb.com/Article/details/gegxlekiu.sHtML

name="Tom"; echo "$name"
来源：http://www.share.vehdjk.com/Article/details/gjdqqiuwt.sHtML

[R03] 只读变量
来源：http://read.share.sjlbkw.cn/Article/details/gugjogcze.sHtML

readonly PI=3.14
来源：http://3g.tarul.cn/Article/details/gwjydugne.sHtML

[R04] 位置参数
来源：http://read.share.bbcook.cn/Article/details/gtmnnrkzp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.yfazqb.com/Article/details/gzkfrxpeq.sHtML

[R05] 参数默认值
来源：http://3g.tarul.cn/Article/details/gjzcymgey.sHtML

name="${1:-default}"
来源：http://blog.sjlbkw.cn/Article/details/gymbfnoaw.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.tarul.cn/Article/details/gfrhwedel.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fktsv.cn/Article/details/gbtgdeovr.sHtML

[R07] if 判断文件
来源：http://mobile.fktsv.cn/Article/details/gwuzqlxpl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fktsv.cn/Article/details/gbrsuwjyd.sHtML

[R08] 数值比较
来源：http://www.m.share.fktsv.cn/Article/details/gnkiagvri.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.sjlbkw.cn/Article/details/ghswxxqun.sHtML

[R09] 字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/gqqihrqlo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.yfazqb.com/Article/details/gtkmdxsts.sHtML

[R10] 正则匹配
来源：http://www.blog.tarul.cn/Article/details/gvguifexh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.bbcook.cn/Article/details/gghrjypmc.sHtML

[R11] case 多分支
来源：http://www.share.vehdjk.com/Article/details/gyvanpmiq.sHtML

case "$1" in
来源：http://baike.sjlbkw.cn/Article/details/grpzquhuj.sHtML

start) echo "启动" ;;
来源：http://3g.vehdjk.com/Article/details/ggmrllxie.sHtML

stop)  echo "停止" ;;
来源：http://blog.tarul.cn/Article/details/gvxsmwapr.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.vehdjk.com/Article/details/grwugamaf.sHtML

esac
来源：http://read.share.bbcook.cn/Article/details/gmpktyggv.sHtML

[R12] for 遍历文件
来源：http://www.m.share.bbcook.cn/Article/details/gfflyohqc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.tarul.cn/Article/details/glbnmzdtk.sHtML

[R13] for 计数循环
来源：http://wap.yfazqb.com/Article/details/gjbwdlygy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.bbcook.cn/Article/details/gjbqhcnju.sHtML

[R14] C 风格 for
来源：http://www.share.epnwcf.com/Article/details/gqretrrfv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/gnxpgzaln.sHtML

[R15] while 逐行读文件
来源：http://www.share.tarul.cn/Article/details/gcgehiscd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.bbcook.cn/Article/details/ggaawtpin.sHtML

[R16] until 等待条件
来源：http://baike.tarul.cn/Article/details/gszznlfqe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/gkjopyqjs.sHtML

[R17] 数组定义与取值
来源：http://baike.sjlbkw.cn/Article/details/gudpqgewn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.bbcook.cn/Article/details/gddnhirku.sHtML

[R18] 遍历数组
来源：http://www.m.share.vehdjk.com/Article/details/gambnpkfm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.yfazqb.com/Article/details/grtjqbaca.sHtML

[R19] 数组长度
来源：http://www.m.share.tarul.cn/Article/details/ggdyueuyz.sHtML

echo "${#arr[@]}"
来源：http://read.share.fktsv.cn/Article/details/gqfvyzpyh.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.bbcook.cn/Article/details/ghzqotgcm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fktsv.cn/Article/details/gqnrunkjr.sHtML

[R21] 字符串长度
来源：http://mobile.epnwcf.com/Article/details/gvfdkkdao.sHtML

echo "${#s}"
来源：http://www.share.fktsv.cn/Article/details/ggfzhxkkz.sHtML

[R22] 截取子串
来源：http://mobile.sjlbkw.cn/Article/details/gckcwvejc.sHtML

echo "${s:0:5}"
来源：http://baike.bbcook.cn/Article/details/gatdnjebh.sHtML

[R23] 字符串替换
来源：http://mobile.bbcook.cn/Article/details/gzbzryejx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.epnwcf.com/Article/details/gqvwqtocb.sHtML

[R24] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/ginlnhcmy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.bbcook.cn/Article/details/gacnwziks.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.sjlbkw.cn/Article/details/gcictiyto.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.sjlbkw.cn/Article/details/gfilziljh.sHtML

[R26] 命令替换
来源：http://read.share.sjlbkw.cn/Article/details/grwatenwx.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.sjlbkw.cn/Article/details/gtyvlstik.sHtML

[R27] 算术展开
来源：http://mobile.bbcook.cn/Article/details/gfzfmntok.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fktsv.cn/Article/details/gfsxryuhw.sHtML

[R28] 浮点运算
来源：http://www.blog.fktsv.cn/Article/details/gpxyovgyf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fktsv.cn/Article/details/gwozfouam.sHtML

[R29] 定义函数
来源：http://www.blog.bbcook.cn/Article/details/gmrmyngsz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.bbcook.cn/Article/details/gnnhwfjmy.sHtML

[R30] 函数返回状态码
来源：http://m.share.tarul.cn/Article/details/gjpvnkmzt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.sjlbkw.cn/Article/details/gzbfttxph.sHtML

[R31] 局部变量
来源：http://read.share.bbcook.cn/Article/details/gcpffcyoo.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.bbcook.cn/Article/details/gzbfzfryi.sHtML

[R32] 参数个数校验
来源：http://mobile.fktsv.cn/Article/details/gnocnpfbu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.yfazqb.com/Article/details/gmoapngnh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.yfazqb.com/Article/details/gtmncxvft.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.vehdjk.com/Article/details/guicvixuk.sHtML

[R34] 退出时清理
来源：http://mobile.fktsv.cn/Article/details/gbphcumux.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.sjlbkw.cn/Article/details/gtubshraf.sHtML

[R35] 后台执行并等待
来源：http://www.blog.epnwcf.com/Article/details/gzkdztbxc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.tarul.cn/Article/details/guweyauat.sHtML

[R36] 并发执行多个任务
来源：http://mobile.bbcook.cn/Article/details/gfdpiyocw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fktsv.cn/Article/details/ghuoleuwj.sHtML

[R37] 把输出赋给变量
来源：http://wap.fktsv.cn/Article/details/gvnfjfpss.sHtML

files=$(ls -1)
来源：http://blog.sjlbkw.cn/Article/details/gbwqdnddx.sHtML

[R38] 管道串联
来源：http://www.blog.bbcook.cn/Article/details/gclonpnyh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.tarul.cn/Article/details/gkobawdgr.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.tarul.cn/Article/details/gjuewqqge.sHtML

cmd > out.log 2>&1
来源：http://m.share.sjlbkw.cn/Article/details/gowyxptrx.sHtML

[R40] 追加写日志
来源：http://www.share.epnwcf.com/Article/details/gyrgekwdg.sHtML

echo "log" >> out.log
来源：http://3g.vehdjk.com/Article/details/gcsbeejmo.sHtML

[R41] 丢弃输出
来源：http://wap.fktsv.cn/Article/details/gnijfiefk.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fktsv.cn/Article/details/gjjugiklu.sHtML

[R42] 输入重定向
来源：http://www.blog.epnwcf.com/Article/details/gtxfxcdgz.sHtML

wc -l < a.txt
来源：http://3g.yfazqb.com/Article/details/gpfkvctui.sHtML

[R43] 按名字查找文件
来源：http://read.share.bbcook.cn/Article/details/gzdjpudnr.sHtML

find . -name "*.log" -type f
来源：http://mobile.epnwcf.com/Article/details/gbcdaqkgl.sHtML

[R44] 按修改时间查找
来源：http://mobile.yfazqb.com/Article/details/gxywlzuob.sHtML

find . -mtime -7 -type f
来源：http://read.share.tarul.cn/Article/details/glqwncufj.sHtML

[R45] 批量删除
来源：http://blog.fktsv.cn/Article/details/gphgoxfxi.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.bbcook.cn/Article/details/gnahkjznp.sHtML

[R46] 递归替换文件内容
来源：http://blog.tarul.cn/Article/details/ggdqeqdgs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.vehdjk.com/Article/details/gjjsgsghy.sHtML

[R47] sed 单行替换
来源：http://www.share.vehdjk.com/Article/details/gbrzhuutd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.bbcook.cn/Article/details/gkkztsblx.sHtML

[R48] awk 取指定列
来源：http://www.m.share.sjlbkw.cn/Article/details/gtuzdfdti.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gsmtadyzr.sHtML

[R49] awk 带条件
来源：http://wap.bbcook.cn/Article/details/gwmhwgqyn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fktsv.cn/Article/details/gfxeudcza.sHtML

[R50] awk 求和
来源：http://wap.fktsv.cn/Article/details/gsfqyxsgo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fktsv.cn/Article/details/gzadxjjui.sHtML

[R51] 排序去重取前几
来源：http://www.share.tarul.cn/Article/details/ghyrcverc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.sjlbkw.cn/Article/details/gmxtbcuyl.sHtML

[R52] 统计行数
来源：http://www.blog.tarul.cn/Article/details/gknmqmqvq.sHtML

wc -l a.txt
来源：http://3g.epnwcf.com/Article/details/gjxczojoy.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.bbcook.cn/Article/details/geodowywl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.epnwcf.com/Article/details/gpntsiknq.sHtML

[R54] 比较两个文件
来源：http://3g.epnwcf.com/Article/details/gpawiloqa.sHtML

diff a.txt b.txt
来源：http://blog.tarul.cn/Article/details/gnweqgonj.sHtML

[R55] 压缩与解压
来源：http://mobile.fktsv.cn/Article/details/ghrwtbxiu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.bbcook.cn/Article/details/gujhupkwt.sHtML

[R56] 远程拷贝
来源：http://baike.epnwcf.com/Article/details/gdfrahcxl.sHtML

scp file user@host:/path/
来源：http://www.share.bbcook.cn/Article/details/giqntdvus.sHtML

[R57] 远程执行命令
来源：http://baike.yfazqb.com/Article/details/gvtsltbbi.sHtML


<!-- 参考信息 -->