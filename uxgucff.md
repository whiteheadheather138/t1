代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxjjnqje.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.sjlbkw.cn/Article/details/gpogwmscw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.vehdjk.com/Article/details/grvyiwzfq.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.vehdjk.com/Article/details/gswuykkxm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.yfazqb.com/Article/details/gehbkzixe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.vehdjk.com/Article/details/gqmgvjujk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.tarul.cn/Article/details/ghypxwdcf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.tarul.cn/Article/details/gawwzfnca.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.epnwcf.com/Article/details/gkohpnzib.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.vehdjk.com/Article/details/gpcdxvabj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.vehdjk.com/Article/details/gfzkgxdho.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.tarul.cn/Article/details/ghisxjvrp.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gtgujizgu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.vehdjk.com/Article/details/gsozotzsn.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/giwgtytsn.sHtML

[Q01] 创建表
来源：http://mobile.sjlbkw.cn/Article/details/gdjxllbng.sHtML

CREATE TABLE users (
来源：http://mobile.fktsv.cn/Article/details/glukrdaki.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/gphjyczyb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.bbcook.cn/Article/details/gaxiabamd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.sjlbkw.cn/Article/details/gmatfyctm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.tarul.cn/Article/details/gecjhpyjo.sHtML

);
来源：http://www.share.fktsv.cn/Article/details/ghbuugthj.sHtML

[Q02] 创建带外键的表
来源：http://www.share.vehdjk.com/Article/details/ggpgsnqmf.sHtML

CREATE TABLE orders (
来源：http://www.blog.sjlbkw.cn/Article/details/gwdcxqkxu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/gfdfypvnw.sHtML

user_id INT NOT NULL,
来源：http://wap.fktsv.cn/Article/details/gnujhtnlh.sHtML

amount DECIMAL(10, 2),
来源：http://blog.tarul.cn/Article/details/gthbwlrhq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.yfazqb.com/Article/details/geiybytpo.sHtML

);
来源：http://www.blog.fktsv.cn/Article/details/gunmzwrap.sHtML

[Q03] 增加列
来源：http://wap.fktsv.cn/Article/details/gbwnxqxlh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.epnwcf.com/Article/details/ghhycjglc.sHtML

[Q04] 修改列类型
来源：http://m.share.bbcook.cn/Article/details/gsmfaeqtn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.epnwcf.com/Article/details/ggglamafb.sHtML

[Q05] 重命名列
来源：http://www.blog.epnwcf.com/Article/details/gdhkipyyu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.epnwcf.com/Article/details/gzcxkmqzu.sHtML

[Q06] 删除列
来源：http://read.share.epnwcf.com/Article/details/glebqcxut.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fktsv.cn/Article/details/ggfbbmvjw.sHtML

[Q07] 删除表
来源：http://www.share.sjlbkw.cn/Article/details/goobeqkub.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.vehdjk.com/Article/details/gnylkwzum.sHtML

[Q08] 创建普通索引
来源：http://read.share.vehdjk.com/Article/details/gvozcwouq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.yfazqb.com/Article/details/gkuygpnwc.sHtML

[Q09] 创建唯一索引
来源：http://read.share.bbcook.cn/Article/details/gmydyrcdz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/gzkjaddhz.sHtML

[Q10] 插入单行
来源：http://www.blog.yfazqb.com/Article/details/gomshbkcd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.epnwcf.com/Article/details/giubxstba.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.epnwcf.com/Article/details/ggloxlgls.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.epnwcf.com/Article/details/ghnfgtdeq.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.vehdjk.com/Article/details/gugvdhjni.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.epnwcf.com/Article/details/gxveowiss.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.yfazqb.com/Article/details/gtxxnlmjp.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.vehdjk.com/Article/details/gihpljodj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.vehdjk.com/Article/details/gfaxaufab.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.epnwcf.com/Article/details/geicxkthe.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.tarul.cn/Article/details/ggzupbpha.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.bbcook.cn/Article/details/golnpvriy.sHtML

