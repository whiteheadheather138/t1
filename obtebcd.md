代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.bbcook.cn/Article/details/gnehgwhvp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fktsv.cn/Article/details/gfqqrtnqc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fktsv.cn/Article/details/gkuboxgdz.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.epnwcf.com/Article/details/gnlujlyhy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fktsv.cn/Article/details/gtzcflbru.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.vehdjk.com/Article/details/guflsysvi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fktsv.cn/Article/details/garwkcqxh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.yfazqb.com/Article/details/gtbrsrmrv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.epnwcf.com/Article/details/gtffokiqb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.yfazqb.com/Article/details/gptcioupp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.vehdjk.com/Article/details/glohbgqai.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fktsv.cn/Article/details/giaaouofc.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gvmbdgtak.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.sjlbkw.cn/Article/details/gxhccmmah.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gkrognxqv.sHtML

[Q01] 创建表
来源：http://www.blog.tarul.cn/Article/details/gqwjcbokc.sHtML

CREATE TABLE users (
来源：http://m.share.epnwcf.com/Article/details/gzimtvvnz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.sjlbkw.cn/Article/details/gbhznmtss.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.sjlbkw.cn/Article/details/gcombrjxx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.sjlbkw.cn/Article/details/gfwnnlkra.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.tarul.cn/Article/details/gunuihkqu.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/giwvscfac.sHtML

[Q02] 创建带外键的表
来源：http://3g.tarul.cn/Article/details/gqzymvpgh.sHtML

CREATE TABLE orders (
来源：http://baike.sjlbkw.cn/Article/details/gmvycryrc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.tarul.cn/Article/details/gfamtlhzr.sHtML

user_id INT NOT NULL,
来源：http://m.share.vehdjk.com/Article/details/gnrhpqiyk.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.epnwcf.com/Article/details/gfhbofmdr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.tarul.cn/Article/details/gejxcyimy.sHtML

);
来源：http://blog.bbcook.cn/Article/details/giqptifka.sHtML

[Q03] 增加列
来源：http://www.share.yfazqb.com/Article/details/geoyvnpwp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.vehdjk.com/Article/details/gbtcggndg.sHtML

[Q04] 修改列类型
来源：http://wap.vehdjk.com/Article/details/gzbanfjwq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.yfazqb.com/Article/details/gtgrbujnx.sHtML

[Q05] 重命名列
来源：http://read.share.sjlbkw.cn/Article/details/geyylxftp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.yfazqb.com/Article/details/gqpttjiwp.sHtML

[Q06] 删除列
来源：http://wap.yfazqb.com/Article/details/gnrqcfeoe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.yfazqb.com/Article/details/gtjpbmday.sHtML

[Q07] 删除表
来源：http://m.share.yfazqb.com/Article/details/gdvphtflt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwiqfgpiy.sHtML

[Q08] 创建普通索引
来源：http://mobile.fktsv.cn/Article/details/gjyzelyfj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/gwxqxatra.sHtML

[Q09] 创建唯一索引
来源：http://baike.sjlbkw.cn/Article/details/guzjyefhc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.sjlbkw.cn/Article/details/guobpkzud.sHtML

[Q10] 插入单行
来源：http://mobile.sjlbkw.cn/Article/details/ghclvgpjh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.epnwcf.com/Article/details/gcfracpcg.sHtML

[Q11] 一次插入多行
来源：http://mobile.fktsv.cn/Article/details/gqbcfubez.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fktsv.cn/Article/details/gxkzniatk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.sjlbkw.cn/Article/details/gtysucvtj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fktsv.cn/Article/details/grirzpykg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.tarul.cn/Article/details/gykrdvvct.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fktsv.cn/Article/details/guestnmpk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.tarul.cn/Article/details/gbjmofkrj.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.yfazqb.com/Article/details/gnjnpclcf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.tarul.cn/Article/details/ggswmysjq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.bbcook.cn/Article/details/gmhvbflix.sHtML

[Q15] 查询全部
来源：http://read.share.epnwcf.com/Article/details/ghncsckex.sHtML

SELECT * FROM users;
来源：http://mobile.tarul.cn/Article/details/grxchdthv.sHtML

[Q16] 查询指定列
来源：http://blog.tarul.cn/Article/details/gboofxsiw.sHtML

SELECT id, name FROM users;
来源：http://www.share.yfazqb.com/Article/details/gzmqurgpv.sHtML

[Q17] 条件查询
来源：http://read.share.yfazqb.com/Article/details/ghalwaeif.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fktsv.cn/Article/details/gcylvmgcp.sHtML

[Q18] 模糊匹配
来源：http://3g.sjlbkw.cn/Article/details/ggkhdmjqh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.tarul.cn/Article/details/gpwxosklg.sHtML

[Q19] 范围查询
来源：http://www.m.share.vehdjk.com/Article/details/glmojhqtc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbilyexz.sHtML

[Q20] IN 列表
来源：http://www.m.share.tarul.cn/Article/details/gncblygsv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.vehdjk.com/Article/details/gasrljuas.sHtML

[Q21] 空值判断
来源：http://www.blog.tarul.cn/Article/details/godfssgko.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.vehdjk.com/Article/details/gxgslnerv.sHtML

[Q22] 排序
来源：http://wap.vehdjk.com/Article/details/gezzgfwqi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.tarul.cn/Article/details/gggubfzob.sHtML

[Q23] 分页
来源：http://blog.epnwcf.com/Article/details/glkgfgdxu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.epnwcf.com/Article/details/gnangdxsg.sHtML

[Q24] 去重
来源：http://blog.yfazqb.com/Article/details/gvdgnezmp.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gdkvqqmzy.sHtML

[Q25] 只取前 N 条
来源：http://baike.bbcook.cn/Article/details/gpvcrvtot.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.sjlbkw.cn/Article/details/gofahifcp.sHtML

[Q26] 计数
来源：http://baike.yfazqb.com/Article/details/gsoszqwsy.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.yfazqb.com/Article/details/guepismcq.sHtML

[Q27] 条件计数
来源：http://read.share.vehdjk.com/Article/details/gefjlznej.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/grnhliblu.sHtML

[Q28] 求和与平均
来源：http://www.blog.bbcook.cn/Article/details/gvonsqzsl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gkpxlwhaq.sHtML

[Q29] 最大最小值
来源：http://wap.bbcook.cn/Article/details/guzxaqweo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.epnwcf.com/Article/details/glymfstrl.sHtML

[Q30] 分组统计
来源：http://www.share.bbcook.cn/Article/details/gaplubxik.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gqlnuiwru.sHtML

[Q31] 分组后过滤
来源：http://wap.vehdjk.com/Article/details/gitkdzejy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.tarul.cn/Article/details/gchrrqoza.sHtML

[Q32] 分组拼接字符串
来源：http://baike.yfazqb.com/Article/details/gldgsacmy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/grhevprnm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.epnwcf.com/Article/details/gzmzvceep.sHtML

[Q33] 多列分组
来源：http://wap.sjlbkw.cn/Article/details/gvyrbbxvj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.vehdjk.com/Article/details/gevhrjuca.sHtML

[Q34] 每组取第一条
来源：http://www.blog.sjlbkw.cn/Article/details/grjbzzvsi.sHtML

SELECT * FROM (
来源：http://m.share.fktsv.cn/Article/details/gzucivabz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.epnwcf.com/Article/details/grvhpqnam.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gwmbamzsu.sHtML

[Q35] 内连接
来源：http://mobile.bbcook.cn/Article/details/gkzdznkyx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/gbbhfzfel.sHtML

[Q36] 左连接
来源：http://www.blog.bbcook.cn/Article/details/ghinrhtak.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.bbcook.cn/Article/details/gznrgouub.sHtML

[Q37] 右连接
来源：http://www.blog.sjlbkw.cn/Article/details/gnastcnhf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.tarul.cn/Article/details/gbhtzrvgq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.sjlbkw.cn/Article/details/gogmoypfl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.sjlbkw.cn/Article/details/ggzrbgqpl.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.yfazqb.com/Article/details/gizmwjvhm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.tarul.cn/Article/details/guhbumiev.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fktsv.cn/Article/details/gvfhgpiyu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.bbcook.cn/Article/details/gfsichsgj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.sjlbkw.cn/Article/details/gbjzbbgvt.sHtML

[Q41] 多表连接
来源：http://3g.epnwcf.com/Article/details/gtjrcyyja.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.bbcook.cn/Article/details/grsjjbiji.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.tarul.cn/Article/details/ghubeegni.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.bbcook.cn/Article/details/gnvyhjvjf.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.bbcook.cn/Article/details/gnlaipajc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.bbcook.cn/Article/details/gqtvgwhya.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.vehdjk.com/Article/details/giuoryzkq.sHtML

[Q43] 标量子查询
来源：http://blog.bbcook.cn/Article/details/gmhmswbno.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.yfazqb.com/Article/details/gpybghyed.sHtML

[Q44] IN 子查询
来源：http://wap.fktsv.cn/Article/details/gfdycgffk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.bbcook.cn/Article/details/gdvibxtcz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.tarul.cn/Article/details/gxfscvccr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/gcjaguavn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.yfazqb.com/Article/details/gijrloqhx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.yfazqb.com/Article/details/gcyelsact.sHtML

[Q47] 与平均值比较
来源：http://wap.vehdjk.com/Article/details/gijlyceiq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.sjlbkw.cn/Article/details/glaijfygg.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.tarul.cn/Article/details/ghxaiqnyi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.yfazqb.com/Article/details/gjdfjkgwb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.epnwcf.com/Article/details/gckmkfsil.sHtML

[Q49] 更新单行
来源：http://3g.bbcook.cn/Article/details/gouyygluz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.yfazqb.com/Article/details/gcksmiugi.sHtML

[Q50] 批量更新
来源：http://m.share.vehdjk.com/Article/details/gdrqoefcu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fktsv.cn/Article/details/ggnqfrgjv.sHtML

[Q51] 用子查询更新
来源：http://baike.fktsv.cn/Article/details/gocoahnzk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.epnwcf.com/Article/details/givbszwcb.sHtML

[Q52] 删除指定行
来源：http://www.share.tarul.cn/Article/details/gztyhvgal.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/grljpwnam.sHtML

[Q53] 按条件删除
来源：http://baike.fktsv.cn/Article/details/gpwvfrvyn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.tarul.cn/Article/details/gykipmwbx.sHtML

[Q54] 清空表
来源：http://www.blog.vehdjk.com/Article/details/gfxftbiuj.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fktsv.cn/Article/details/gydssnmsv.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.sjlbkw.cn/Article/details/gtsbvfkns.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.bbcook.cn/Article/details/gmiytvxhy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.bbcook.cn/Article/details/gayvygrgr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.bbcook.cn/Article/details/gkwszmafw.sHtML

[Q57] 行号
来源：http://read.share.epnwcf.com/Article/details/gieqjahcw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.tarul.cn/Article/details/gnnlofxsq.sHtML

[Q58] 累计求和
来源：http://blog.epnwcf.com/Article/details/gwvhxxyqk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gqflimlnu.sHtML

[Q59] 分组内累计
来源：http://mobile.yfazqb.com/Article/details/gfypatdlh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gkhkckexk.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.yfazqb.com/Article/details/gcwniesbh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.epnwcf.com/Article/details/gblasenwi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.epnwcf.com/Article/details/ggzamqfdu.sHtML

[Q61] 移动平均
来源：http://mobile.bbcook.cn/Article/details/gcpyqusmt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gkspnhcxk.sHtML

[Q62] 分组占比
来源：http://read.share.bbcook.cn/Article/details/gjraledor.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gokfmlnlf.sHtML

[Q63] 开启事务
来源：http://www.blog.bbcook.cn/Article/details/gzgdnzgyg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.tarul.cn/Article/details/glbapnxtw.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/gptkxjwfb.sHtML

COMMIT;
来源：http://www.blog.fktsv.cn/Article/details/gdiyjcxge.sHtML

[Q65] 回滚事务
来源：http://wap.bbcook.cn/Article/details/gefknfwuv.sHtML

ROLLBACK;
来源：http://3g.bbcook.cn/Article/details/grpayqoba.sHtML

[Q66] 行锁查询
来源：http://3g.vehdjk.com/Article/details/gyiznjxgj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.bbcook.cn/Article/details/gegbpnkut.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fktsv.cn/Article/details/gjftifefj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.epnwcf.com/Article/details/gmkzydkwm.sHtML

[Q68] 保存点
来源：http://m.share.vehdjk.com/Article/details/gktcwnhme.sHtML

SAVEPOINT sp1;
来源：http://www.blog.yfazqb.com/Article/details/gxlvjcesj.sHtML

ROLLBACK TO sp1;
来源：http://www.share.yfazqb.com/Article/details/gmhuejqeq.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.tarul.cn/Article/details/gxclniube.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.tarul.cn/Article/details/ggrqmndan.sHtML

[Q70] 更新统计信息
来源：http://baike.fktsv.cn/Article/details/gpwtehljr.sHtML

ANALYZE TABLE users;
来源：http://wap.bbcook.cn/Article/details/gbvyvvthr.sHtML

[Q71] 查看建表语句
来源：http://www.blog.tarul.cn/Article/details/gylsopuvu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.yfazqb.com/Article/details/gqhhoiwvp.sHtML

[Q72] 查看索引
来源：http://mobile.bbcook.cn/Article/details/gettwegar.sHtML

SHOW INDEX FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gbbsvkwzc.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fktsv.cn/Article/details/grsiocpxc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.epnwcf.com/Article/details/gqlbyjalz.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.epnwcf.com/Article/details/gyjlsgwdd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.yfazqb.com/Article/details/gsapsdksy.sHtML

[Q75] 日期格式化
来源：http://m.share.tarul.cn/Article/details/gdjtpjomz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.vehdjk.com/Article/details/gxikendjb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.vehdjk.com/Article/details/gqlstruoq.sHtML

[Q76] 按天统计
来源：http://3g.bbcook.cn/Article/details/govcspibg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.epnwcf.com/Article/details/gmomvmvsd.sHtML

[Q77] 时间加减
来源：http://wap.vehdjk.com/Article/details/gwrhxxbrq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.tarul.cn/Article/details/gzyfsextm.sHtML

[Q78] 当前时间
来源：http://baike.fktsv.cn/Article/details/giaagmgts.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.yfazqb.com/Article/details/gejjcalud.sHtML

[Q79] 字符串拼接
来源：http://www.blog.bbcook.cn/Article/details/gokxywvln.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.bbcook.cn/Article/details/gablwpjof.sHtML

[Q80] 字符串截取
来源：http://mobile.tarul.cn/Article/details/gekenvwfy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.epnwcf.com/Article/details/goazwgygt.sHtML

[Q81] 字符串替换
来源：http://3g.vehdjk.com/Article/details/gznehhipm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fktsv.cn/Article/details/gajyeusii.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.tarul.cn/Article/details/gbfqocwsy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gknucvewe.sHtML

[Q83] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/galgiuphh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/ggwwvrwki.sHtML

[Q84] 去除首尾空格
来源：http://m.share.vehdjk.com/Article/details/gjbrkjkve.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gtkwudqeu.sHtML

[Q85] 数值取整
来源：http://www.blog.fktsv.cn/Article/details/gkwwowsrf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.epnwcf.com/Article/details/gjyyllygl.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.bbcook.cn/Article/details/gwjzzvdep.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fktsv.cn/Article/details/gpalxalcc.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.epnwcf.com/Article/details/gpcptiudt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.bbcook.cn/Article/details/gtpgsbwer.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.epnwcf.com/Article/details/gywopklyj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.yfazqb.com/Article/details/ghbkqdvsf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.vehdjk.com/Article/details/gieelbysm.sHtML

[Q89] 判断表是否存在
来源：http://m.share.epnwcf.com/Article/details/gnuazklxi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.yfazqb.com/Article/details/gbvoeqqpv.sHtML

[Q90] 生成序号列
来源：http://www.share.bbcook.cn/Article/details/grqovarjo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.vehdjk.com/Article/details/gdxyaoiyt.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gursvcrzk.sHtML

R. Bash 专题
来源：http://wap.bbcook.cn/Article/details/gakfnwekc.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gnblsigwo.sHtML

[R01] shebang 与严格模式
来源：http://baike.yfazqb.com/Article/details/grglzzdjz.sHtML

#!/usr/bin/env bash
来源：http://mobile.fktsv.cn/Article/details/gnnlzrlqd.sHtML

set -euo pipefail
来源：http://3g.tarul.cn/Article/details/gizlsxtyu.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.bbcook.cn/Article/details/gyhukcdyj.sHtML

name="Tom"; echo "$name"
来源：http://blog.tarul.cn/Article/details/gwqrpcbls.sHtML

[R03] 只读变量
来源：http://read.share.vehdjk.com/Article/details/gqrqgmiri.sHtML

readonly PI=3.14
来源：http://baike.vehdjk.com/Article/details/gnaodtcab.sHtML

[R04] 位置参数
来源：http://m.share.fktsv.cn/Article/details/gjgbfeumq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.epnwcf.com/Article/details/gguopfxiq.sHtML

[R05] 参数默认值
来源：http://3g.sjlbkw.cn/Article/details/grdyceref.sHtML

name="${1:-default}"
来源：http://mobile.fktsv.cn/Article/details/gmqiuwnxh.sHtML

[R06] 判断命令是否存在
来源：http://baike.tarul.cn/Article/details/gfnjdlhlz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/gjgukqzdv.sHtML

[R07] if 判断文件
来源：http://www.blog.epnwcf.com/Article/details/gzkicbyxy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fktsv.cn/Article/details/gudqfqryh.sHtML

[R08] 数值比较
来源：http://www.share.vehdjk.com/Article/details/ggqlwmuyf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.sjlbkw.cn/Article/details/ghbaoxhad.sHtML

[R09] 字符串比较
来源：http://www.blog.sjlbkw.cn/Article/details/gufsnowip.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.sjlbkw.cn/Article/details/gksxavjcg.sHtML

[R10] 正则匹配
来源：http://www.blog.vehdjk.com/Article/details/gjeikeyuq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fktsv.cn/Article/details/gkhjkernf.sHtML

[R11] case 多分支
来源：http://blog.epnwcf.com/Article/details/glkvznxnx.sHtML

case "$1" in
来源：http://www.m.share.bbcook.cn/Article/details/gfgaxxkly.sHtML

start) echo "启动" ;;
来源：http://wap.yfazqb.com/Article/details/gblyhgrnd.sHtML

stop)  echo "停止" ;;
来源：http://read.share.yfazqb.com/Article/details/gdkbejrwt.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.tarul.cn/Article/details/gkrquohcx.sHtML

