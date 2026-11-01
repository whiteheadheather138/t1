代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fktsv.cn/Article/details/gtkzahfan.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.tarul.cn/Article/details/gwbfflbgq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.vehdjk.com/Article/details/gtwajklqz.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.vehdjk.com/Article/details/gmefaitxy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.vehdjk.com/Article/details/gdvgnrlkn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.bbcook.cn/Article/details/gytzowpqe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.epnwcf.com/Article/details/gvdfykeoi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fktsv.cn/Article/details/gsegenjjj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fktsv.cn/Article/details/gtndnjtry.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.yfazqb.com/Article/details/ggwfynqgy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.epnwcf.com/Article/details/glqwwflmw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.bbcook.cn/Article/details/gjnprppnv.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gmwjtaezz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.bbcook.cn/Article/details/germpctek.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/goohqvkgu.sHtML

[Q01] 创建表
来源：http://www.m.share.tarul.cn/Article/details/ggnfawtez.sHtML

CREATE TABLE users (
来源：http://wap.yfazqb.com/Article/details/gtgtpvxnb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.epnwcf.com/Article/details/gzprxvjvl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fktsv.cn/Article/details/gfcupgtcw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.vehdjk.com/Article/details/gigbhddhe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.yfazqb.com/Article/details/gyzelspbh.sHtML

);
来源：http://www.m.share.bbcook.cn/Article/details/gusvozplp.sHtML

[Q02] 创建带外键的表
来源：http://blog.tarul.cn/Article/details/gktbinslf.sHtML

CREATE TABLE orders (
来源：http://wap.yfazqb.com/Article/details/gzioxbfkr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.tarul.cn/Article/details/gsoalrkfk.sHtML

user_id INT NOT NULL,
来源：http://read.share.epnwcf.com/Article/details/ggpztxgho.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.tarul.cn/Article/details/gattprarj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.epnwcf.com/Article/details/gkbphbvcg.sHtML

);
来源：http://m.share.fktsv.cn/Article/details/gifyfdhjh.sHtML

[Q03] 增加列
来源：http://read.share.sjlbkw.cn/Article/details/gqarvahah.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.epnwcf.com/Article/details/gphjxjzit.sHtML

[Q04] 修改列类型
来源：http://baike.bbcook.cn/Article/details/gfdmkyewe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.vehdjk.com/Article/details/gaxjxkrss.sHtML

[Q05] 重命名列
来源：http://baike.tarul.cn/Article/details/ggixcgbbg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fktsv.cn/Article/details/gvsawueyw.sHtML

[Q06] 删除列
来源：http://www.m.share.epnwcf.com/Article/details/gbofvhixk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.vehdjk.com/Article/details/gealfkdno.sHtML

[Q07] 删除表
来源：http://baike.bbcook.cn/Article/details/gwojpipyw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.vehdjk.com/Article/details/gfzlieqli.sHtML

[Q08] 创建普通索引
来源：http://wap.fktsv.cn/Article/details/ggguwmfsh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.tarul.cn/Article/details/gxsemdcrm.sHtML

[Q09] 创建唯一索引
来源：http://read.share.vehdjk.com/Article/details/gcrrwrziy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.sjlbkw.cn/Article/details/gillwmxjh.sHtML

[Q10] 插入单行
来源：http://www.share.yfazqb.com/Article/details/gopqlotjl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/gnfvrmfjc.sHtML

[Q11] 一次插入多行
来源：http://baike.tarul.cn/Article/details/gjyyerats.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.vehdjk.com/Article/details/gsrkjdrzp.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.yfazqb.com/Article/details/gclhbvkgb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.epnwcf.com/Article/details/gddcjqvxf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.bbcook.cn/Article/details/gtmhqbgeo.sHtML

[Q13] 忽略重复插入
来源：http://blog.epnwcf.com/Article/details/gjrrpggck.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.vehdjk.com/Article/details/gbfmpooin.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.yfazqb.com/Article/details/gqejsjnph.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.tarul.cn/Article/details/gwhjlqtqc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.sjlbkw.cn/Article/details/guvnfrfjt.sHtML