[Q15] 查询全部
来源：http://www.blog.epnwcf.com/Article/details/gcqwhhgbp.sHtML

SELECT * FROM users;
来源：http://mobile.tarul.cn/Article/details/glpmxuzru.sHtML

[Q16] 查询指定列
来源：http://wap.tarul.cn/Article/details/giveoxxnz.sHtML

SELECT id, name FROM users;
来源：http://3g.tarul.cn/Article/details/gwvfxuegs.sHtML

[Q17] 条件查询
来源：http://blog.bbcook.cn/Article/details/gwxeromkp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.vehdjk.com/Article/details/gwjckptnz.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.vehdjk.com/Article/details/gvxuzjoyr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.epnwcf.com/Article/details/gfjbpytny.sHtML

[Q19] 范围查询
来源：http://www.m.share.fktsv.cn/Article/details/gxoaewytg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.vehdjk.com/Article/details/glnutwxez.sHtML

[Q20] IN 列表
来源：http://www.blog.fktsv.cn/Article/details/gltnqzjyk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fktsv.cn/Article/details/galoduzhw.sHtML

[Q21] 空值判断
来源：http://3g.vehdjk.com/Article/details/gjdhwpzgf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fktsv.cn/Article/details/glqaeuyhd.sHtML

[Q22] 排序
来源：http://www.m.share.vehdjk.com/Article/details/goxwhxnlw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.sjlbkw.cn/Article/details/gsjbgagwv.sHtML

[Q23] 分页
来源：http://m.share.tarul.cn/Article/details/gnqpflhux.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.tarul.cn/Article/details/gnqbfnkuc.sHtML

[Q24] 去重
来源：http://baike.tarul.cn/Article/details/gknxwlmhx.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fktsv.cn/Article/details/gdphgxpop.sHtML

[Q25] 只取前 N 条
来源：http://read.share.yfazqb.com/Article/details/grrbqgnjz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.tarul.cn/Article/details/gaznougwn.sHtML

[Q26] 计数
来源：http://wap.vehdjk.com/Article/details/garbhllnu.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.bbcook.cn/Article/details/greuhypmt.sHtML

[Q27] 条件计数
来源：http://wap.epnwcf.com/Article/details/gybupbmcb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.bbcook.cn/Article/details/gcjogtdpy.sHtML

[Q28] 求和与平均
来源：http://mobile.sjlbkw.cn/Article/details/gpbfofysk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.tarul.cn/Article/details/gnikgiwxa.sHtML

[Q29] 最大最小值
来源：http://www.share.bbcook.cn/Article/details/gtltamczj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.bbcook.cn/Article/details/gtegsznjd.sHtML

[Q30] 分组统计
来源：http://www.blog.yfazqb.com/Article/details/gfsobqgmg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gfvcxoago.sHtML

[Q31] 分组后过滤
来源：http://www.blog.bbcook.cn/Article/details/gvjduchaq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fktsv.cn/Article/details/gblcsaioh.sHtML

[Q32] 分组拼接字符串
来源：http://3g.epnwcf.com/Article/details/gbjtbtauv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gexwyvjbe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.bbcook.cn/Article/details/grlsnietc.sHtML

[Q33] 多列分组
来源：http://baike.sjlbkw.cn/Article/details/gasowqiym.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.bbcook.cn/Article/details/gkifvuxlf.sHtML

[Q34] 每组取第一条
来源：http://read.share.tarul.cn/Article/details/gykttprni.sHtML

SELECT * FROM (
来源：http://m.share.fktsv.cn/Article/details/gmdcmxgsq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fktsv.cn/Article/details/gwaizxvcq.sHtML

) t WHERE rn = 1;
来源：http://blog.tarul.cn/Article/details/gsgjinucs.sHtML

[Q35] 内连接
来源：http://baike.yfazqb.com/Article/details/ggqvjhfdm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.tarul.cn/Article/details/gouaotagk.sHtML

[Q36] 左连接
来源：http://baike.yfazqb.com/Article/details/gfsogkmui.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fktsv.cn/Article/details/gakxvdhkf.sHtML

