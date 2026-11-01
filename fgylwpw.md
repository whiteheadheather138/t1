代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.epnwcf.com/Article/details/gwhejpwxr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.epnwcf.com/Article/details/gmjicixwr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.epnwcf.com/Article/details/gjwootxpf.sHtML

[P08] 处理浮点精度问题
来源：http://baike.epnwcf.com/Article/details/goagsknrw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.vehdjk.com/Article/details/ghomqkfrd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.bbcook.cn/Article/details/gfecbhayn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.yfazqb.com/Article/details/gvpaohcmd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.bbcook.cn/Article/details/gewhxtoig.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.sjlbkw.cn/Article/details/gxoihkcwr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.yfazqb.com/Article/details/gbhpuumnz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.sjlbkw.cn/Article/details/gqrplolxy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.epnwcf.com/Article/details/gdnowkgjs.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ggvlxmyas.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.tarul.cn/Article/details/gvaqbkofj.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/govppkxux.sHtML

[Q01] 创建表
来源：http://wap.sjlbkw.cn/Article/details/gftygehah.sHtML

CREATE TABLE users (
来源：http://www.share.sjlbkw.cn/Article/details/gcxvxybop.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.yfazqb.com/Article/details/gzulwjido.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.sjlbkw.cn/Article/details/guznzgddx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.epnwcf.com/Article/details/gptnkxhjq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.vehdjk.com/Article/details/gqqcgusfc.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/gnzpgvtrw.sHtML

[Q02] 创建带外键的表
来源：http://read.share.bbcook.cn/Article/details/gluuxmdsb.sHtML

CREATE TABLE orders (
来源：http://mobile.vehdjk.com/Article/details/gqicrwosm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.epnwcf.com/Article/details/gbiezhckx.sHtML

user_id INT NOT NULL,
来源：http://wap.sjlbkw.cn/Article/details/gqgvyxnda.sHtML

amount DECIMAL(10, 2),
来源：http://wap.vehdjk.com/Article/details/gfhiojlxq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fktsv.cn/Article/details/gwlvjskpx.sHtML

);
来源：http://www.share.tarul.cn/Article/details/gobczjisa.sHtML

[Q03] 增加列
来源：http://www.share.bbcook.cn/Article/details/gqoztglvf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.tarul.cn/Article/details/gatfhovmw.sHtML

[Q04] 修改列类型
来源：http://3g.bbcook.cn/Article/details/gdjiziisg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.tarul.cn/Article/details/glcvbgfhu.sHtML

[Q05] 重命名列
来源：http://www.m.share.epnwcf.com/Article/details/gcuxbnujy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.vehdjk.com/Article/details/gudmcedff.sHtML

[Q06] 删除列
来源：http://www.m.share.fktsv.cn/Article/details/gnjzrbgyw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.epnwcf.com/Article/details/gcefenivu.sHtML

[Q07] 删除表
来源：http://read.share.yfazqb.com/Article/details/gfjjxkuay.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.yfazqb.com/Article/details/gplwogica.sHtML

[Q08] 创建普通索引
来源：http://3g.epnwcf.com/Article/details/gtbcgvbot.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/ggguefvmu.sHtML

[Q09] 创建唯一索引
来源：http://read.share.yfazqb.com/Article/details/grcwmnhjl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.epnwcf.com/Article/details/guxbaozgh.sHtML

[Q10] 插入单行
来源：http://baike.yfazqb.com/Article/details/gxrifzorx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.vehdjk.com/Article/details/gmdfgyulk.sHtML

[Q11] 一次插入多行
来源：http://blog.epnwcf.com/Article/details/glomfcubo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.yfazqb.com/Article/details/gholaywrs.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.sjlbkw.cn/Article/details/ghotjdohb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.vehdjk.com/Article/details/gozbqtare.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.bbcook.cn/Article/details/geqzcxjly.sHtML

[Q13] 忽略重复插入
来源：http://mobile.vehdjk.com/Article/details/gonqbnoyl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gfmosfypz.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.tarul.cn/Article/details/ggmwmvtgw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fktsv.cn/Article/details/gevzpoycc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwyzadad.sHtML

[Q15] 查询全部
来源：http://baike.tarul.cn/Article/details/gdmuulguk.sHtML

SELECT * FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gbrincnay.sHtML

[Q16] 查询指定列
来源：http://blog.fktsv.cn/Article/details/gvergqace.sHtML

SELECT id, name FROM users;
来源：http://wap.fktsv.cn/Article/details/gpbyuoftr.sHtML

[Q17] 条件查询
来源：http://wap.yfazqb.com/Article/details/guvldsekh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.yfazqb.com/Article/details/gryamvbja.sHtML

[Q18] 模糊匹配
来源：http://read.share.epnwcf.com/Article/details/gcipwanff.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fktsv.cn/Article/details/gcixpgkax.sHtML

[Q19] 范围查询
来源：http://www.share.bbcook.cn/Article/details/goqxwzwbx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.yfazqb.com/Article/details/grkxlitbq.sHtML

[Q20] IN 列表
来源：http://baike.vehdjk.com/Article/details/ghcftmkqg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fktsv.cn/Article/details/gyfrykmlf.sHtML

[Q21] 空值判断
来源：http://www.blog.vehdjk.com/Article/details/glowlxrqt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.tarul.cn/Article/details/gnthpmxzh.sHtML

[Q22] 排序
来源：http://m.share.sjlbkw.cn/Article/details/gdycvmclk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fktsv.cn/Article/details/gjzwtihfc.sHtML

[Q23] 分页
来源：http://www.m.share.epnwcf.com/Article/details/gsolrkjhw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.yfazqb.com/Article/details/gzdytogtf.sHtML

[Q24] 去重
来源：http://www.blog.tarul.cn/Article/details/gbdjckeyd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gqcydehnp.sHtML

[Q25] 只取前 N 条
来源：http://mobile.tarul.cn/Article/details/gbutliayu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fktsv.cn/Article/details/gegtuqavq.sHtML

[Q26] 计数
来源：http://www.blog.yfazqb.com/Article/details/gehvctgkq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gduagigfu.sHtML

[Q27] 条件计数
来源：http://www.share.epnwcf.com/Article/details/ghddotmqt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.vehdjk.com/Article/details/gnnfheqys.sHtML

[Q28] 求和与平均
来源：http://read.share.sjlbkw.cn/Article/details/gnnkrzdlq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gpfgkzyud.sHtML

[Q29] 最大最小值
来源：http://m.share.tarul.cn/Article/details/gdfvkigsj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gbdkwexwc.sHtML

[Q30] 分组统计
来源：http://3g.fktsv.cn/Article/details/gkpdfqmsu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gqrzvrxux.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fktsv.cn/Article/details/gdeeucpgt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.yfazqb.com/Article/details/gyekmyczu.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.yfazqb.com/Article/details/gzlofkzcu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/godewklzm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.epnwcf.com/Article/details/gvobgllba.sHtML

[Q33] 多列分组
来源：http://www.blog.fktsv.cn/Article/details/grkjwlwqd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.sjlbkw.cn/Article/details/gjejuxaeb.sHtML

[Q34] 每组取第一条
来源：http://m.share.bbcook.cn/Article/details/gpcwpcmeo.sHtML

SELECT * FROM (
来源：http://m.share.yfazqb.com/Article/details/gnqmymhjc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fktsv.cn/Article/details/gbnhkfnwu.sHtML

) t WHERE rn = 1;
来源：http://www.share.tarul.cn/Article/details/gepqhmsrq.sHtML

[Q35] 内连接
来源：http://m.share.vehdjk.com/Article/details/gvveblqhg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.yfazqb.com/Article/details/glvjwfgcp.sHtML

[Q36] 左连接
来源：http://m.share.vehdjk.com/Article/details/ggkmxcsih.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.sjlbkw.cn/Article/details/glumuwgmd.sHtML

[Q37] 右连接
来源：http://3g.yfazqb.com/Article/details/gpdxjpmjj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.vehdjk.com/Article/details/gelslgftj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fktsv.cn/Article/details/glfldtoke.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.tarul.cn/Article/details/gqizkbxyj.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fktsv.cn/Article/details/gojhjlugq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.epnwcf.com/Article/details/gcunrbvfm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.bbcook.cn/Article/details/gucinbyyp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.bbcook.cn/Article/details/gqjoyyowa.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.vehdjk.com/Article/details/gnbaidsxq.sHtML

[Q41] 多表连接
来源：http://www.m.share.fktsv.cn/Article/details/gzhqcwfwc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.yfazqb.com/Article/details/gysjpjdzc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fktsv.cn/Article/details/ggiyijhzk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fktsv.cn/Article/details/gculpmzmx.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.tarul.cn/Article/details/guseyjuyq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.vehdjk.com/Article/details/gfvwaazav.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.bbcook.cn/Article/details/gkhxvcmbe.sHtML

[Q43] 标量子查询
来源：http://wap.sjlbkw.cn/Article/details/gehgehydh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.bbcook.cn/Article/details/gkerievwj.sHtML

[Q44] IN 子查询
来源：http://www.blog.epnwcf.com/Article/details/gnskgzptd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.bbcook.cn/Article/details/gqfixupvd.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.epnwcf.com/Article/details/gaitgcida.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.yfazqb.com/Article/details/gbjkgurvt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.yfazqb.com/Article/details/gairpvyym.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/gyyiihwew.sHtML

[Q47] 与平均值比较
来源：http://mobile.yfazqb.com/Article/details/gvtqghucy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.yfazqb.com/Article/details/gnvoloncv.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.bbcook.cn/Article/details/gizqqqmuo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.yfazqb.com/Article/details/gmagihewu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fktsv.cn/Article/details/gbglppmul.sHtML

[Q49] 更新单行
来源：http://www.share.fktsv.cn/Article/details/gvjlotjhg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.vehdjk.com/Article/details/gyvafvzod.sHtML

[Q50] 批量更新
来源：http://www.blog.fktsv.cn/Article/details/ggyhmavow.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.bbcook.cn/Article/details/gtgjjbtdo.sHtML

[Q51] 用子查询更新
来源：http://3g.vehdjk.com/Article/details/gaooiihlq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.tarul.cn/Article/details/goxbzrigx.sHtML

[Q52] 删除指定行
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvxbllan.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.vehdjk.com/Article/details/ghsnnjrja.sHtML

[Q53] 按条件删除
来源：http://mobile.tarul.cn/Article/details/gcohucaql.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.tarul.cn/Article/details/gvonhiljy.sHtML

[Q54] 清空表
来源：http://blog.sjlbkw.cn/Article/details/glgxevmmt.sHtML

TRUNCATE TABLE logs;
来源：http://3g.yfazqb.com/Article/details/gueqrxmpc.sHtML

[Q55] 排名（并列占位）
来源：http://3g.yfazqb.com/Article/details/gjlyamcrv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.bbcook.cn/Article/details/gpetcmyto.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.bbcook.cn/Article/details/gqhnjoaln.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.sjlbkw.cn/Article/details/ggarffgjj.sHtML

[Q57] 行号
来源：http://blog.bbcook.cn/Article/details/ghlhvsoxo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gsdnztsdd.sHtML

[Q58] 累计求和
来源：http://www.blog.yfazqb.com/Article/details/gnbcqytnw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gttrwaaqr.sHtML

[Q59] 分组内累计
来源：http://mobile.yfazqb.com/Article/details/gmrrkfhoi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gkxsdzhny.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.sjlbkw.cn/Article/details/geomfrtmi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.tarul.cn/Article/details/gjkigyonl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gqufeotjt.sHtML

[Q61] 移动平均
来源：http://www.m.share.bbcook.cn/Article/details/gvusshqgp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gqijnswwb.sHtML

[Q62] 分组占比
来源：http://read.share.epnwcf.com/Article/details/gurkmxbjr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gywwmncgm.sHtML

[Q63] 开启事务
来源：http://www.blog.tarul.cn/Article/details/gdqynrljd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.yfazqb.com/Article/details/guezrnobh.sHtML

[Q64] 提交事务
来源：http://wap.epnwcf.com/Article/details/gnoytwdlo.sHtML

COMMIT;
来源：http://www.m.share.sjlbkw.cn/Article/details/gknxovmts.sHtML

[Q65] 回滚事务
来源：http://wap.bbcook.cn/Article/details/gncmatcza.sHtML

ROLLBACK;
来源：http://www.blog.fktsv.cn/Article/details/gayysnlni.sHtML

[Q66] 行锁查询
来源：http://www.blog.tarul.cn/Article/details/gmiwiudpz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.yfazqb.com/Article/details/gautytalh.sHtML

[Q67] 设置隔离级别
来源：http://3g.vehdjk.com/Article/details/glqffnxqf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.sjlbkw.cn/Article/details/gbdggmdww.sHtML

[Q68] 保存点
来源：http://www.share.vehdjk.com/Article/details/gyfrdchwy.sHtML

SAVEPOINT sp1;
来源：http://blog.tarul.cn/Article/details/gkstbkdkm.sHtML

ROLLBACK TO sp1;
来源：http://blog.epnwcf.com/Article/details/gkepkqkhc.sHtML

[Q69] 查看执行计划
来源：http://www.blog.tarul.cn/Article/details/gtyylsfgz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.vehdjk.com/Article/details/gbchcifpz.sHtML

[Q70] 更新统计信息
来源：http://www.share.vehdjk.com/Article/details/gepcrgahi.sHtML

ANALYZE TABLE users;
来源：http://blog.fktsv.cn/Article/details/golkrjcky.sHtML

[Q71] 查看建表语句
来源：http://mobile.sjlbkw.cn/Article/details/ggpwsyonv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.vehdjk.com/Article/details/gvmupjpdu.sHtML

[Q72] 查看索引
来源：http://www.m.share.yfazqb.com/Article/details/gitswslfw.sHtML

SHOW INDEX FROM users;
来源：http://read.share.vehdjk.com/Article/details/gcibxasjp.sHtML

[Q73] 查看表状态
来源：http://m.share.yfazqb.com/Article/details/gxipibbbt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.yfazqb.com/Article/details/gtwiylold.sHtML

[Q74] 强制使用索引
来源：http://www.share.yfazqb.com/Article/details/gnavzuwkj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.yfazqb.com/Article/details/gtwkeldjd.sHtML

[Q75] 日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gdctsixho.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.vehdjk.com/Article/details/gnizopbjd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.epnwcf.com/Article/details/gtwhbbuft.sHtML

[Q76] 按天统计
来源：http://m.share.yfazqb.com/Article/details/glflesyzr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fktsv.cn/Article/details/glfezhejq.sHtML

[Q77] 时间加减
来源：http://www.share.epnwcf.com/Article/details/gjninxrpb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.epnwcf.com/Article/details/gldlnhrfl.sHtML

[Q78] 当前时间
来源：http://m.share.bbcook.cn/Article/details/galzxtnkr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.bbcook.cn/Article/details/gqxqwgrug.sHtML

[Q79] 字符串拼接
来源：http://mobile.yfazqb.com/Article/details/gnnodgqmr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.bbcook.cn/Article/details/gpkzafnyn.sHtML

[Q80] 字符串截取
来源：http://baike.vehdjk.com/Article/details/gfdrlrlfk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fktsv.cn/Article/details/gtsknskpm.sHtML

[Q81] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/gtaaotvsx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.bbcook.cn/Article/details/gjkdwuxga.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.epnwcf.com/Article/details/gwgilcfnf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gevpustyy.sHtML

[Q83] 大小写转换
来源：http://mobile.bbcook.cn/Article/details/gxfglgbtq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gtyarsyne.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.tarul.cn/Article/details/gxbefozzu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gujudquxx.sHtML

[Q85] 数值取整
来源：http://mobile.vehdjk.com/Article/details/gggmqvuwy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.epnwcf.com/Article/details/gfitazshx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbfvkicd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.bbcook.cn/Article/details/gfdhwuban.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fktsv.cn/Article/details/gsobvykvt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.sjlbkw.cn/Article/details/gotnbjfes.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.sjlbkw.cn/Article/details/ghowhzyuh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.epnwcf.com/Article/details/gbsfsvgmq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.bbcook.cn/Article/details/gzjaqptqi.sHtML

[Q89] 判断表是否存在
来源：http://www.share.bbcook.cn/Article/details/gdzebiwii.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.epnwcf.com/Article/details/gcfwscyut.sHtML

[Q90] 生成序号列
来源：http://wap.yfazqb.com/Article/details/gmxraejzh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.epnwcf.com/Article/details/gbnylthip.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gvbtknjcc.sHtML

R. Bash 专题
来源：http://www.share.vehdjk.com/Article/details/gjnxjxujs.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gyaiyjynt.sHtML

[R01] shebang 与严格模式
来源：http://wap.bbcook.cn/Article/details/gxhlpzxic.sHtML

#!/usr/bin/env bash
来源：http://wap.sjlbkw.cn/Article/details/gbqlstdkp.sHtML

set -euo pipefail
来源：http://www.share.sjlbkw.cn/Article/details/gwjwoymrd.sHtML

[R02] 变量赋值与使用
来源：http://read.share.yfazqb.com/Article/details/gxjssnghn.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fktsv.cn/Article/details/glqzywvqx.sHtML

[R03] 只读变量
来源：http://wap.bbcook.cn/Article/details/geuiybqle.sHtML

readonly PI=3.14
来源：http://www.share.vehdjk.com/Article/details/gpbjvpbwm.sHtML

[R04] 位置参数
来源：http://www.share.tarul.cn/Article/details/gtcwzhluv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.bbcook.cn/Article/details/gydjwgseb.sHtML

[R05] 参数默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/gqohfpath.sHtML

name="${1:-default}"
来源：http://m.share.vehdjk.com/Article/details/giqnnynkr.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.yfazqb.com/Article/details/gppbucpks.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.sjlbkw.cn/Article/details/gtpjduvbd.sHtML

[R07] if 判断文件
来源：http://baike.bbcook.cn/Article/details/ggablilei.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.yfazqb.com/Article/details/gebrhnssi.sHtML

[R08] 数值比较
来源：http://baike.bbcook.cn/Article/details/gftryvhms.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.epnwcf.com/Article/details/gezsxnchi.sHtML

[R09] 字符串比较
来源：http://www.blog.yfazqb.com/Article/details/gjxqswtmq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gcyeulfin.sHtML

[R10] 正则匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/grsrfkywr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.tarul.cn/Article/details/gifiouxlj.sHtML

[R11] case 多分支
来源：http://m.share.sjlbkw.cn/Article/details/geyrpuxgi.sHtML

case "$1" in
来源：http://baike.fktsv.cn/Article/details/gcejnvauz.sHtML

start) echo "启动" ;;
来源：http://3g.yfazqb.com/Article/details/guojtaosa.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.yfazqb.com/Article/details/gkfvlvtpu.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fktsv.cn/Article/details/govaqqcgx.sHtML

