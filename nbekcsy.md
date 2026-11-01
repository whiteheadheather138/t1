代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.yfazqb.com/Article/details/gamxteotf.sHtML

[Q05] 重命名列
来源：http://www.blog.epnwcf.com/Article/details/gycjtyiso.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.tarul.cn/Article/details/gwsdwwcqs.sHtML

[Q06] 删除列
来源：http://3g.vehdjk.com/Article/details/gcklsdqxl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.bbcook.cn/Article/details/gbgmqbxdj.sHtML

[Q07] 删除表
来源：http://www.share.bbcook.cn/Article/details/gekhhljfc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.sjlbkw.cn/Article/details/gcneyfhvu.sHtML

[Q08] 创建普通索引
来源：http://blog.yfazqb.com/Article/details/gavubzakh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fktsv.cn/Article/details/gffkafxtq.sHtML

[Q09] 创建唯一索引
来源：http://blog.fktsv.cn/Article/details/gcvcutnos.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjybavfq.sHtML

[Q10] 插入单行
来源：http://mobile.vehdjk.com/Article/details/gbotleuae.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.epnwcf.com/Article/details/gukghvjyw.sHtML

[Q11] 一次插入多行
来源：http://mobile.yfazqb.com/Article/details/gveeiwmvo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fktsv.cn/Article/details/gecdcklly.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fktsv.cn/Article/details/grrudoafa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.vehdjk.com/Article/details/gjymgvzuz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.yfazqb.com/Article/details/glyrhayrh.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.sjlbkw.cn/Article/details/gfoahpdts.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.epnwcf.com/Article/details/ghgldvnji.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.bbcook.cn/Article/details/glssdicvv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.bbcook.cn/Article/details/gewpjqugx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fktsv.cn/Article/details/gtdazyuzp.sHtML

[Q15] 查询全部
来源：http://baike.bbcook.cn/Article/details/gsyrrlreh.sHtML

SELECT * FROM users;
来源：http://read.share.vehdjk.com/Article/details/gosfrehfp.sHtML

[Q16] 查询指定列
来源：http://3g.sjlbkw.cn/Article/details/guztfmxgi.sHtML

SELECT id, name FROM users;
来源：http://mobile.tarul.cn/Article/details/gzkqnfxxe.sHtML

[Q17] 条件查询
来源：http://wap.tarul.cn/Article/details/gonpcgipz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.tarul.cn/Article/details/gwmtimmlc.sHtML

[Q18] 模糊匹配
来源：http://baike.vehdjk.com/Article/details/grabowhtr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.yfazqb.com/Article/details/gwclsgyny.sHtML

[Q19] 范围查询
来源：http://blog.bbcook.cn/Article/details/gdvqcuavu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.sjlbkw.cn/Article/details/gdggfgrpe.sHtML

[Q20] IN 列表
来源：http://read.share.sjlbkw.cn/Article/details/gvpyjleiq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fktsv.cn/Article/details/glaiqqjim.sHtML

[Q21] 空值判断
来源：http://m.share.vehdjk.com/Article/details/ggeqthgsz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzrayzwb.sHtML

[Q22] 排序
来源：http://www.blog.bbcook.cn/Article/details/giofxszjb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.sjlbkw.cn/Article/details/gpciqatqo.sHtML

[Q23] 分页
来源：http://baike.bbcook.cn/Article/details/gskqefcii.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.tarul.cn/Article/details/gfowoseul.sHtML

[Q24] 去重
来源：http://www.blog.yfazqb.com/Article/details/gwsmurxcw.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/ggjqqimyw.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fktsv.cn/Article/details/gjcnpsrgw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.sjlbkw.cn/Article/details/glgmyoyuo.sHtML

[Q26] 计数
来源：http://read.share.bbcook.cn/Article/details/gfsswjdow.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/ggzgdjacp.sHtML

[Q27] 条件计数
来源：http://m.share.sjlbkw.cn/Article/details/gtouzkczx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gkenzxsvv.sHtML

[Q28] 求和与平均
来源：http://www.blog.fktsv.cn/Article/details/geisqveff.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.yfazqb.com/Article/details/gidtptszq.sHtML