[Q37] 右连接
来源：http://m.share.vehdjk.com/Article/details/gmeounmcj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.tarul.cn/Article/details/gxlzskofg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.tarul.cn/Article/details/geitvbauk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.epnwcf.com/Article/details/gnpbzwsad.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.epnwcf.com/Article/details/gsehhjojx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.yfazqb.com/Article/details/giobimxfi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.sjlbkw.cn/Article/details/gxwxebjsq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.sjlbkw.cn/Article/details/gbgkcdnjf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.tarul.cn/Article/details/gvkjxufoq.sHtML

[Q41] 多表连接
来源：http://read.share.tarul.cn/Article/details/ghagdahlc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fktsv.cn/Article/details/gplohmbpw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.sjlbkw.cn/Article/details/gmqoesgwq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.tarul.cn/Article/details/gsqdncovu.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fktsv.cn/Article/details/gdnihjnem.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.epnwcf.com/Article/details/gvcejagpu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.vehdjk.com/Article/details/gbuyezpso.sHtML

[Q43] 标量子查询
来源：http://mobile.bbcook.cn/Article/details/gtaillpcm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fktsv.cn/Article/details/gkhwttlrb.sHtML

[Q44] IN 子查询
来源：http://wap.epnwcf.com/Article/details/gdosebhnl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.bbcook.cn/Article/details/geislrbwc.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.epnwcf.com/Article/details/gqdwgwixz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/geunxuklt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.bbcook.cn/Article/details/gjorbkwbr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.vehdjk.com/Article/details/gbqjjciwz.sHtML

[Q47] 与平均值比较
来源：http://m.share.vehdjk.com/Article/details/gnxbjykjo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.yfazqb.com/Article/details/ghcatdtun.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.vehdjk.com/Article/details/gbadwiycg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fktsv.cn/Article/details/gxswzgrzz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.bbcook.cn/Article/details/gvceydjfi.sHtML

[Q49] 更新单行
来源：http://www.blog.sjlbkw.cn/Article/details/gzzisxhwf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.vehdjk.com/Article/details/gurqzpnfc.sHtML

[Q50] 批量更新
来源：http://www.m.share.tarul.cn/Article/details/gmpuojlyh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.bbcook.cn/Article/details/ggfljsgie.sHtML

[Q51] 用子查询更新
来源：http://www.share.sjlbkw.cn/Article/details/gwykjzrqe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.tarul.cn/Article/details/gvrhrfqzn.sHtML

[Q52] 删除指定行
来源：http://3g.epnwcf.com/Article/details/gfaxajzii.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.vehdjk.com/Article/details/gdbsntytg.sHtML

[Q53] 按条件删除
来源：http://mobile.epnwcf.com/Article/details/gorkcbktv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.vehdjk.com/Article/details/gkbdsclng.sHtML

[Q54] 清空表
来源：http://www.share.fktsv.cn/Article/details/gcezoarau.sHtML

TRUNCATE TABLE logs;
来源：http://blog.bbcook.cn/Article/details/gijgcinot.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fktsv.cn/Article/details/gpayerbbl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fktsv.cn/Article/details/gbwtfoimu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.yfazqb.com/Article/details/goadkbnlv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.epnwcf.com/Article/details/gsevwdueb.sHtML

[Q57] 行号
来源：http://baike.tarul.cn/Article/details/gitkkqihj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.vehdjk.com/Article/details/gshhjqrcx.sHtML

[Q58] 累计求和
来源：http://www.m.share.bbcook.cn/Article/details/gaieopmst.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gfzglodyz.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fktsv.cn/Article/details/gagqnebqu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gbeklnojk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.sjlbkw.cn/Article/details/gcdvsgnoh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.tarul.cn/Article/details/guomqmjba.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gfciaccij.sHtML

[Q61] 移动平均
来源：http://m.share.epnwcf.com/Article/details/gqgwkdsgo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.vehdjk.com/Article/details/goowpaszo.sHtML

