代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.bbcook.cn/Article/details/gigdpoiny.sHtML

);
来源：http://mobile.sjlbkw.cn/Article/details/gmjthfmjk.sHtML

[Q02] 创建带外键的表
来源：http://read.share.tarul.cn/Article/details/glvmogtzx.sHtML

CREATE TABLE orders (
来源：http://www.blog.tarul.cn/Article/details/gxgagltto.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/gllvnviwm.sHtML

user_id INT NOT NULL,
来源：http://www.share.vehdjk.com/Article/details/gtykojnew.sHtML

amount DECIMAL(10, 2),
来源：http://3g.tarul.cn/Article/details/guwnrdyrg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fktsv.cn/Article/details/gdmcfxdyy.sHtML

);
来源：http://www.blog.vehdjk.com/Article/details/gukonupzu.sHtML

[Q03] 增加列
来源：http://read.share.fktsv.cn/Article/details/ggliogdin.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.sjlbkw.cn/Article/details/guxozkohc.sHtML

[Q04] 修改列类型
来源：http://3g.epnwcf.com/Article/details/gndzbrjja.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.epnwcf.com/Article/details/gtbdirxvj.sHtML

[Q05] 重命名列
来源：http://wap.epnwcf.com/Article/details/gbddiqhlx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.vehdjk.com/Article/details/gmshdwzye.sHtML

[Q06] 删除列
来源：http://mobile.vehdjk.com/Article/details/gyexrtiwl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.tarul.cn/Article/details/gjvcabjoa.sHtML

[Q07] 删除表
来源：http://read.share.bbcook.cn/Article/details/ggzgylkev.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.vehdjk.com/Article/details/gjebdbjtd.sHtML

[Q08] 创建普通索引
来源：http://mobile.sjlbkw.cn/Article/details/ggecljslj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.epnwcf.com/Article/details/gewksjjus.sHtML

[Q09] 创建唯一索引
来源：http://read.share.vehdjk.com/Article/details/gmadtcfyv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.bbcook.cn/Article/details/gqzabbocr.sHtML

[Q10] 插入单行
来源：http://3g.tarul.cn/Article/details/gxjqhppma.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fktsv.cn/Article/details/gpejqyulj.sHtML

[Q11] 一次插入多行
来源：http://read.share.bbcook.cn/Article/details/gihhwqbcz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.bbcook.cn/Article/details/gubuhpluo.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fktsv.cn/Article/details/ghwhslypf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.bbcook.cn/Article/details/gbudpjqvd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fktsv.cn/Article/details/gvtidpbnt.sHtML

[Q13] 忽略重复插入
来源：http://www.share.bbcook.cn/Article/details/gqcbwuvbb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gyueohfql.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.bbcook.cn/Article/details/gbrojjpkd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.epnwcf.com/Article/details/gradwaboj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.yfazqb.com/Article/details/gjmcpmerc.sHtML

[Q15] 查询全部
来源：http://baike.yfazqb.com/Article/details/gvrrzltin.sHtML

SELECT * FROM users;
来源：http://mobile.fktsv.cn/Article/details/gdyxqdabu.sHtML

[Q16] 查询指定列
来源：http://read.share.epnwcf.com/Article/details/gswnwrfuo.sHtML

SELECT id, name FROM users;
来源：http://mobile.fktsv.cn/Article/details/gcmfbvrbv.sHtML

[Q17] 条件查询
来源：http://baike.sjlbkw.cn/Article/details/gqtarteen.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.yfazqb.com/Article/details/gxdicfxrw.sHtML

[Q18] 模糊匹配
来源：http://www.share.yfazqb.com/Article/details/gixgyhmlx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.sjlbkw.cn/Article/details/gfkoibumg.sHtML

[Q19] 范围查询
来源：http://www.m.share.epnwcf.com/Article/details/gkgycjnoq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.epnwcf.com/Article/details/gjbxlwpxq.sHtML

[Q20] IN 列表
来源：http://read.share.sjlbkw.cn/Article/details/gnzwaokgy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.vehdjk.com/Article/details/gfyrqekti.sHtML

[Q21] 空值判断
来源：http://3g.yfazqb.com/Article/details/gnngfllds.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdxdrvma.sHtML

