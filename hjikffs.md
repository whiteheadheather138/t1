代发 wailian999

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ghkkfeagd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.epnwcf.com/Article/details/gmwvjcpod.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gcezuysiq.sHtML

[Q01] 创建表
来源：http://baike.fktsv.cn/Article/details/gcjpyoygd.sHtML

CREATE TABLE users (
来源：http://read.share.tarul.cn/Article/details/gixwffwxj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.tarul.cn/Article/details/gvpamfyes.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.vehdjk.com/Article/details/gvrynqipo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.tarul.cn/Article/details/grhjsaerc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.yfazqb.com/Article/details/gmtqipqco.sHtML

);
来源：http://www.m.share.fktsv.cn/Article/details/gyepaesox.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fktsv.cn/Article/details/gebpokpge.sHtML

CREATE TABLE orders (
来源：http://blog.fktsv.cn/Article/details/gtewpcmsv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.epnwcf.com/Article/details/ghwvwljdu.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.sjlbkw.cn/Article/details/gefchwxwz.sHtML

amount DECIMAL(10, 2),
来源：http://3g.bbcook.cn/Article/details/gfscsthla.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.vehdjk.com/Article/details/gykupiigc.sHtML

);
来源：http://3g.sjlbkw.cn/Article/details/guwzpiubk.sHtML

[Q03] 增加列
来源：http://mobile.fktsv.cn/Article/details/gpfltbjoh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.epnwcf.com/Article/details/gkrrbjrml.sHtML

[Q04] 修改列类型
来源：http://read.share.sjlbkw.cn/Article/details/gddjnuddt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fktsv.cn/Article/details/gzusjkpix.sHtML

[Q05] 重命名列
来源：http://www.m.share.vehdjk.com/Article/details/gknczupcz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.sjlbkw.cn/Article/details/gnzpssjle.sHtML

[Q06] 删除列
来源：http://www.blog.tarul.cn/Article/details/giwymlxfm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.vehdjk.com/Article/details/gummwysyj.sHtML

[Q07] 删除表
来源：http://www.blog.vehdjk.com/Article/details/gvclcmgzx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.yfazqb.com/Article/details/gbahmpxed.sHtML

[Q08] 创建普通索引
来源：http://blog.epnwcf.com/Article/details/gletjiona.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/gxnvkfvyr.sHtML

[Q09] 创建唯一索引
来源：http://3g.vehdjk.com/Article/details/gncvnbotc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.yfazqb.com/Article/details/glpyjqfwp.sHtML

[Q10] 插入单行
来源：http://mobile.yfazqb.com/Article/details/gjzsqminx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.epnwcf.com/Article/details/gwcdfyrjt.sHtML

[Q11] 一次插入多行
来源：http://m.share.sjlbkw.cn/Article/details/guwlwbjpv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/gmjunbulr.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.sjlbkw.cn/Article/details/gacpqktla.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.sjlbkw.cn/Article/details/gzwxqgkhi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fktsv.cn/Article/details/gjgayspcf.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fktsv.cn/Article/details/gqbbjvzlg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.tarul.cn/Article/details/goxoefjap.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.tarul.cn/Article/details/gbprrjakm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.bbcook.cn/Article/details/gcasxgzhf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.yfazqb.com/Article/details/gjwpbmilo.sHtML

[Q15] 查询全部
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhfabfpy.sHtML

SELECT * FROM users;
来源：http://read.share.yfazqb.com/Article/details/grzxoiutw.sHtML

[Q16] 查询指定列
来源：http://www.blog.bbcook.cn/Article/details/gjwtidbak.sHtML

SELECT id, name FROM users;
来源：http://mobile.epnwcf.com/Article/details/ghtyybkfc.sHtML

[Q17] 条件查询
来源：http://wap.yfazqb.com/Article/details/gtzrrcsrj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.yfazqb.com/Article/details/gitmvsagl.sHtML

[Q18] 模糊匹配
来源：http://wap.sjlbkw.cn/Article/details/gmoojliub.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.tarul.cn/Article/details/gccepugdj.sHtML