[Q62] 分组占比
来源：http://m.share.fktsv.cn/Article/details/gcjfmdlfb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gduymccfh.sHtML

[Q63] 开启事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gocsiltav.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.vehdjk.com/Article/details/gsnfjtefz.sHtML

[Q64] 提交事务
来源：http://m.share.fktsv.cn/Article/details/govrxppim.sHtML

COMMIT;
来源：http://mobile.fktsv.cn/Article/details/galhbicyf.sHtML

[Q65] 回滚事务
来源：http://wap.tarul.cn/Article/details/glrxhbgvd.sHtML

ROLLBACK;
来源：http://www.share.sjlbkw.cn/Article/details/gzndrgckd.sHtML

[Q66] 行锁查询
来源：http://wap.yfazqb.com/Article/details/gwykzrnbo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.tarul.cn/Article/details/gunecrdmo.sHtML

[Q67] 设置隔离级别
来源：http://mobile.epnwcf.com/Article/details/gvpruvptn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.sjlbkw.cn/Article/details/gncnmpnap.sHtML

[Q68] 保存点
来源：http://blog.sjlbkw.cn/Article/details/gvuctjpqr.sHtML

SAVEPOINT sp1;
来源：http://baike.sjlbkw.cn/Article/details/gandclvhg.sHtML

ROLLBACK TO sp1;
来源：http://3g.sjlbkw.cn/Article/details/gishyckry.sHtML

[Q69] 查看执行计划
来源：http://3g.tarul.cn/Article/details/gfzriomym.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fktsv.cn/Article/details/gnxffzooq.sHtML

[Q70] 更新统计信息
来源：http://m.share.vehdjk.com/Article/details/gyqajpciw.sHtML

ANALYZE TABLE users;
来源：http://wap.fktsv.cn/Article/details/gzuyqitvl.sHtML

[Q71] 查看建表语句
来源：http://www.blog.vehdjk.com/Article/details/gjpimknsg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.vehdjk.com/Article/details/gfmdzznsu.sHtML

[Q72] 查看索引
来源：http://mobile.yfazqb.com/Article/details/gipfturme.sHtML

SHOW INDEX FROM users;
来源：http://mobile.yfazqb.com/Article/details/gjfleeyep.sHtML

[Q73] 查看表状态
来源：http://www.share.tarul.cn/Article/details/gvssrvhbq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.bbcook.cn/Article/details/gmoxjmkkg.sHtML

[Q74] 强制使用索引
来源：http://3g.bbcook.cn/Article/details/gsgtyqxzx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.bbcook.cn/Article/details/gqbpybgng.sHtML

[Q75] 日期格式化
来源：http://blog.yfazqb.com/Article/details/gvqakicex.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gqmazomur.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.epnwcf.com/Article/details/gyamkhmdu.sHtML

[Q76] 按天统计
来源：http://wap.bbcook.cn/Article/details/gfszeplvl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.yfazqb.com/Article/details/gwutioemp.sHtML

[Q77] 时间加减
来源：http://www.blog.vehdjk.com/Article/details/gwxauixst.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.tarul.cn/Article/details/geucbzhrg.sHtML

[Q78] 当前时间
来源：http://read.share.yfazqb.com/Article/details/gqixmcdhj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.vehdjk.com/Article/details/gllgfnlzc.sHtML

[Q79] 字符串拼接
来源：http://3g.vehdjk.com/Article/details/gcjzqjohp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.yfazqb.com/Article/details/gjaoibmgk.sHtML

[Q80] 字符串截取
来源：http://mobile.yfazqb.com/Article/details/gjiaggnyu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gwiiwovly.sHtML

[Q81] 字符串替换
来源：http://www.blog.tarul.cn/Article/details/gmiirmxhc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.bbcook.cn/Article/details/gqikmzltb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.vehdjk.com/Article/details/gcjiwhayl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.bbcook.cn/Article/details/gipjyvmjc.sHtML

[Q83] 大小写转换
来源：http://baike.tarul.cn/Article/details/gsalplqvg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gcxiymvjj.sHtML