esac
来源：http://www.share.sjlbkw.cn/Article/details/gpwsdmzzu.sHtML

[R12] for 遍历文件
来源：http://www.blog.yfazqb.com/Article/details/gqvlquena.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fktsv.cn/Article/details/gvljdrzby.sHtML

[R13] for 计数循环
来源：http://baike.bbcook.cn/Article/details/gqgtejjow.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.yfazqb.com/Article/details/gyboqimtz.sHtML

[R14] C 风格 for
来源：http://www.blog.vehdjk.com/Article/details/gavjmcprt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.epnwcf.com/Article/details/gpbtstryh.sHtML

[R15] while 逐行读文件
来源：http://mobile.tarul.cn/Article/details/grhxgalii.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.bbcook.cn/Article/details/gybklxguu.sHtML

[R16] until 等待条件
来源：http://3g.bbcook.cn/Article/details/gydlbvvah.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.sjlbkw.cn/Article/details/gltudneju.sHtML

[R17] 数组定义与取值
来源：http://m.share.bbcook.cn/Article/details/goqaojlgf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.tarul.cn/Article/details/gvqhevuct.sHtML

[R18] 遍历数组
来源：http://m.share.vehdjk.com/Article/details/gkrdrqilw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.yfazqb.com/Article/details/geiqcbqcy.sHtML