[Q19] 范围查询
来源：http://www.share.tarul.cn/Article/details/gznkiiraq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.vehdjk.com/Article/details/gmpooqdqn.sHtML

[Q20] IN 列表
来源：http://mobile.yfazqb.com/Article/details/guemadgpw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.epnwcf.com/Article/details/gifqjvppy.sHtML

[Q21] 空值判断
来源：http://blog.sjlbkw.cn/Article/details/giruoubev.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.tarul.cn/Article/details/gizkrfvuo.sHtML

[Q22] 排序
来源：http://wap.sjlbkw.cn/Article/details/gptrecbhi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.sjlbkw.cn/Article/details/gfxrjknsm.sHtML

[Q23] 分页
来源：http://www.blog.yfazqb.com/Article/details/gdtesbbvk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.yfazqb.com/Article/details/gktjywbmd.sHtML

[Q24] 去重
来源：http://wap.yfazqb.com/Article/details/galskuhcx.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.yfazqb.com/Article/details/gcylmsyrx.sHtML

[Q25] 只取前 N 条
来源：http://m.share.yfazqb.com/Article/details/gnilqnzjl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/gnvpxvwyj.sHtML

[Q26] 计数
来源：http://wap.tarul.cn/Article/details/gkfliheyw.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.tarul.cn/Article/details/gpoyqzzcx.sHtML

[Q27] 条件计数
来源：http://www.share.bbcook.cn/Article/details/ghduuinzr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.vehdjk.com/Article/details/glootisup.sHtML

[Q28] 求和与平均
来源：http://www.share.vehdjk.com/Article/details/gmyjsfmqe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gartdcxza.sHtML

[Q29] 最大最小值
来源：http://baike.bbcook.cn/Article/details/geoputhza.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gazugyppl.sHtML

[Q30] 分组统计
来源：http://www.blog.bbcook.cn/Article/details/gxtljfece.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gflctrqhq.sHtML

[Q31] 分组后过滤
来源：http://read.share.bbcook.cn/Article/details/geqoqpmpo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.yfazqb.com/Article/details/goealtolt.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/ghwyjdxgn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gqapkcypp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.vehdjk.com/Article/details/gzcgocfam.sHtML

[Q33] 多列分组
来源：http://3g.sjlbkw.cn/Article/details/gsaslzswn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fktsv.cn/Article/details/gtbnvcmyk.sHtML

[Q34] 每组取第一条
来源：http://mobile.fktsv.cn/Article/details/guaigsafm.sHtML

SELECT * FROM (
来源：http://mobile.epnwcf.com/Article/details/gtxgnaswt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.vehdjk.com/Article/details/gllenafvy.sHtML

) t WHERE rn = 1;
来源：http://wap.epnwcf.com/Article/details/ghjtmeixw.sHtML

[Q35] 内连接
来源：http://3g.sjlbkw.cn/Article/details/ghzeyfccg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.epnwcf.com/Article/details/gwgfkdvti.sHtML

[Q36] 左连接
来源：http://mobile.sjlbkw.cn/Article/details/gjtwcoosv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.vehdjk.com/Article/details/glhnjhljd.sHtML

[Q37] 右连接
来源：http://mobile.fktsv.cn/Article/details/gyrvvbpil.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fktsv.cn/Article/details/gmyaikymp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.vehdjk.com/Article/details/gybkcxqqg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.tarul.cn/Article/details/guxjihmtr.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.epnwcf.com/Article/details/geepbbajg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.vehdjk.com/Article/details/gohpxtihm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.tarul.cn/Article/details/gcacjybaw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fktsv.cn/Article/details/gvgxhissq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.epnwcf.com/Article/details/ganifgnte.sHtML

[Q41] 多表连接
来源：http://read.share.bbcook.cn/Article/details/gusxgemfb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.epnwcf.com/Article/details/gfhevbbqp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.vehdjk.com/Article/details/gnpoxjhmy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.tarul.cn/Article/details/gyvtpkrzy.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.vehdjk.com/Article/details/gxpbaftjl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fktsv.cn/Article/details/gwojrcuhh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.tarul.cn/Article/details/gbokoyoyi.sHtML