[Q22] 排序
来源：http://baike.bbcook.cn/Article/details/grjtcaynp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.yfazqb.com/Article/details/gptbedihb.sHtML

[Q23] 分页
来源：http://baike.yfazqb.com/Article/details/gdlbfpnnz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.sjlbkw.cn/Article/details/gesognuqk.sHtML

[Q24] 去重
来源：http://m.share.vehdjk.com/Article/details/gwxxchqcc.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.vehdjk.com/Article/details/grudiueju.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.yfazqb.com/Article/details/gjbxsppni.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.sjlbkw.cn/Article/details/glpgleyir.sHtML

[Q26] 计数
来源：http://wap.yfazqb.com/Article/details/gaapnagma.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.epnwcf.com/Article/details/ginkgxbzf.sHtML

[Q27] 条件计数
来源：http://read.share.vehdjk.com/Article/details/goqwsrjcl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.bbcook.cn/Article/details/gvepxvlpc.sHtML

[Q28] 求和与平均
来源：http://wap.tarul.cn/Article/details/gbtmrrybo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.bbcook.cn/Article/details/gkisfnixs.sHtML

[Q29] 最大最小值
来源：http://blog.fktsv.cn/Article/details/gcnlvtaru.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.tarul.cn/Article/details/gsxwjwqed.sHtML

[Q30] 分组统计
来源：http://wap.epnwcf.com/Article/details/gmqfkufri.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gakvomqmk.sHtML

[Q31] 分组后过滤
来源：http://blog.fktsv.cn/Article/details/gfjmqmvbr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.bbcook.cn/Article/details/ghpppimaz.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fktsv.cn/Article/details/gbnumcsue.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.epnwcf.com/Article/details/gjcllezzo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.bbcook.cn/Article/details/gfkkiobtl.sHtML

[Q33] 多列分组
来源：http://blog.tarul.cn/Article/details/gthritdhg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.bbcook.cn/Article/details/gdiirdgvh.sHtML

[Q34] 每组取第一条
来源：http://www.share.tarul.cn/Article/details/gewgmffay.sHtML

SELECT * FROM (
来源：http://baike.epnwcf.com/Article/details/gtqnbzrym.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.epnwcf.com/Article/details/grybzhpcb.sHtML

) t WHERE rn = 1;
来源：http://read.share.bbcook.cn/Article/details/gojkhoxse.sHtML

[Q35] 内连接
来源：http://mobile.epnwcf.com/Article/details/gsjrsiwqs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.yfazqb.com/Article/details/grokkqwer.sHtML

[Q36] 左连接
来源：http://www.share.sjlbkw.cn/Article/details/gzbytogbk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fktsv.cn/Article/details/gouaokben.sHtML

[Q37] 右连接
来源：http://blog.fktsv.cn/Article/details/gsyvpocsa.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.bbcook.cn/Article/details/gvvlsdhxx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.epnwcf.com/Article/details/gbnegtlsx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.tarul.cn/Article/details/gmzxtvgfq.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.sjlbkw.cn/Article/details/gdvzzarvv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.vehdjk.com/Article/details/gbpqnncwn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fktsv.cn/Article/details/gylhkfdei.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.tarul.cn/Article/details/gdwlmdzzs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.epnwcf.com/Article/details/gvwwdokfq.sHtML

[Q41] 多表连接
来源：http://wap.yfazqb.com/Article/details/gropgdsmv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fktsv.cn/Article/details/gxqzxqsyn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fktsv.cn/Article/details/gppxjznff.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.yfazqb.com/Article/details/gytjvuqsh.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.yfazqb.com/Article/details/gkaqgvhom.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fktsv.cn/Article/details/ggxtdbuhj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.yfazqb.com/Article/details/gdgiswtzw.sHtML

[Q43] 标量子查询
来源：http://wap.sjlbkw.cn/Article/details/gbwnyqnzp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.epnwcf.com/Article/details/gcezintcg.sHtML

[Q44] IN 子查询
来源：http://read.share.yfazqb.com/Article/details/gjvedffwo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fktsv.cn/Article/details/gaznafiwd.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.vehdjk.com/Article/details/gptxisgoi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/geiquxkvx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.tarul.cn/Article/details/gvzeaupob.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.bbcook.cn/Article/details/gqyihzusd.sHtML