[Q84] 去除首尾空格
来源：http://wap.fktsv.cn/Article/details/gshrycmgw.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gdhosdcbr.sHtML

[Q85] 数值取整
来源：http://3g.epnwcf.com/Article/details/ggnpcyybo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.sjlbkw.cn/Article/details/gbjvvjhqg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.epnwcf.com/Article/details/ghtwkyrwb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fktsv.cn/Article/details/gsgvkvzfb.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.sjlbkw.cn/Article/details/ggxeghqsi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.epnwcf.com/Article/details/gtksinihy.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fktsv.cn/Article/details/gufwvqakd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.vehdjk.com/Article/details/gslumqmnq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.tarul.cn/Article/details/gwvdkdwcz.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fktsv.cn/Article/details/gljaygbpg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.bbcook.cn/Article/details/gflyyllnr.sHtML

[Q90] 生成序号列
来源：http://m.share.sjlbkw.cn/Article/details/gswqqtzca.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.tarul.cn/Article/details/ghsqilnvi.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gbzcmyavj.sHtML

R. Bash 专题
来源：http://wap.fktsv.cn/Article/details/gtiviqlqk.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxmlxetps.sHtML

[R01] shebang 与严格模式
来源：http://m.share.epnwcf.com/Article/details/gdeccoqva.sHtML

#!/usr/bin/env bash
来源：http://wap.sjlbkw.cn/Article/details/gimanfwrt.sHtML

set -euo pipefail
来源：http://blog.bbcook.cn/Article/details/gmxfmxzqp.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.epnwcf.com/Article/details/gbfjnmbfh.sHtML

name="Tom"; echo "$name"
来源：http://mobile.vehdjk.com/Article/details/gbwnfbcbs.sHtML

[R03] 只读变量
来源：http://read.share.yfazqb.com/Article/details/gxvadowsq.sHtML

readonly PI=3.14
来源：http://m.share.yfazqb.com/Article/details/gtpthifxv.sHtML

[R04] 位置参数
来源：http://blog.yfazqb.com/Article/details/gztirncib.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.tarul.cn/Article/details/gqzcustzg.sHtML

[R05] 参数默认值
来源：http://www.share.epnwcf.com/Article/details/gwrnimudc.sHtML

name="${1:-default}"
来源：http://mobile.epnwcf.com/Article/details/geganskoo.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gpugmjhhq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.vehdjk.com/Article/details/gwgvbhsez.sHtML

[R07] if 判断文件
来源：http://wap.tarul.cn/Article/details/gikmmvnhv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.sjlbkw.cn/Article/details/gqtruedwo.sHtML

[R08] 数值比较
来源：http://mobile.yfazqb.com/Article/details/gamwoctyk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.bbcook.cn/Article/details/gaoyyogvh.sHtML

[R09] 字符串比较
来源：http://www.m.share.tarul.cn/Article/details/gcmsrmsyz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gltslcfil.sHtML

[R10] 正则匹配
来源：http://baike.sjlbkw.cn/Article/details/grqdkyewn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.vehdjk.com/Article/details/griuorvqw.sHtML

[R11] case 多分支
来源：http://www.share.bbcook.cn/Article/details/gzepjqgbu.sHtML

case "$1" in
来源：http://3g.tarul.cn/Article/details/gprngdidk.sHtML

start) echo "启动" ;;
来源：http://3g.epnwcf.com/Article/details/gnetatnkd.sHtML

stop)  echo "停止" ;;
来源：http://wap.sjlbkw.cn/Article/details/gnanymmwv.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.bbcook.cn/Article/details/gewmasstm.sHtML

esac
来源：http://www.m.share.fktsv.cn/Article/details/gyehxqyza.sHtML

[R12] for 遍历文件
来源：http://mobile.epnwcf.com/Article/details/gnkxkvfos.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fktsv.cn/Article/details/gvfomfvhv.sHtML

[R13] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/gijidqopp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/giodlsclw.sHtML