[Q43] 标量子查询
来源：http://blog.vehdjk.com/Article/details/gnltzgbqu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fktsv.cn/Article/details/gcmsmikgc.sHtML

[Q44] IN 子查询
来源：http://www.share.bbcook.cn/Article/details/ghmleiral.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.yfazqb.com/Article/details/gfzusduxw.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdhjcjbi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.tarul.cn/Article/details/gzebpbkvk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.yfazqb.com/Article/details/ghxoagcou.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/gliwdzakv.sHtML

[Q47] 与平均值比较
来源：http://blog.sjlbkw.cn/Article/details/gttcpvlzv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.vehdjk.com/Article/details/gkfpsbujw.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.epnwcf.com/Article/details/gyeosppxb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fktsv.cn/Article/details/gpnyawibs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fktsv.cn/Article/details/gbmopwgrd.sHtML

[Q49] 更新单行
来源：http://read.share.bbcook.cn/Article/details/gqahsvgws.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/gjhvokbrd.sHtML

[Q50] 批量更新
来源：http://www.share.vehdjk.com/Article/details/gvckgolye.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fktsv.cn/Article/details/gscwxtnoj.sHtML

[Q51] 用子查询更新
来源：http://baike.epnwcf.com/Article/details/gnrfbefyl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.tarul.cn/Article/details/gkyeilpzo.sHtML

[Q52] 删除指定行
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrlvtkkt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.tarul.cn/Article/details/gedtyjnwc.sHtML

[Q53] 按条件删除
来源：http://baike.epnwcf.com/Article/details/grmufwqzw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.vehdjk.com/Article/details/ggnakjzdt.sHtML

[Q54] 清空表
来源：http://3g.sjlbkw.cn/Article/details/gjzrbjolq.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fktsv.cn/Article/details/gogfhleax.sHtML

[Q55] 排名（并列占位）
来源：http://wap.tarul.cn/Article/details/gwnbupdpg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.sjlbkw.cn/Article/details/gvjpmgkad.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.vehdjk.com/Article/details/glbfpzrzx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.sjlbkw.cn/Article/details/gunjhetcj.sHtML

[Q57] 行号
来源：http://mobile.yfazqb.com/Article/details/gvjzqhlxf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.vehdjk.com/Article/details/gkuufneyx.sHtML

[Q58] 累计求和
来源：http://www.m.share.tarul.cn/Article/details/gzelfjjzi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fktsv.cn/Article/details/gokyjzsnn.sHtML

[Q59] 分组内累计
来源：http://wap.bbcook.cn/Article/details/gearqxyuw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gtqumznfm.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fktsv.cn/Article/details/grdfgcbbu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.sjlbkw.cn/Article/details/gbirecwuk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gldgvpvxy.sHtML

[Q61] 移动平均
来源：http://www.share.epnwcf.com/Article/details/ghvkwkvwi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/ghwpvbxgs.sHtML

[Q62] 分组占比
来源：http://www.share.bbcook.cn/Article/details/gvjjghbdh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/gnpajeupz.sHtML

[Q63] 开启事务
来源：http://www.blog.tarul.cn/Article/details/goewprfty.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fktsv.cn/Article/details/gfemnytwb.sHtML

[Q64] 提交事务
来源：http://m.share.tarul.cn/Article/details/gkpvfcgrc.sHtML

COMMIT;
来源：http://baike.epnwcf.com/Article/details/gqhdmvzzl.sHtML

[Q65] 回滚事务
来源：http://mobile.fktsv.cn/Article/details/gsnsyqcli.sHtML

ROLLBACK;
来源：http://wap.tarul.cn/Article/details/gjovwdpld.sHtML

[Q66] 行锁查询
来源：http://wap.fktsv.cn/Article/details/gljmsdqer.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.vehdjk.com/Article/details/guxearnuo.sHtML

[Q67] 设置隔离级别
来源：http://baike.sjlbkw.cn/Article/details/gifxttlpt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.epnwcf.com/Article/details/gygeaiytc.sHtML