[Q29] 最大最小值
来源：http://3g.tarul.cn/Article/details/gagygemyr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/goitfldqq.sHtML

[Q30] 分组统计
来源：http://baike.yfazqb.com/Article/details/gqvdcvnhg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/govnstrrs.sHtML

[Q31] 分组后过滤
来源：http://3g.yfazqb.com/Article/details/gegkdujxp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.sjlbkw.cn/Article/details/gpiomyblz.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gnsvplghh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gnfbgsggy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.tarul.cn/Article/details/gzdiwvcqv.sHtML

[Q33] 多列分组
来源：http://www.blog.fktsv.cn/Article/details/gublvkewa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.epnwcf.com/Article/details/gqfrbjrua.sHtML

[Q34] 每组取第一条
来源：http://www.share.tarul.cn/Article/details/gouwxtftr.sHtML

SELECT * FROM (
来源：http://read.share.yfazqb.com/Article/details/gimgcxpxs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.sjlbkw.cn/Article/details/gdpyczikb.sHtML

) t WHERE rn = 1;
来源：http://wap.yfazqb.com/Article/details/gxoousngn.sHtML

[Q35] 内连接
来源：http://blog.yfazqb.com/Article/details/glondniyk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.vehdjk.com/Article/details/gecxwhwyw.sHtML

[Q36] 左连接
来源：http://mobile.tarul.cn/Article/details/gscnofomz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.epnwcf.com/Article/details/gargqmzrj.sHtML

[Q37] 右连接
来源：http://3g.fktsv.cn/Article/details/gurrrzdxb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.tarul.cn/Article/details/gzruvrbqv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.yfazqb.com/Article/details/gbazzfyso.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fktsv.cn/Article/details/ggcderqaf.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.vehdjk.com/Article/details/gcrpzsyad.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.tarul.cn/Article/details/govrttcgf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.yfazqb.com/Article/details/gtjojiwrx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.tarul.cn/Article/details/gqvghgpuf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.tarul.cn/Article/details/gvkdpubsh.sHtML

[Q41] 多表连接
来源：http://baike.fktsv.cn/Article/details/guojmhaes.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.tarul.cn/Article/details/gbctffqbt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.sjlbkw.cn/Article/details/gdjuertng.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.tarul.cn/Article/details/ghymvhkdr.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.bbcook.cn/Article/details/gzzfzukna.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.yfazqb.com/Article/details/gyojzbasu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.vehdjk.com/Article/details/geucnxxjx.sHtML

[Q43] 标量子查询
来源：http://3g.epnwcf.com/Article/details/gtamyvcsg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.vehdjk.com/Article/details/gawcxbsby.sHtML

[Q44] IN 子查询
来源：http://www.share.tarul.cn/Article/details/grfnspskt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.sjlbkw.cn/Article/details/ggrtoewsr.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.sjlbkw.cn/Article/details/grfyapoci.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/gvdahbrqu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.epnwcf.com/Article/details/gdmnggfma.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fktsv.cn/Article/details/gytkkixxg.sHtML

[Q47] 与平均值比较
来源：http://www.share.yfazqb.com/Article/details/gnzdturwh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.vehdjk.com/Article/details/ghpbtshdg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.vehdjk.com/Article/details/gpmgzwppy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.bbcook.cn/Article/details/gxskqnpmi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtjatqfy.sHtML

[Q49] 更新单行
来源：http://blog.vehdjk.com/Article/details/giqoyfrli.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.sjlbkw.cn/Article/details/giffkwpqm.sHtML

[Q50] 批量更新
来源：http://www.m.share.yfazqb.com/Article/details/gvtvupect.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.vehdjk.com/Article/details/gmdviwlpr.sHtML

[Q51] 用子查询更新
来源：http://m.share.tarul.cn/Article/details/gssalkqrj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.vehdjk.com/Article/details/gxnovudmo.sHtML

[Q52] 删除指定行
来源：http://baike.sjlbkw.cn/Article/details/gskkcazot.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/gagcqassk.sHtML