[R19] 数组长度
来源：http://wap.fktsv.cn/Article/details/gqfoyjzjz.sHtML

echo "${#arr[@]}"
来源：http://wap.bbcook.cn/Article/details/gwqrgnqzy.sHtML

[R20] 关联数组（字典）
来源：http://www.share.sjlbkw.cn/Article/details/gdhsnyiek.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.epnwcf.com/Article/details/gdqelixso.sHtML

[R21] 字符串长度
来源：http://read.share.tarul.cn/Article/details/gtmukvtvc.sHtML

echo "${#s}"
来源：http://mobile.epnwcf.com/Article/details/ghskqagwj.sHtML

[R22] 截取子串
来源：http://m.share.epnwcf.com/Article/details/gvwgprxae.sHtML

echo "${s:0:5}"
来源：http://www.m.share.epnwcf.com/Article/details/gkjuaejow.sHtML

[R23] 字符串替换
来源：http://wap.epnwcf.com/Article/details/gpczsabzp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.yfazqb.com/Article/details/gieuqweah.sHtML

[R24] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gmauvkmzo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fktsv.cn/Article/details/gktatrwel.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.yfazqb.com/Article/details/gllyjvnmc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.epnwcf.com/Article/details/gormjayuy.sHtML

[R26] 命令替换
来源：http://baike.yfazqb.com/Article/details/gsoynegzi.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.yfazqb.com/Article/details/gtuooofrs.sHtML