[Q68] 保存点
来源：http://baike.epnwcf.com/Article/details/gqewedarv.sHtML

SAVEPOINT sp1;
来源：http://baike.bbcook.cn/Article/details/gbppbiopw.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.epnwcf.com/Article/details/gbbwmobem.sHtML

[Q69] 查看执行计划
来源：http://blog.fktsv.cn/Article/details/gciddbayi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fktsv.cn/Article/details/gwfhajtel.sHtML

[Q70] 更新统计信息
来源：http://read.share.sjlbkw.cn/Article/details/gxayegbot.sHtML

ANALYZE TABLE users;
来源：http://blog.vehdjk.com/Article/details/gpizuslqc.sHtML

[Q71] 查看建表语句
来源：http://www.share.bbcook.cn/Article/details/gdoaxzfac.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fktsv.cn/Article/details/gofiyvkfu.sHtML

[Q72] 查看索引
来源：http://www.share.tarul.cn/Article/details/gceduglvq.sHtML

SHOW INDEX FROM users;
来源：http://www.share.epnwcf.com/Article/details/gzrhyiinh.sHtML

[Q73] 查看表状态
来源：http://baike.fktsv.cn/Article/details/gsvtindvs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fktsv.cn/Article/details/gvqljcbgs.sHtML

[Q74] 强制使用索引
来源：http://m.share.vehdjk.com/Article/details/gigajiwux.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.bbcook.cn/Article/details/gycwygceq.sHtML

[Q75] 日期格式化
来源：http://mobile.vehdjk.com/Article/details/gwkbhvvzf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gaggcsmcq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.tarul.cn/Article/details/gwvsfupzi.sHtML

[Q76] 按天统计
来源：http://blog.bbcook.cn/Article/details/grmyjvkpe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.sjlbkw.cn/Article/details/gfoymazwt.sHtML

[Q77] 时间加减
来源：http://www.blog.sjlbkw.cn/Article/details/ggulkzqiu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.sjlbkw.cn/Article/details/gbxpwawth.sHtML

[Q78] 当前时间
来源：http://mobile.yfazqb.com/Article/details/guhvoquna.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.epnwcf.com/Article/details/gbvidhaix.sHtML

[Q79] 字符串拼接
来源：http://www.blog.sjlbkw.cn/Article/details/gmiqskppp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.tarul.cn/Article/details/gqjdwaraz.sHtML

[Q80] 字符串截取
来源：http://wap.epnwcf.com/Article/details/gklneogug.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gcslwkydb.sHtML

[Q81] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/gzxfhitzh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.tarul.cn/Article/details/gqgbmmaat.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.epnwcf.com/Article/details/gidpvvmcp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/ghwnbhwlp.sHtML

[Q83] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/gmspwgfew.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gsulzpvyh.sHtML

[Q84] 去除首尾空格
来源：http://blog.tarul.cn/Article/details/gmithwzdi.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gydtggelf.sHtML

[Q85] 数值取整
来源：http://m.share.epnwcf.com/Article/details/gtuzfgtrb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.bbcook.cn/Article/details/gonacldpm.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.epnwcf.com/Article/details/gsevpfmdn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.yfazqb.com/Article/details/gbtwbxmuc.sHtML

[Q87] JSON 字段做条件
来源：http://3g.epnwcf.com/Article/details/gvtovedda.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.yfazqb.com/Article/details/gwrnqmbbt.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.yfazqb.com/Article/details/gfzupukpp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.tarul.cn/Article/details/gblekyqzy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.epnwcf.com/Article/details/gliburwzw.sHtML

[Q89] 判断表是否存在
来源：http://3g.vehdjk.com/Article/details/gorpsyfwq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.epnwcf.com/Article/details/gidnlvqoo.sHtML

[Q90] 生成序号列
来源：http://wap.tarul.cn/Article/details/gbbyonrdm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.sjlbkw.cn/Article/details/gcenrkxbs.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gnvbftwfn.sHtML

R. Bash 专题
来源：http://www.m.share.vehdjk.com/Article/details/goqctyhbk.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/guqpwipjq.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fktsv.cn/Article/details/gkupalusw.sHtML