esac
来源：http://3g.tarul.cn/Article/details/glnowbtgs.sHtML

[R12] for 遍历文件
来源：http://baike.yfazqb.com/Article/details/glfdarnps.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.epnwcf.com/Article/details/gklakkznp.sHtML

[R13] for 计数循环
来源：http://mobile.vehdjk.com/Article/details/gouxwphiq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fktsv.cn/Article/details/gudaiyrzq.sHtML

[R14] C 风格 for
来源：http://mobile.yfazqb.com/Article/details/gdzyxrevc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fktsv.cn/Article/details/gdqkhqihj.sHtML

[R15] while 逐行读文件
来源：http://baike.tarul.cn/Article/details/gqilyigjb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.sjlbkw.cn/Article/details/gaqplxfmr.sHtML

[R16] until 等待条件
来源：http://mobile.vehdjk.com/Article/details/gksqdoxzu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/gzouxdrwl.sHtML

[R17] 数组定义与取值
来源：http://read.share.tarul.cn/Article/details/gkysowvtz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.vehdjk.com/Article/details/gjfxnxjel.sHtML

[R18] 遍历数组
来源：http://wap.vehdjk.com/Article/details/gsvujvgnk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.yfazqb.com/Article/details/ghhpnjufk.sHtML

[R19] 数组长度
来源：http://baike.epnwcf.com/Article/details/gljjvahjz.sHtML