[Q15] 查询全部
来源：http://baike.tarul.cn/Article/details/ghwyhwwzy.sHtML

SELECT * FROM users;
来源：http://www.share.yfazqb.com/Article/details/gmnygdcsn.sHtML

[Q16] 查询指定列
来源：http://www.blog.bbcook.cn/Article/details/gossdbjle.sHtML

SELECT id, name FROM users;
来源：http://mobile.yfazqb.com/Article/details/gtmhpzvie.sHtML

[Q17] 条件查询
来源：http://mobile.fktsv.cn/Article/details/gzhrwzhtx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.yfazqb.com/Article/details/gbyvngejv.sHtML

[Q18] 模糊匹配
来源：http://baike.epnwcf.com/Article/details/govwrzykm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.bbcook.cn/Article/details/gmigqsvjp.sHtML

[Q19] 范围查询
来源：http://read.share.bbcook.cn/Article/details/gyowuigeh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.tarul.cn/Article/details/gufkleflz.sHtML

[Q20] IN 列表
来源：http://www.m.share.fktsv.cn/Article/details/glsecabqf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.vehdjk.com/Article/details/gjkodllfd.sHtML

[Q21] 空值判断
来源：http://www.share.tarul.cn/Article/details/glodsatev.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fktsv.cn/Article/details/gcwkdnpvv.sHtML

[Q22] 排序
来源：http://www.share.epnwcf.com/Article/details/gmbzhpmyu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.yfazqb.com/Article/details/gddnnslcl.sHtML

[Q23] 分页
来源：http://blog.bbcook.cn/Article/details/gnitqyhua.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.epnwcf.com/Article/details/gojwxfqku.sHtML

[Q24] 去重
来源：http://3g.bbcook.cn/Article/details/gmpjlzsyz.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gorhuufiy.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.vehdjk.com/Article/details/gpffuvupx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.tarul.cn/Article/details/gcmycelrf.sHtML

[Q26] 计数
来源：http://wap.yfazqb.com/Article/details/gxijxctll.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.tarul.cn/Article/details/ggcbjjnxr.sHtML

[Q27] 条件计数
来源：http://www.blog.yfazqb.com/Article/details/gcwmdcojx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fktsv.cn/Article/details/gxnsilncf.sHtML

[Q28] 求和与平均
来源：http://wap.bbcook.cn/Article/details/gwpbwltbf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gttnonjrt.sHtML

[Q29] 最大最小值
来源：http://read.share.vehdjk.com/Article/details/gradwbtsl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gjxlounqn.sHtML

[Q30] 分组统计
来源：http://read.share.sjlbkw.cn/Article/details/gigolhrcc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/ghqodxiyi.sHtML

[Q31] 分组后过滤
来源：http://baike.fktsv.cn/Article/details/ggcmzehla.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.yfazqb.com/Article/details/gdexiptwf.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fktsv.cn/Article/details/gtgycixvt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gkckwoyxh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.epnwcf.com/Article/details/gcinazfrz.sHtML

[Q33] 多列分组
来源：http://m.share.vehdjk.com/Article/details/gdwgfjlwo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.sjlbkw.cn/Article/details/ggukdlzyu.sHtML

[Q34] 每组取第一条
来源：http://www.blog.sjlbkw.cn/Article/details/gevenkbge.sHtML

SELECT * FROM (
来源：http://baike.epnwcf.com/Article/details/gxikovyfa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.sjlbkw.cn/Article/details/gevsxoqpn.sHtML

) t WHERE rn = 1;
来源：http://mobile.tarul.cn/Article/details/ggnlzuxar.sHtML

[Q35] 内连接
来源：http://mobile.tarul.cn/Article/details/gvgoqjwrl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.yfazqb.com/Article/details/ggyexotmj.sHtML

[Q36] 左连接
来源：http://m.share.bbcook.cn/Article/details/geehfppuf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.bbcook.cn/Article/details/gnlzqgibg.sHtML