[Q47] 与平均值比较
来源：http://baike.vehdjk.com/Article/details/gknotuunw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.yfazqb.com/Article/details/guoidbwem.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.epnwcf.com/Article/details/gvaogoogl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.vehdjk.com/Article/details/gbjmodzms.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.vehdjk.com/Article/details/gckhhnkwp.sHtML

[Q49] 更新单行
来源：http://baike.bbcook.cn/Article/details/gznztzejm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.epnwcf.com/Article/details/gqrrcctbd.sHtML

[Q50] 批量更新
来源：http://3g.epnwcf.com/Article/details/gdcevlfrq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.epnwcf.com/Article/details/gefnklhfb.sHtML

[Q51] 用子查询更新
来源：http://3g.epnwcf.com/Article/details/gdsrwmmxw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fktsv.cn/Article/details/geddwesgr.sHtML

[Q52] 删除指定行
来源：http://wap.bbcook.cn/Article/details/gygtoolgy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.tarul.cn/Article/details/gilnwxegh.sHtML

[Q53] 按条件删除
来源：http://wap.sjlbkw.cn/Article/details/gcuyiypue.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.vehdjk.com/Article/details/gwumwqdrh.sHtML

[Q54] 清空表
来源：http://www.m.share.vehdjk.com/Article/details/gbgqrziyd.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.sjlbkw.cn/Article/details/gpgvdrvgv.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.bbcook.cn/Article/details/gmvkqcrzj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.tarul.cn/Article/details/goaddfctv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.sjlbkw.cn/Article/details/gpjaprmbr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.yfazqb.com/Article/details/gpfgknqyx.sHtML

[Q57] 行号
来源：http://www.blog.bbcook.cn/Article/details/giwtacfup.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.yfazqb.com/Article/details/gyqemmrpm.sHtML

[Q58] 累计求和
来源：http://www.m.share.fktsv.cn/Article/details/gnuufvcjd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.vehdjk.com/Article/details/gfyanctgt.sHtML

[Q59] 分组内累计
来源：http://blog.tarul.cn/Article/details/gmddptrxe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gskmvxack.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.vehdjk.com/Article/details/guebeuciy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fktsv.cn/Article/details/gtpiniqpz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.tarul.cn/Article/details/gbvyanvkc.sHtML

[Q61] 移动平均
来源：http://www.blog.tarul.cn/Article/details/gfyjjnnov.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gfpxzmsdt.sHtML

[Q62] 分组占比
来源：http://blog.bbcook.cn/Article/details/gxcysdvuk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/grbtmrlmy.sHtML

[Q63] 开启事务
来源：http://mobile.tarul.cn/Article/details/gtqjfhssm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fktsv.cn/Article/details/gqtuyuoun.sHtML

[Q64] 提交事务
来源：http://m.share.tarul.cn/Article/details/gfjoycmin.sHtML

COMMIT;
来源：http://mobile.sjlbkw.cn/Article/details/gkcitswsg.sHtML

[Q65] 回滚事务
来源：http://wap.bbcook.cn/Article/details/graouudxz.sHtML

ROLLBACK;
来源：http://www.m.share.fktsv.cn/Article/details/gdaxaukyx.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fktsv.cn/Article/details/gbhgvpaha.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.yfazqb.com/Article/details/gvrkhxoxx.sHtML

[Q67] 设置隔离级别
来源：http://blog.fktsv.cn/Article/details/gnxwpyvmq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.sjlbkw.cn/Article/details/gzwwdrmal.sHtML

[Q68] 保存点
来源：http://www.blog.vehdjk.com/Article/details/gtajbezkn.sHtML

SAVEPOINT sp1;
来源：http://m.share.tarul.cn/Article/details/gvceecorj.sHtML

ROLLBACK TO sp1;
来源：http://m.share.vehdjk.com/Article/details/glaodoovy.sHtML

[Q69] 查看执行计划
来源：http://m.share.yfazqb.com/Article/details/gfegstxhe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fktsv.cn/Article/details/glmsufagq.sHtML