#!/usr/bin/env bash
来源：http://read.share.tarul.cn/Article/details/gpdviabay.sHtML

set -euo pipefail
来源：http://3g.yfazqb.com/Article/details/gyovtbwms.sHtML

[R02] 变量赋值与使用
来源：http://www.share.epnwcf.com/Article/details/gdsssndez.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.tarul.cn/Article/details/gxvmrrhck.sHtML

[R03] 只读变量
来源：http://blog.sjlbkw.cn/Article/details/grhqicawe.sHtML

readonly PI=3.14
来源：http://wap.tarul.cn/Article/details/gqwksuybi.sHtML

[R04] 位置参数
来源：http://wap.epnwcf.com/Article/details/gjluaptua.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.bbcook.cn/Article/details/gycpjexwm.sHtML

[R05] 参数默认值
来源：http://blog.fktsv.cn/Article/details/gwftguaxz.sHtML

name="${1:-default}"
来源：http://www.m.share.epnwcf.com/Article/details/gpszqlvoj.sHtML

[R06] 判断命令是否存在
来源：http://m.share.vehdjk.com/Article/details/gvksyiznf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.vehdjk.com/Article/details/gollxjcku.sHtML

[R07] if 判断文件
来源：http://baike.yfazqb.com/Article/details/gnavmzaru.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.epnwcf.com/Article/details/gzhlxsfjd.sHtML

[R08] 数值比较
来源：http://www.m.share.tarul.cn/Article/details/gutbfgutv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.vehdjk.com/Article/details/gzlmjxbkk.sHtML

[R09] 字符串比较
来源：http://blog.epnwcf.com/Article/details/gdfnmljla.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.epnwcf.com/Article/details/gchkdpkyb.sHtML

[R10] 正则匹配
来源：http://m.share.fktsv.cn/Article/details/glifjkjgn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.bbcook.cn/Article/details/gmpwkuejx.sHtML

[R11] case 多分支
来源：http://m.share.epnwcf.com/Article/details/gytgdyaac.sHtML

case "$1" in
来源：http://wap.sjlbkw.cn/Article/details/gkommxuzk.sHtML

start) echo "启动" ;;
来源：http://www.m.share.bbcook.cn/Article/details/gcdgztdsb.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.tarul.cn/Article/details/gorvordsd.sHtML

*)     echo "未知命令" ;;
来源：http://blog.sjlbkw.cn/Article/details/gbdoxinyq.sHtML

esac
来源：http://wap.fktsv.cn/Article/details/gslzlpeji.sHtML

[R12] for 遍历文件
来源：http://www.share.yfazqb.com/Article/details/gmiraxmnt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.epnwcf.com/Article/details/geuzovxoc.sHtML

[R13] for 计数循环
来源：http://mobile.fktsv.cn/Article/details/ghqqsnmyi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.tarul.cn/Article/details/gyqxjvtvy.sHtML

[R14] C 风格 for
来源：http://mobile.tarul.cn/Article/details/glghbrvvx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.tarul.cn/Article/details/gjdrirvft.sHtML

[R15] while 逐行读文件
来源：http://baike.fktsv.cn/Article/details/gcghbqnvo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.vehdjk.com/Article/details/gjyklwrox.sHtML

[R16] until 等待条件
来源：http://www.m.share.yfazqb.com/Article/details/gscmbstvj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.yfazqb.com/Article/details/gvpyurqhs.sHtML

[R17] 数组定义与取值
来源：http://3g.vehdjk.com/Article/details/gnbdpkuqa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fktsv.cn/Article/details/gohyqfgsq.sHtML

[R18] 遍历数组
来源：http://www.share.fktsv.cn/Article/details/gvdxvywgf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.yfazqb.com/Article/details/grbuswlze.sHtML

[R19] 数组长度
来源：http://blog.fktsv.cn/Article/details/gnypghyqw.sHtML

echo "${#arr[@]}"
来源：http://wap.bbcook.cn/Article/details/gqvjpigqa.sHtML

[R20] 关联数组（字典）
来源：http://read.share.bbcook.cn/Article/details/gekfqknua.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.yfazqb.com/Article/details/gfijozjkr.sHtML