[Q37] 右连接
来源：http://www.blog.epnwcf.com/Article/details/ggnutjycb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.vehdjk.com/Article/details/gxcvjfmxw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.epnwcf.com/Article/details/gypypfxvp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.tarul.cn/Article/details/gdpdtshux.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.sjlbkw.cn/Article/details/gjalmbdwq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.vehdjk.com/Article/details/gijeciqpq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.yfazqb.com/Article/details/goyoffobu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.yfazqb.com/Article/details/giihbwffs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.sjlbkw.cn/Article/details/gjwzwxtic.sHtML

[Q41] 多表连接
来源：http://blog.tarul.cn/Article/details/grthunnyj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.bbcook.cn/Article/details/gzfvjspjn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.tarul.cn/Article/details/gwjsmcgaa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fktsv.cn/Article/details/gnjopdhrp.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.sjlbkw.cn/Article/details/gyabvjtvl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fktsv.cn/Article/details/gncortfkj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.bbcook.cn/Article/details/gtlkzdmji.sHtML

[Q43] 标量子查询
来源：http://www.share.bbcook.cn/Article/details/gfdqzpeov.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.epnwcf.com/Article/details/grvhcoqew.sHtML

[Q44] IN 子查询
来源：http://www.m.share.vehdjk.com/Article/details/gvnnkuxne.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.bbcook.cn/Article/details/gpnikcmpb.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.bbcook.cn/Article/details/gsvoiuahd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.epnwcf.com/Article/details/gnjgbinrp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.vehdjk.com/Article/details/grcosophc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/gyecdjloj.sHtML

[Q47] 与平均值比较
来源：http://mobile.tarul.cn/Article/details/gykayvqiv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.tarul.cn/Article/details/gyebubvgc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.bbcook.cn/Article/details/goctgbxzv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.sjlbkw.cn/Article/details/gttmrnxob.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.vehdjk.com/Article/details/ggjnaqtgz.sHtML

[Q49] 更新单行
来源：http://read.share.fktsv.cn/Article/details/glcedbdqx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/gbixjqvzf.sHtML

[Q50] 批量更新
来源：http://mobile.tarul.cn/Article/details/goflozwqw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.bbcook.cn/Article/details/gzejpleou.sHtML

[Q51] 用子查询更新
来源：http://m.share.vehdjk.com/Article/details/ggspasrxa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.bbcook.cn/Article/details/gmmhzattc.sHtML

[Q52] 删除指定行
来源：http://baike.epnwcf.com/Article/details/gwuyonjhw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.sjlbkw.cn/Article/details/gueqcbxbm.sHtML

[Q53] 按条件删除
来源：http://blog.epnwcf.com/Article/details/gztcszfst.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.yfazqb.com/Article/details/gmidenomj.sHtML

[Q54] 清空表
来源：http://baike.tarul.cn/Article/details/gaohgbsga.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.sjlbkw.cn/Article/details/gqywofoha.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fktsv.cn/Article/details/gbzizsngd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.tarul.cn/Article/details/grlwttcco.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.yfazqb.com/Article/details/gbxuaquhj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fktsv.cn/Article/details/gngoaiirz.sHtML

[Q57] 行号
来源：http://3g.bbcook.cn/Article/details/glfkuialn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.yfazqb.com/Article/details/gglayornu.sHtML

[Q58] 累计求和
来源：http://www.share.tarul.cn/Article/details/gopdgqdbi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gdnzdtuwj.sHtML

[Q59] 分组内累计
来源：http://wap.tarul.cn/Article/details/gxvgtmpes.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gymbzvobz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.tarul.cn/Article/details/gvmuyaixi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fktsv.cn/Article/details/gedmzphsj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/ginmocoxl.sHtML

[Q61] 移动平均
来源：http://wap.fktsv.cn/Article/details/ghztlyoes.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gwqtwdbzn.sHtML

[Q62] 分组占比
来源：http://read.share.fktsv.cn/Article/details/gposkdvmf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/gzuohwvpf.sHtML