[Q70] 更新统计信息
来源：http://www.share.vehdjk.com/Article/details/grjxwwxba.sHtML

ANALYZE TABLE users;
来源：http://blog.yfazqb.com/Article/details/gdixfkqul.sHtML

[Q71] 查看建表语句
来源：http://wap.tarul.cn/Article/details/gryzlznzj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.sjlbkw.cn/Article/details/gglrjihfl.sHtML

[Q72] 查看索引
来源：http://blog.yfazqb.com/Article/details/gxoqodffj.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fktsv.cn/Article/details/gdconkcme.sHtML

[Q73] 查看表状态
来源：http://blog.epnwcf.com/Article/details/glrnojlyn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.sjlbkw.cn/Article/details/glnqnmwue.sHtML

[Q74] 强制使用索引
来源：http://www.blog.vehdjk.com/Article/details/gmvafbqlu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.yfazqb.com/Article/details/gzwbatlur.sHtML

[Q75] 日期格式化
来源：http://m.share.sjlbkw.cn/Article/details/gbdhuklpx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhrckdkr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.epnwcf.com/Article/details/giomtrzav.sHtML

[Q76] 按天统计
来源：http://www.m.share.tarul.cn/Article/details/geptxkdwm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.yfazqb.com/Article/details/gtkdibvyi.sHtML

[Q77] 时间加减
来源：http://wap.epnwcf.com/Article/details/gqndynimw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.sjlbkw.cn/Article/details/gohnqaqnb.sHtML

[Q78] 当前时间
来源：http://www.blog.tarul.cn/Article/details/gzypvpojg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.vehdjk.com/Article/details/gadlucuau.sHtML

[Q79] 字符串拼接
来源：http://www.share.epnwcf.com/Article/details/guvbmjvcd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.vehdjk.com/Article/details/gbefyqwvy.sHtML

[Q80] 字符串截取
来源：http://www.m.share.yfazqb.com/Article/details/gjgcjlrpu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.yfazqb.com/Article/details/gcxlxaoyc.sHtML

[Q81] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/gmlhzhhuc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.epnwcf.com/Article/details/gwwvfxvpb.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fktsv.cn/Article/details/gpefhoeuc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gacmaizkf.sHtML

[Q83] 大小写转换
来源：http://m.share.vehdjk.com/Article/details/gunqewqqw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gwvkpsvjz.sHtML

[Q84] 去除首尾空格
来源：http://mobile.vehdjk.com/Article/details/gkhaicusm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gzjkinnhz.sHtML

[Q85] 数值取整
来源：http://read.share.vehdjk.com/Article/details/gcfyhffjv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fktsv.cn/Article/details/gqpwjgqnj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.bbcook.cn/Article/details/gvjxjxilw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.tarul.cn/Article/details/gnsnctdwh.sHtML

[Q87] JSON 字段做条件
来源：http://blog.bbcook.cn/Article/details/genuptgud.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.tarul.cn/Article/details/ggnkgdjfx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.vehdjk.com/Article/details/gpmfufhzx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.epnwcf.com/Article/details/gcbkognhl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/ghrwhemdr.sHtML

[Q89] 判断表是否存在
来源：http://www.share.epnwcf.com/Article/details/gphdivbqr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.vehdjk.com/Article/details/gxhxiklty.sHtML

[Q90] 生成序号列
来源：http://www.blog.bbcook.cn/Article/details/gybomafzq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.sjlbkw.cn/Article/details/gctxconnl.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gpvxvdjcu.sHtML

R. Bash 专题
来源：http://m.share.tarul.cn/Article/details/ghlnxobnw.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gotrronkr.sHtML

[R01] shebang 与严格模式
来源：http://baike.epnwcf.com/Article/details/gzexdxkin.sHtML

#!/usr/bin/env bash
来源：http://www.share.tarul.cn/Article/details/gvyqkktqt.sHtML

set -euo pipefail
来源：http://wap.epnwcf.com/Article/details/gqqqyjuxj.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fktsv.cn/Article/details/gevzvfefk.sHtML

name="Tom"; echo "$name"
来源：http://wap.tarul.cn/Article/details/gnpncyhjw.sHtML