[R27] 算术展开
来源：http://wap.sjlbkw.cn/Article/details/gitislqcr.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fktsv.cn/Article/details/gmtupjsmz.sHtML

[R28] 浮点运算
来源：http://www.share.epnwcf.com/Article/details/gbxfilxyd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.yfazqb.com/Article/details/gblosmhry.sHtML

[R29] 定义函数
来源：http://www.share.epnwcf.com/Article/details/gvoycqxnq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.sjlbkw.cn/Article/details/gxlkyxgfg.sHtML

[R30] 函数返回状态码
来源：http://www.blog.bbcook.cn/Article/details/gnsnfvgxq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.tarul.cn/Article/details/gaahksjiu.sHtML

[R31] 局部变量
来源：http://blog.epnwcf.com/Article/details/guyozpveq.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fktsv.cn/Article/details/gsvwrqoeg.sHtML

[R32] 参数个数校验
来源：http://m.share.yfazqb.com/Article/details/gpstsaoff.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fktsv.cn/Article/details/gddwccbrz.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.bbcook.cn/Article/details/gmaabbyag.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.bbcook.cn/Article/details/ggkgrhfia.sHtML

[R34] 退出时清理
来源：http://www.m.share.epnwcf.com/Article/details/gkvdlqmfo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.epnwcf.com/Article/details/gqacaeibn.sHtML

[R35] 后台执行并等待
来源：http://blog.epnwcf.com/Article/details/gnfdxpynt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fktsv.cn/Article/details/gupwtakdf.sHtML

[R36] 并发执行多个任务
来源：http://m.share.bbcook.cn/Article/details/gmrnatdla.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.tarul.cn/Article/details/gdhunboez.sHtML

[R37] 把输出赋给变量
来源：http://read.share.bbcook.cn/Article/details/ggblmecxi.sHtML


<!-- 参考信息 -->