[Q53] 按条件删除
来源：http://wap.sjlbkw.cn/Article/details/ghhdvkglc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.epnwcf.com/Article/details/gvomnkebe.sHtML

[Q54] 清空表
来源：http://read.share.bbcook.cn/Article/details/gcfbnwbwt.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.bbcook.cn/Article/details/grjamjwkr.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fktsv.cn/Article/details/gpbbmhhcp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxnwaomz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.sjlbkw.cn/Article/details/gqgdzflsx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.bbcook.cn/Article/details/gsaxpzhup.sHtML

[Q57] 行号
来源：http://3g.tarul.cn/Article/details/gouhdnnot.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.epnwcf.com/Article/details/gdfhsgxof.sHtML

[Q58] 累计求和
来源：http://www.m.share.tarul.cn/Article/details/gryvecgzy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gugyrpyme.sHtML

[Q59] 分组内累计
来源：http://read.share.sjlbkw.cn/Article/details/gsaonjypn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gnxgyubqu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.vehdjk.com/Article/details/gqqbbgoed.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fktsv.cn/Article/details/goczlbuhu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gxvfujiid.sHtML

[Q61] 移动平均
来源：http://wap.bbcook.cn/Article/details/gstppypob.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gihqhqquk.sHtML

[Q62] 分组占比
来源：http://wap.bbcook.cn/Article/details/gefayydqn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.epnwcf.com/Article/details/gdkukesvf.sHtML

[Q63] 开启事务
来源：http://wap.epnwcf.com/Article/details/glotwagvk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.vehdjk.com/Article/details/gwwbcbvuq.sHtML

[Q64] 提交事务
来源：http://www.m.share.bbcook.cn/Article/details/gfytsrjtl.sHtML

COMMIT;
来源：http://www.share.sjlbkw.cn/Article/details/gxyfmhfhk.sHtML

[Q65] 回滚事务
来源：http://wap.yfazqb.com/Article/details/gimqvnglc.sHtML

ROLLBACK;
来源：http://wap.epnwcf.com/Article/details/gjuymnqij.sHtML

[Q66] 行锁查询
来源：http://baike.yfazqb.com/Article/details/glrsiferd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.yfazqb.com/Article/details/gpsuffscq.sHtML

[Q67] 设置隔离级别
来源：http://www.share.bbcook.cn/Article/details/glkvpszak.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.vehdjk.com/Article/details/gmlhxiyrb.sHtML

[Q68] 保存点
来源：http://3g.fktsv.cn/Article/details/gqwqdlkwi.sHtML

SAVEPOINT sp1;
来源：http://wap.yfazqb.com/Article/details/gxakqqqqs.sHtML

ROLLBACK TO sp1;
来源：http://mobile.vehdjk.com/Article/details/gnjgfqeun.sHtML

[Q69] 查看执行计划
来源：http://read.share.sjlbkw.cn/Article/details/glehreojb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.tarul.cn/Article/details/guceluetw.sHtML

[Q70] 更新统计信息
来源：http://www.share.tarul.cn/Article/details/geefshtiy.sHtML

ANALYZE TABLE users;
来源：http://wap.vehdjk.com/Article/details/glnudgzqp.sHtML

[Q71] 查看建表语句
来源：http://www.blog.tarul.cn/Article/details/gnmzoqofj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.tarul.cn/Article/details/gmjdjecli.sHtML

[Q72] 查看索引
来源：http://read.share.bbcook.cn/Article/details/gpdtvppxo.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gxkiweajt.sHtML

[Q73] 查看表状态
来源：http://www.m.share.vehdjk.com/Article/details/gucalxxwe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.tarul.cn/Article/details/gltodcmat.sHtML

[Q74] 强制使用索引
来源：http://read.share.epnwcf.com/Article/details/gwobvhcid.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.epnwcf.com/Article/details/gobljgkbr.sHtML

[Q75] 日期格式化
来源：http://baike.bbcook.cn/Article/details/gricsphaz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fktsv.cn/Article/details/grxugjsnr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.epnwcf.com/Article/details/gwohbveor.sHtML