[R21] 字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/ghbwmuial.sHtML

echo "${#s}"
来源：http://baike.tarul.cn/Article/details/gvrsjohgi.sHtML

[R22] 截取子串
来源：http://read.share.fktsv.cn/Article/details/gukqvucyi.sHtML

echo "${s:0:5}"
来源：http://blog.vehdjk.com/Article/details/gwdxlgpsr.sHtML

[R23] 字符串替换
来源：http://www.blog.epnwcf.com/Article/details/glewqyyss.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fktsv.cn/Article/details/gtivewjju.sHtML

[R24] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/gimzezhdq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.vehdjk.com/Article/details/ggzcfjzvl.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.sjlbkw.cn/Article/details/gkyqrhqcv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.yfazqb.com/Article/details/gmxwhrnie.sHtML

[R26] 命令替换
来源：http://www.share.fktsv.cn/Article/details/gdtlomdjy.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.yfazqb.com/Article/details/gmxcekjcx.sHtML

[R27] 算术展开
来源：http://read.share.fktsv.cn/Article/details/grihkxddb.sHtML

echo $((1 + 2 * 3))
来源：http://blog.bbcook.cn/Article/details/gvsuhbult.sHtML

[R28] 浮点运算
来源：http://3g.sjlbkw.cn/Article/details/gxkdcdoca.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.tarul.cn/Article/details/gcxtalycb.sHtML

[R29] 定义函数
来源：http://wap.vehdjk.com/Article/details/gjvdvvpga.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.bbcook.cn/Article/details/gkxtnwjsz.sHtML

[R30] 函数返回状态码
来源：http://blog.bbcook.cn/Article/details/gownwllnz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fktsv.cn/Article/details/geeoutnjo.sHtML

[R31] 局部变量
来源：http://blog.tarul.cn/Article/details/gsdkgxtjv.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.yfazqb.com/Article/details/gfmsjyhnr.sHtML

[R32] 参数个数校验
来源：http://wap.sjlbkw.cn/Article/details/gsvwsloxr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.bbcook.cn/Article/details/gwowunyst.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.epnwcf.com/Article/details/gcjnhxqle.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.bbcook.cn/Article/details/ggkyscfej.sHtML

[R34] 退出时清理
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmqufwpq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fktsv.cn/Article/details/gnohfuiiv.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fktsv.cn/Article/details/gkotfuzgp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.tarul.cn/Article/details/garxxwacf.sHtML

[R36] 并发执行多个任务
来源：http://www.share.sjlbkw.cn/Article/details/gplzikhmd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.bbcook.cn/Article/details/guljmcdfa.sHtML

[R37] 把输出赋给变量
来源：http://www.share.yfazqb.com/Article/details/gapagrnas.sHtML

files=$(ls -1)
来源：http://blog.fktsv.cn/Article/details/gfgqlzrxq.sHtML

[R38] 管道串联
来源：http://blog.fktsv.cn/Article/details/gvovbzncs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fktsv.cn/Article/details/gcwxqdkbe.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.vehdjk.com/Article/details/geztcjcrk.sHtML

cmd > out.log 2>&1
来源：http://mobile.sjlbkw.cn/Article/details/grfgbnnbg.sHtML

[R40] 追加写日志
来源：http://www.m.share.bbcook.cn/Article/details/gtlpbhhcd.sHtML

echo "log" >> out.log
来源：http://www.blog.bbcook.cn/Article/details/grkoomkqs.sHtML

[R41] 丢弃输出
来源：http://baike.bbcook.cn/Article/details/gsfdiphzk.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fktsv.cn/Article/details/gnqebbpui.sHtML

[R42] 输入重定向
来源：http://mobile.bbcook.cn/Article/details/gvaiejepd.sHtML

wc -l < a.txt
来源：http://www.m.share.epnwcf.com/Article/details/grjyrbsut.sHtML

[R43] 按名字查找文件
来源：http://read.share.epnwcf.com/Article/details/grebttmxx.sHtML


<!-- 参考信息 -->