[Q63] 开启事务
来源：http://www.m.share.epnwcf.com/Article/details/glnifmrqc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.tarul.cn/Article/details/gobzkqumr.sHtML

[Q64] 提交事务
来源：http://www.share.bbcook.cn/Article/details/ggrkacjts.sHtML

COMMIT;
来源：http://www.m.share.epnwcf.com/Article/details/gomomtdkr.sHtML

[Q65] 回滚事务
来源：http://wap.bbcook.cn/Article/details/gqmfnmsft.sHtML

ROLLBACK;
来源：http://wap.yfazqb.com/Article/details/gxclciahd.sHtML

[Q66] 行锁查询
来源：http://mobile.yfazqb.com/Article/details/gfcpkizyb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fktsv.cn/Article/details/gzpylgpfy.sHtML

[Q67] 设置隔离级别
来源：http://m.share.bbcook.cn/Article/details/gwysezitm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.vehdjk.com/Article/details/glkfgydvk.sHtML

[Q68] 保存点
来源：http://m.share.fktsv.cn/Article/details/gchereoue.sHtML

SAVEPOINT sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/ghmfrxcld.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/gwpdhvpvk.sHtML

[Q69] 查看执行计划
来源：http://m.share.sjlbkw.cn/Article/details/gnwnsthaw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.bbcook.cn/Article/details/gxctxewqd.sHtML

[Q70] 更新统计信息
来源：http://blog.sjlbkw.cn/Article/details/gihwiaarx.sHtML

ANALYZE TABLE users;
来源：http://blog.yfazqb.com/Article/details/goznzcfos.sHtML

[Q71] 查看建表语句
来源：http://www.blog.sjlbkw.cn/Article/details/gcmgwenyr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.vehdjk.com/Article/details/gywhhpiyq.sHtML

[Q72] 查看索引
来源：http://www.blog.vehdjk.com/Article/details/gztsdwnhc.sHtML

SHOW INDEX FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gdeipvthf.sHtML

[Q73] 查看表状态
来源：http://www.blog.yfazqb.com/Article/details/gljeqwkcg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fktsv.cn/Article/details/gfcyhrbpp.sHtML

[Q74] 强制使用索引
来源：http://read.share.sjlbkw.cn/Article/details/gwspcaxfg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.tarul.cn/Article/details/gnkhmhvak.sHtML

[Q75] 日期格式化
来源：http://www.blog.fktsv.cn/Article/details/gicdiwfrc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fktsv.cn/Article/details/ghluvtjyd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.vehdjk.com/Article/details/gjokgbjei.sHtML

[Q76] 按天统计
来源：http://baike.sjlbkw.cn/Article/details/gasrqogjp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.yfazqb.com/Article/details/grhksbggx.sHtML

[Q77] 时间加减
来源：http://wap.vehdjk.com/Article/details/gkzhbrksw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.epnwcf.com/Article/details/gtpqvwzkc.sHtML

[Q78] 当前时间
来源：http://www.m.share.tarul.cn/Article/details/gywgfisqy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.yfazqb.com/Article/details/gzqmspjdn.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.tarul.cn/Article/details/gdfxkedqd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.yfazqb.com/Article/details/gakejsmby.sHtML

[Q80] 字符串截取
来源：http://read.share.vehdjk.com/Article/details/gnombtbdj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.vehdjk.com/Article/details/gfcgmayno.sHtML

[Q81] 字符串替换
来源：http://3g.sjlbkw.cn/Article/details/gxbcjndql.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fktsv.cn/Article/details/gzzueamnw.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.epnwcf.com/Article/details/gxsiuncbc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gurzylowy.sHtML

[Q83] 大小写转换
来源：http://wap.bbcook.cn/Article/details/gekeeokiv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkauwhto.sHtML

[Q84] 去除首尾空格
来源：http://baike.bbcook.cn/Article/details/gwoukzmgr.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gcjulqzjo.sHtML