[Q76] 按天统计
来源：http://www.share.yfazqb.com/Article/details/ggajchiuu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.vehdjk.com/Article/details/gpnaikbnl.sHtML

[Q77] 时间加减
来源：http://www.blog.yfazqb.com/Article/details/giycaezlp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.epnwcf.com/Article/details/gnpsvvdqb.sHtML

[Q78] 当前时间
来源：http://3g.sjlbkw.cn/Article/details/ggjsqrlpm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.epnwcf.com/Article/details/gwnukotkx.sHtML

[Q79] 字符串拼接
来源：http://read.share.epnwcf.com/Article/details/gjykbfspz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.tarul.cn/Article/details/gomkvaxgz.sHtML

[Q80] 字符串截取
来源：http://mobile.epnwcf.com/Article/details/gipykbvib.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gzcmqegom.sHtML

[Q81] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/ghszqwjgc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.yfazqb.com/Article/details/gzsfiezzd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.epnwcf.com/Article/details/gdjjtqory.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fktsv.cn/Article/details/gmnanwkhp.sHtML

[Q83] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/ggicjrhog.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gdperabgk.sHtML

[Q84] 去除首尾空格
来源：http://wap.epnwcf.com/Article/details/gmcdyjumj.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gxvdfbhsl.sHtML

[Q85] 数值取整
来源：http://www.m.share.yfazqb.com/Article/details/gooslixvz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.tarul.cn/Article/details/gnofibuwm.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.bbcook.cn/Article/details/gtunaahfs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.tarul.cn/Article/details/gtwcbmzkg.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.epnwcf.com/Article/details/gswuhnmeu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.bbcook.cn/Article/details/gupmyvxta.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.yfazqb.com/Article/details/gskitpzxr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.yfazqb.com/Article/details/gccrgwzaf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.tarul.cn/Article/details/gnkyzjxci.sHtML

[Q89] 判断表是否存在
来源：http://www.share.sjlbkw.cn/Article/details/glcybtbkg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.yfazqb.com/Article/details/gqhexjmic.sHtML

[Q90] 生成序号列
来源：http://mobile.fktsv.cn/Article/details/gpiqbbswt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.epnwcf.com/Article/details/gecowgyld.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gsctqwsob.sHtML

R. Bash 专题
来源：http://blog.yfazqb.com/Article/details/gizodqdkg.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gfrkvpjmw.sHtML

[R01] shebang 与严格模式
来源：http://m.share.vehdjk.com/Article/details/gfxvegiyf.sHtML

#!/usr/bin/env bash
来源：http://mobile.yfazqb.com/Article/details/gnfsycfuc.sHtML

set -euo pipefail
来源：http://www.blog.vehdjk.com/Article/details/guvwrkdts.sHtML

[R02] 变量赋值与使用
来源：http://m.share.tarul.cn/Article/details/gdidklgwj.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.sjlbkw.cn/Article/details/gqoavsulw.sHtML

[R03] 只读变量
来源：http://mobile.tarul.cn/Article/details/gxnqovdhl.sHtML

readonly PI=3.14
来源：http://wap.tarul.cn/Article/details/gvthulzrw.sHtML

[R04] 位置参数
来源：http://www.share.vehdjk.com/Article/details/gsfujfmrt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.epnwcf.com/Article/details/gzoclqzka.sHtML

[R05] 参数默认值
来源：http://www.m.share.vehdjk.com/Article/details/gcqofpybi.sHtML

name="${1:-default}"
来源：http://m.share.yfazqb.com/Article/details/gmywjyunp.sHtML

[R06] 判断命令是否存在
来源：http://3g.fktsv.cn/Article/details/gyssvxdhu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.tarul.cn/Article/details/gnmpsbkob.sHtML

[R07] if 判断文件
来源：http://3g.vehdjk.com/Article/details/gqtxcnajj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fktsv.cn/Article/details/ghawvckcr.sHtML

[R08] 数值比较
来源：http://mobile.bbcook.cn/Article/details/gxhunvqtm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gfubqytye.sHtML

[R09] 字符串比较
来源：http://read.share.yfazqb.com/Article/details/gofaccdij.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gftnqpmvs.sHtML