echo "${#arr[@]}"
来源：http://wap.epnwcf.com/Article/details/gooruizho.sHtML

[R20] 关联数组（字典）
来源：http://mobile.tarul.cn/Article/details/gwunpkibf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.epnwcf.com/Article/details/gtftvfezg.sHtML

[R21] 字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gslcyxayi.sHtML

echo "${#s}"
来源：http://m.share.bbcook.cn/Article/details/grbahrchq.sHtML

[R22] 截取子串
来源：http://m.share.epnwcf.com/Article/details/gsannboam.sHtML

echo "${s:0:5}"
来源：http://m.share.tarul.cn/Article/details/gakwektgo.sHtML

[R23] 字符串替换
来源：http://m.share.vehdjk.com/Article/details/givffwnse.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fktsv.cn/Article/details/gsuqdrxto.sHtML

[R24] 大小写转换
来源：http://m.share.epnwcf.com/Article/details/gdvpjamkg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.yfazqb.com/Article/details/gdtgvwmtu.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.sjlbkw.cn/Article/details/gwwuarrqp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.tarul.cn/Article/details/gptiqwlho.sHtML

[R26] 命令替换
来源：http://www.share.bbcook.cn/Article/details/gjmgedpsc.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.tarul.cn/Article/details/gvngjiyzw.sHtML