[R03] 只读变量
来源：http://baike.tarul.cn/Article/details/gkpboiitp.sHtML

readonly PI=3.14
来源：http://baike.vehdjk.com/Article/details/gqewzxhcm.sHtML

[R04] 位置参数
来源：http://wap.epnwcf.com/Article/details/ggnauiitq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.vehdjk.com/Article/details/gpqozvidc.sHtML

[R05] 参数默认值
来源：http://www.share.tarul.cn/Article/details/gxnfpqukr.sHtML

name="${1:-default}"
来源：http://3g.sjlbkw.cn/Article/details/gwntjqeap.sHtML

[R06] 判断命令是否存在
来源：http://blog.epnwcf.com/Article/details/gjyctsxwh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fktsv.cn/Article/details/gyjbaxmrm.sHtML

[R07] if 判断文件
来源：http://www.blog.bbcook.cn/Article/details/gyiexpkex.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.vehdjk.com/Article/details/guiceuzjq.sHtML

[R08] 数值比较
来源：http://baike.bbcook.cn/Article/details/gzybwqrzn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.tarul.cn/Article/details/gzkovujjy.sHtML

[R09] 字符串比较
来源：http://baike.fktsv.cn/Article/details/gcqneubcw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.tarul.cn/Article/details/gwhqbnogb.sHtML

[R10] 正则匹配
来源：http://blog.yfazqb.com/Article/details/gexufutla.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.epnwcf.com/Article/details/giydusptw.sHtML

[R11] case 多分支
来源：http://3g.yfazqb.com/Article/details/ghbhhmdjk.sHtML

case "$1" in
来源：http://mobile.tarul.cn/Article/details/gdxqeknaz.sHtML

start) echo "启动" ;;
来源：http://wap.sjlbkw.cn/Article/details/gbhnlwwql.sHtML

stop)  echo "停止" ;;
来源：http://wap.bbcook.cn/Article/details/gsukblctj.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fktsv.cn/Article/details/gwxrorfgc.sHtML

esac
来源：http://mobile.vehdjk.com/Article/details/ghxtqkkuh.sHtML

[R12] for 遍历文件
来源：http://www.share.fktsv.cn/Article/details/gnjtwygtp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.tarul.cn/Article/details/gzashjgvq.sHtML

[R13] for 计数循环
来源：http://www.m.share.fktsv.cn/Article/details/gpzytruar.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.epnwcf.com/Article/details/gszzouvss.sHtML

[R14] C 风格 for
来源：http://blog.tarul.cn/Article/details/gjulzfbti.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gfegzbvml.sHtML

[R15] while 逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gikznbnct.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.vehdjk.com/Article/details/gbimthalc.sHtML

[R16] until 等待条件
来源：http://3g.tarul.cn/Article/details/gkyyrngex.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gtjqdieoa.sHtML

[R17] 数组定义与取值
来源：http://3g.tarul.cn/Article/details/gcomgizbu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.sjlbkw.cn/Article/details/gqhtxvoee.sHtML

[R18] 遍历数组
来源：http://mobile.tarul.cn/Article/details/grfkxzxim.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.yfazqb.com/Article/details/grkfdzefs.sHtML

[R19] 数组长度
来源：http://3g.fktsv.cn/Article/details/gtvcljrjv.sHtML

echo "${#arr[@]}"
来源：http://3g.fktsv.cn/Article/details/gkbyvkzow.sHtML

[R20] 关联数组（字典）
来源：http://www.share.vehdjk.com/Article/details/gllxyzxth.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.vehdjk.com/Article/details/gojxdhupw.sHtML

[R21] 字符串长度
来源：http://mobile.yfazqb.com/Article/details/grczntehk.sHtML

echo "${#s}"
来源：http://www.blog.epnwcf.com/Article/details/gtrtnzkml.sHtML

[R22] 截取子串
来源：http://read.share.yfazqb.com/Article/details/gqybgyulq.sHtML

echo "${s:0:5}"
来源：http://read.share.yfazqb.com/Article/details/ghfjjhrhf.sHtML

[R23] 字符串替换
来源：http://www.share.sjlbkw.cn/Article/details/ghbqbpcjg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.yfazqb.com/Article/details/gzybemose.sHtML