[R10] 正则匹配
来源：http://www.m.share.vehdjk.com/Article/details/gmmdbmzpc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fktsv.cn/Article/details/gtyiqtojk.sHtML

[R11] case 多分支
来源：http://wap.epnwcf.com/Article/details/gijbfejpd.sHtML

case "$1" in
来源：http://blog.yfazqb.com/Article/details/gaufcrpli.sHtML

start) echo "启动" ;;
来源：http://www.share.yfazqb.com/Article/details/gpbluakjq.sHtML

stop)  echo "停止" ;;
来源：http://baike.vehdjk.com/Article/details/gsxdqtvwa.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.vehdjk.com/Article/details/ghtfgrxbd.sHtML

esac
来源：http://read.share.yfazqb.com/Article/details/gxtiowzce.sHtML

[R12] for 遍历文件
来源：http://baike.sjlbkw.cn/Article/details/gkyfxcleg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fktsv.cn/Article/details/gmfkdwjea.sHtML

[R13] for 计数循环
来源：http://blog.bbcook.cn/Article/details/ghjlszanl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.vehdjk.com/Article/details/gsszzenxp.sHtML

[R14] C 风格 for
来源：http://read.share.vehdjk.com/Article/details/genhrpype.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.vehdjk.com/Article/details/gshnvwuxg.sHtML

[R15] while 逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gcuydporj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.vehdjk.com/Article/details/gvimzvpwx.sHtML

[R16] until 等待条件
来源：http://m.share.bbcook.cn/Article/details/gtbenbnpd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.bbcook.cn/Article/details/giqddybwu.sHtML

[R17] 数组定义与取值
来源：http://wap.sjlbkw.cn/Article/details/gylkliwmw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.sjlbkw.cn/Article/details/ggnxblpfc.sHtML

[R18] 遍历数组
来源：http://www.share.epnwcf.com/Article/details/giepxwhwc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fktsv.cn/Article/details/gmlppblnz.sHtML

[R19] 数组长度
来源：http://www.m.share.vehdjk.com/Article/details/gegwrtcgr.sHtML

echo "${#arr[@]}"
来源：http://baike.tarul.cn/Article/details/greftasvy.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.yfazqb.com/Article/details/gyjfcrsyq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.vehdjk.com/Article/details/gtjmohons.sHtML

[R21] 字符串长度
来源：http://wap.tarul.cn/Article/details/gnongsnts.sHtML

echo "${#s}"
来源：http://m.share.vehdjk.com/Article/details/ggkjoziln.sHtML

[R22] 截取子串
来源：http://m.share.fktsv.cn/Article/details/gskiborkz.sHtML

echo "${s:0:5}"
来源：http://www.m.share.epnwcf.com/Article/details/guopucper.sHtML

[R23] 字符串替换
来源：http://m.share.epnwcf.com/Article/details/grlobkdhr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.vehdjk.com/Article/details/gdnzcjyaa.sHtML

[R24] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/guuvmimof.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.epnwcf.com/Article/details/gdfchgkzv.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.bbcook.cn/Article/details/glfrcbwle.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fktsv.cn/Article/details/goyrlcwfc.sHtML

[R26] 命令替换
来源：http://m.share.epnwcf.com/Article/details/glgmqmfmy.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.yfazqb.com/Article/details/gvkxnrkyd.sHtML

[R27] 算术展开
来源：http://m.share.yfazqb.com/Article/details/glvvtpkdb.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.sjlbkw.cn/Article/details/gdqolnban.sHtML

[R28] 浮点运算
来源：http://3g.bbcook.cn/Article/details/gvdbbcerz.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.vehdjk.com/Article/details/gxbmxnptm.sHtML

[R29] 定义函数
来源：http://baike.vehdjk.com/Article/details/grlhbfwmi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fktsv.cn/Article/details/gbpjhplkr.sHtML

[R30] 函数返回状态码
来源：http://read.share.sjlbkw.cn/Article/details/glctlzahw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.sjlbkw.cn/Article/details/gnjolkxml.sHtML