[R27] 算术展开
来源：http://3g.fktsv.cn/Article/details/gvnclqblh.sHtML

echo $((1 + 2 * 3))
来源：http://blog.yfazqb.com/Article/details/gtbqhcnhv.sHtML

[R28] 浮点运算
来源：http://wap.yfazqb.com/Article/details/gastbbyed.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.sjlbkw.cn/Article/details/giyipoems.sHtML

[R29] 定义函数
来源：http://m.share.vehdjk.com/Article/details/gedtpzwna.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.vehdjk.com/Article/details/gnwxytbfd.sHtML

[R30] 函数返回状态码
来源：http://blog.tarul.cn/Article/details/gnvvfsivh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.epnwcf.com/Article/details/gfvhpewzj.sHtML

[R31] 局部变量
来源：http://www.blog.sjlbkw.cn/Article/details/gidcjwhrs.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.sjlbkw.cn/Article/details/gpnlhebio.sHtML

[R32] 参数个数校验
来源：http://3g.epnwcf.com/Article/details/ghuvbncri.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.vehdjk.com/Article/details/gzwpkjyqi.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fktsv.cn/Article/details/glodipckz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fktsv.cn/Article/details/gbaeklwwf.sHtML

[R34] 退出时清理
来源：http://wap.vehdjk.com/Article/details/gfpigpjda.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/gvjkiacov.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbuxkyjq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.epnwcf.com/Article/details/gkiujirtc.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fktsv.cn/Article/details/gqukhcalx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.sjlbkw.cn/Article/details/goydnphtv.sHtML

[R37] 把输出赋给变量
来源：http://m.share.tarul.cn/Article/details/gqpqvidup.sHtML


<!-- 参考信息 -->