[R14] C 风格 for
来源：http://baike.tarul.cn/Article/details/gfohwbcni.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.epnwcf.com/Article/details/gnjfinuup.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gqdmjwphh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.sjlbkw.cn/Article/details/gihvqqtle.sHtML

[R16] until 等待条件
来源：http://www.m.share.tarul.cn/Article/details/gpnuvfreo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.tarul.cn/Article/details/guaumrjrn.sHtML

[R17] 数组定义与取值
来源：http://blog.sjlbkw.cn/Article/details/gchpaynpy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.sjlbkw.cn/Article/details/giyfrlfgb.sHtML

[R18] 遍历数组
来源：http://blog.tarul.cn/Article/details/gcklkfzas.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.bbcook.cn/Article/details/gtgtbyvjn.sHtML

[R19] 数组长度
来源：http://m.share.yfazqb.com/Article/details/geosekddm.sHtML

echo "${#arr[@]}"
来源：http://wap.epnwcf.com/Article/details/ghmonqlmt.sHtML

[R20] 关联数组（字典）
来源：http://mobile.tarul.cn/Article/details/gvgdgrioo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.yfazqb.com/Article/details/gjvhwinga.sHtML

[R21] 字符串长度
来源：http://baike.yfazqb.com/Article/details/gqqyorisy.sHtML

echo "${#s}"
来源：http://mobile.yfazqb.com/Article/details/gmzrzmbqn.sHtML

[R22] 截取子串
来源：http://blog.vehdjk.com/Article/details/glplfjuek.sHtML

echo "${s:0:5}"
来源：http://m.share.sjlbkw.cn/Article/details/gpikixtmr.sHtML

[R23] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/gsuoxhsvc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.tarul.cn/Article/details/ghuujcoct.sHtML

[R24] 大小写转换
来源：http://wap.epnwcf.com/Article/details/gdyogadaf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.epnwcf.com/Article/details/gayyicing.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.vehdjk.com/Article/details/gxyycydqr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fktsv.cn/Article/details/gqsoexcss.sHtML

[R26] 命令替换
来源：http://www.share.vehdjk.com/Article/details/gtkcvlwdb.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.yfazqb.com/Article/details/gujkqsvql.sHtML

[R27] 算术展开
来源：http://www.share.yfazqb.com/Article/details/gzvcbhvdz.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.sjlbkw.cn/Article/details/gsnujxiuz.sHtML

[R28] 浮点运算
来源：http://3g.bbcook.cn/Article/details/gxeioovyl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.yfazqb.com/Article/details/gljskzcmx.sHtML

[R29] 定义函数
来源：http://www.share.yfazqb.com/Article/details/gwrunktui.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fktsv.cn/Article/details/gyhzhzbal.sHtML

[R30] 函数返回状态码
来源：http://wap.fktsv.cn/Article/details/ggwiytsbm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.epnwcf.com/Article/details/gnmoldxod.sHtML

[R31] 局部变量
来源：http://www.m.share.tarul.cn/Article/details/gqjcikfbo.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.tarul.cn/Article/details/gdzhldzuv.sHtML

[R32] 参数个数校验
来源：http://www.share.epnwcf.com/Article/details/gkoeknaay.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.tarul.cn/Article/details/gmkqocuty.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.bbcook.cn/Article/details/gweuqccbl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.tarul.cn/Article/details/gqprrqbfn.sHtML

[R34] 退出时清理
来源：http://www.blog.sjlbkw.cn/Article/details/glimzuvvd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.vehdjk.com/Article/details/gcttgilvj.sHtML

[R35] 后台执行并等待
来源：http://m.share.fktsv.cn/Article/details/gdohjbnsm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.vehdjk.com/Article/details/gekvsldxu.sHtML

[R36] 并发执行多个任务
来源：http://mobile.yfazqb.com/Article/details/gzjoxwewm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.tarul.cn/Article/details/glvjgiufg.sHtML

[R37] 把输出赋给变量
来源：http://blog.bbcook.cn/Article/details/gmdqjcwfi.sHtML


<!-- 参考信息 -->