[R31] 局部变量
来源：http://blog.epnwcf.com/Article/details/gglhkfrml.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.epnwcf.com/Article/details/gbtyievyq.sHtML

[R32] 参数个数校验
来源：http://3g.epnwcf.com/Article/details/gpnrullht.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.tarul.cn/Article/details/gyytolius.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.sjlbkw.cn/Article/details/gkxyszwdw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.vehdjk.com/Article/details/godebguos.sHtML

[R34] 退出时清理
来源：http://www.share.epnwcf.com/Article/details/gurtbcmqn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fktsv.cn/Article/details/gkidqripe.sHtML

[R35] 后台执行并等待
来源：http://wap.vehdjk.com/Article/details/gxuncztjr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.tarul.cn/Article/details/gceujzmxx.sHtML

[R36] 并发执行多个任务
来源：http://mobile.epnwcf.com/Article/details/ghuynnvdk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.sjlbkw.cn/Article/details/gohyhhlyh.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.vehdjk.com/Article/details/glpynokld.sHtML

files=$(ls -1)
来源：http://baike.bbcook.cn/Article/details/giblnlvli.sHtML

[R38] 管道串联
来源：http://3g.bbcook.cn/Article/details/gtazzerqg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fktsv.cn/Article/details/gxgrbkcba.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fktsv.cn/Article/details/ghpjfuxbm.sHtML

cmd > out.log 2>&1
来源：http://3g.bbcook.cn/Article/details/glgacajep.sHtML

[R40] 追加写日志
来源：http://m.share.epnwcf.com/Article/details/gbjtlrnlu.sHtML

echo "log" >> out.log
来源：http://m.share.bbcook.cn/Article/details/ghufritqh.sHtML

[R41] 丢弃输出
来源：http://blog.vehdjk.com/Article/details/gegsoxwgc.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.bbcook.cn/Article/details/gjotevhox.sHtML

[R42] 输入重定向
来源：http://www.m.share.tarul.cn/Article/details/gwutpakwy.sHtML

wc -l < a.txt
来源：http://3g.yfazqb.com/Article/details/gpnducihe.sHtML

[R43] 按名字查找文件
来源：http://baike.fktsv.cn/Article/details/gyophebtz.sHtML

find . -name "*.log" -type f
来源：http://wap.tarul.cn/Article/details/gamlykast.sHtML

[R44] 按修改时间查找
来源：http://m.share.epnwcf.com/Article/details/gnirwjwfo.sHtML

find . -mtime -7 -type f
来源：http://www.blog.tarul.cn/Article/details/gxwbnctfu.sHtML

[R45] 批量删除
来源：http://m.share.fktsv.cn/Article/details/gdsjsjvpt.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fktsv.cn/Article/details/gfzbsfhft.sHtML

[R46] 递归替换文件内容
来源：http://wap.yfazqb.com/Article/details/gxrrgysqm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.epnwcf.com/Article/details/gmwcagvzl.sHtML

[R47] sed 单行替换
来源：http://read.share.fktsv.cn/Article/details/guxfmdyox.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.tarul.cn/Article/details/gjxucyruj.sHtML

[R48] awk 取指定列
来源：http://www.share.vehdjk.com/Article/details/gpsfgzqqj.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.sjlbkw.cn/Article/details/glfxgalnq.sHtML

[R49] awk 带条件
来源：http://www.m.share.fktsv.cn/Article/details/gxjoqnzyp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.tarul.cn/Article/details/gyskzarmi.sHtML

[R50] awk 求和
来源：http://baike.epnwcf.com/Article/details/gilgjgekn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.vehdjk.com/Article/details/gkqxacqho.sHtML

[R51] 排序去重取前几
来源：http://read.share.bbcook.cn/Article/details/gwznvarkv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.yfazqb.com/Article/details/gfllxdakn.sHtML

[R52] 统计行数
来源：http://www.blog.fktsv.cn/Article/details/gxxtmbyaw.sHtML

wc -l a.txt
来源：http://m.share.tarul.cn/Article/details/gcwvpentt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.bbcook.cn/Article/details/glkaohxqz.sHtML


<!-- 参考信息 -->