[R24] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/gfrpuagta.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.epnwcf.com/Article/details/gfxvrtdxf.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.vehdjk.com/Article/details/gyzonpsos.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.yfazqb.com/Article/details/gnwnszpqo.sHtML

[R26] 命令替换
来源：http://read.share.fktsv.cn/Article/details/gyhyejizt.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.yfazqb.com/Article/details/gwssofyxg.sHtML

[R27] 算术展开
来源：http://read.share.fktsv.cn/Article/details/ganuqcdyn.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.yfazqb.com/Article/details/gdghlikps.sHtML

[R28] 浮点运算
来源：http://www.m.share.yfazqb.com/Article/details/givsjhnbo.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.sjlbkw.cn/Article/details/gszntrefr.sHtML

[R29] 定义函数
来源：http://read.share.fktsv.cn/Article/details/gqcroslrt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fktsv.cn/Article/details/gsdzphmra.sHtML

[R30] 函数返回状态码
来源：http://read.share.fktsv.cn/Article/details/gppaugjkz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.vehdjk.com/Article/details/gdetfsbdg.sHtML

[R31] 局部变量
来源：http://m.share.epnwcf.com/Article/details/gycbyiolk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.vehdjk.com/Article/details/gkoitzaiw.sHtML

[R32] 参数个数校验
来源：http://blog.epnwcf.com/Article/details/grhozupha.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gplftjqny.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.tarul.cn/Article/details/gcazvfozh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.yfazqb.com/Article/details/gblzqvtif.sHtML

[R34] 退出时清理
来源：http://mobile.tarul.cn/Article/details/gjhvtjwrp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/grsqkznrz.sHtML

[R35] 后台执行并等待
来源：http://wap.fktsv.cn/Article/details/geqisohle.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.vehdjk.com/Article/details/guzspsydk.sHtML

[R36] 并发执行多个任务
来源：http://www.share.vehdjk.com/Article/details/garmzylxq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.epnwcf.com/Article/details/gcwvuimwb.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.tarul.cn/Article/details/gcumyyiud.sHtML

files=$(ls -1)
来源：http://www.share.epnwcf.com/Article/details/gdijcdthb.sHtML

[R38] 管道串联
来源：http://www.share.vehdjk.com/Article/details/gguiugrie.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.sjlbkw.cn/Article/details/gsbzralwa.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.epnwcf.com/Article/details/glzruaynt.sHtML

cmd > out.log 2>&1
来源：http://3g.yfazqb.com/Article/details/gwplbkbqe.sHtML

[R40] 追加写日志
来源：http://3g.epnwcf.com/Article/details/gocnzguyd.sHtML

echo "log" >> out.log
来源：http://read.share.vehdjk.com/Article/details/gngxgswan.sHtML

[R41] 丢弃输出
来源：http://wap.sjlbkw.cn/Article/details/gbeaacpgz.sHtML

cmd >/dev/null 2>&1
来源：http://baike.vehdjk.com/Article/details/gqtkfyufn.sHtML

[R42] 输入重定向
来源：http://3g.sjlbkw.cn/Article/details/ghhlpqkkg.sHtML

wc -l < a.txt
来源：http://mobile.sjlbkw.cn/Article/details/grauuabqb.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.tarul.cn/Article/details/gnzfgnuhd.sHtML

find . -name "*.log" -type f
来源：http://mobile.tarul.cn/Article/details/gllcnlrud.sHtML

[R44] 按修改时间查找
来源：http://www.share.bbcook.cn/Article/details/gebwkhdre.sHtML

find . -mtime -7 -type f
来源：http://blog.bbcook.cn/Article/details/gsoruraxj.sHtML

[R45] 批量删除
来源：http://www.blog.epnwcf.com/Article/details/gzywhwnen.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.vehdjk.com/Article/details/galjusgvr.sHtML

[R46] 递归替换文件内容
来源：http://baike.tarul.cn/Article/details/groisaogl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fktsv.cn/Article/details/gmorcoval.sHtML

[R47] sed 单行替换
来源：http://wap.yfazqb.com/Article/details/gprvkrege.sHtML


<!-- 参考信息 -->