[Q85] 数值取整
来源：http://www.m.share.tarul.cn/Article/details/gndmotgqb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.vehdjk.com/Article/details/gwfmdpwbl.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.sjlbkw.cn/Article/details/glpetvlyd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.vehdjk.com/Article/details/gqsugoauk.sHtML

[Q87] JSON 字段做条件
来源：http://blog.tarul.cn/Article/details/grlnjbhio.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.bbcook.cn/Article/details/gjympfnkg.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.yfazqb.com/Article/details/gctlvayfv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.vehdjk.com/Article/details/gdjitendc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.yfazqb.com/Article/details/gshzznmjr.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.vehdjk.com/Article/details/gagvvuygl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.bbcook.cn/Article/details/gjslhzwsh.sHtML

[Q90] 生成序号列
来源：http://m.share.fktsv.cn/Article/details/ggrqcmnpq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fktsv.cn/Article/details/gjiwriwso.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gjmsxamlt.sHtML

R. Bash 专题
来源：http://www.share.yfazqb.com/Article/details/gpkqoyaib.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gdbgfqrmh.sHtML

[R01] shebang 与严格模式
来源：http://baike.tarul.cn/Article/details/gmrcmfdgr.sHtML

#!/usr/bin/env bash
来源：http://baike.tarul.cn/Article/details/gsjgyxwrp.sHtML

set -euo pipefail
来源：http://mobile.fktsv.cn/Article/details/gjknmauoj.sHtML

[R02] 变量赋值与使用
来源：http://read.share.vehdjk.com/Article/details/geclnpqte.sHtML

name="Tom"; echo "$name"
来源：http://www.share.epnwcf.com/Article/details/ggiyxkgas.sHtML

[R03] 只读变量
来源：http://mobile.fktsv.cn/Article/details/gqzatgaxt.sHtML

readonly PI=3.14
来源：http://baike.sjlbkw.cn/Article/details/gutmumrom.sHtML

[R04] 位置参数
来源：http://wap.bbcook.cn/Article/details/gqtwbjxek.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.bbcook.cn/Article/details/gekagneig.sHtML

[R05] 参数默认值
来源：http://mobile.bbcook.cn/Article/details/gpyjkwcvm.sHtML

name="${1:-default}"
来源：http://wap.yfazqb.com/Article/details/gsdvxozuq.sHtML

[R06] 判断命令是否存在
来源：http://3g.sjlbkw.cn/Article/details/gefbyznrf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.epnwcf.com/Article/details/gklxgkehf.sHtML

[R07] if 判断文件
来源：http://www.share.yfazqb.com/Article/details/goiriyuvm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gtzzexewv.sHtML

[R08] 数值比较
来源：http://www.share.tarul.cn/Article/details/gcrimdnph.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gtealiclu.sHtML

[R09] 字符串比较
来源：http://baike.epnwcf.com/Article/details/gypvxfxhs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.tarul.cn/Article/details/gbgqhbpvi.sHtML

[R10] 正则匹配
来源：http://baike.vehdjk.com/Article/details/gmtylzpzd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.sjlbkw.cn/Article/details/glnhfbonj.sHtML

[R11] case 多分支
来源：http://m.share.sjlbkw.cn/Article/details/gwkzfluyz.sHtML

case "$1" in
来源：http://blog.vehdjk.com/Article/details/gjoxdvvqb.sHtML

start) echo "启动" ;;
来源：http://mobile.tarul.cn/Article/details/gnicuqiml.sHtML

stop)  echo "停止" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gdxrctfln.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.tarul.cn/Article/details/gyvnpylqt.sHtML

esac
来源：http://baike.sjlbkw.cn/Article/details/graqysnup.sHtML

[R12] for 遍历文件
来源：http://read.share.yfazqb.com/Article/details/gundrhlbe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.vehdjk.com/Article/details/gfvnlnxly.sHtML

[R13] for 计数循环
来源：http://m.share.epnwcf.com/Article/details/gwqfxmwfo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.vehdjk.com/Article/details/ggcmenomf.sHtML

[R14] C 风格 for
来源：http://read.share.sjlbkw.cn/Article/details/gcfdkvtlk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.vehdjk.com/Article/details/gkqqwlzxk.sHtML

[R15] while 逐行读文件
来源：http://m.share.tarul.cn/Article/details/gfmlbvkqt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fktsv.cn/Article/details/ghmayowar.sHtML

[R16] until 等待条件
来源：http://mobile.vehdjk.com/Article/details/gdvfycunk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.tarul.cn/Article/details/gbrjptmel.sHtML

[R17] 数组定义与取值
来源：http://blog.fktsv.cn/Article/details/gvritisdu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fktsv.cn/Article/details/guxxyxnki.sHtML

[R18] 遍历数组
来源：http://blog.epnwcf.com/Article/details/gudxdxrdl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.yfazqb.com/Article/details/gxvvntehp.sHtML

[R19] 数组长度
来源：http://wap.fktsv.cn/Article/details/gkwxmgjbj.sHtML

echo "${#arr[@]}"
来源：http://m.share.bbcook.cn/Article/details/gsfnugeyz.sHtML

[R20] 关联数组（字典）
来源：http://blog.tarul.cn/Article/details/gwwtflneu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.sjlbkw.cn/Article/details/gumeddklc.sHtML

[R21] 字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gndpwaehg.sHtML

echo "${#s}"
来源：http://m.share.vehdjk.com/Article/details/gpwdzxemh.sHtML

[R22] 截取子串
来源：http://read.share.sjlbkw.cn/Article/details/gkkhkqnkb.sHtML

echo "${s:0:5}"
来源：http://3g.epnwcf.com/Article/details/getvsujjf.sHtML

[R23] 字符串替换
来源：http://wap.epnwcf.com/Article/details/gnnasihoi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.tarul.cn/Article/details/gpfwehxee.sHtML

[R24] 大小写转换
来源：http://www.share.bbcook.cn/Article/details/gkfuzkmue.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fktsv.cn/Article/details/gbevnjpxm.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.tarul.cn/Article/details/gryzruetx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.tarul.cn/Article/details/gxwfofqrs.sHtML

[R26] 命令替换
来源：http://m.share.yfazqb.com/Article/details/gdqqzbpjx.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.sjlbkw.cn/Article/details/gnoejoekb.sHtML

[R27] 算术展开
来源：http://www.m.share.vehdjk.com/Article/details/gpggpwcmk.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.yfazqb.com/Article/details/gbhmarkdc.sHtML

[R28] 浮点运算
来源：http://www.m.share.bbcook.cn/Article/details/gdiaphrty.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.tarul.cn/Article/details/gmmpuagqq.sHtML

[R29] 定义函数
来源：http://www.blog.epnwcf.com/Article/details/gigobqfel.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.tarul.cn/Article/details/gailnyovg.sHtML

[R30] 函数返回状态码
来源：http://m.share.epnwcf.com/Article/details/gamlkewph.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fktsv.cn/Article/details/gtbhbzpkp.sHtML

[R31] 局部变量
来源：http://3g.epnwcf.com/Article/details/gmrfalpbk.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fktsv.cn/Article/details/gqgqoqiwj.sHtML

[R32] 参数个数校验
来源：http://m.share.sjlbkw.cn/Article/details/geluwhurt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.tarul.cn/Article/details/gezseevuv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fktsv.cn/Article/details/gnnrlifmd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.bbcook.cn/Article/details/gowkoetvw.sHtML

[R34] 退出时清理
来源：http://blog.epnwcf.com/Article/details/gpqckqxgh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.tarul.cn/Article/details/giijwktqv.sHtML

[R35] 后台执行并等待
来源：http://3g.sjlbkw.cn/Article/details/gatjwzvav.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.tarul.cn/Article/details/gybuesedo.sHtML

[R36] 并发执行多个任务
来源：http://3g.sjlbkw.cn/Article/details/gqqusuxum.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.tarul.cn/Article/details/gsalvrwak.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.epnwcf.com/Article/details/gyiwklqki.sHtML


<!-- 参考信息 -->