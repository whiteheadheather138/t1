代发 wailian999

================================================================================
来源：http://blog.vehdjk.com/Article/details/ggqeochej.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fktsv.cn/Article/details/gxzugapkm.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gklzrmhnl.sHtML

[Q01] 创建表
来源：http://wap.tarul.cn/Article/details/ggdmnydrk.sHtML

CREATE TABLE users (
来源：http://3g.tarul.cn/Article/details/gqevrulxq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fktsv.cn/Article/details/gsuvoyfek.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.epnwcf.com/Article/details/gbxjelpji.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.sjlbkw.cn/Article/details/gmemhhmyy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.yfazqb.com/Article/details/gozrxasjs.sHtML

);
来源：http://www.m.share.epnwcf.com/Article/details/gmsxbpsnc.sHtML

[Q02] 创建带外键的表
来源：http://read.share.yfazqb.com/Article/details/gmkvhuhun.sHtML

CREATE TABLE orders (
来源：http://www.share.tarul.cn/Article/details/gjddjznan.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fktsv.cn/Article/details/gbykdyrmd.sHtML

user_id INT NOT NULL,
来源：http://blog.tarul.cn/Article/details/gusltlyjj.sHtML

amount DECIMAL(10, 2),
来源：http://3g.bbcook.cn/Article/details/gigkwkdkx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.vehdjk.com/Article/details/gzngnixug.sHtML

);
来源：http://read.share.bbcook.cn/Article/details/gunrzfvim.sHtML

[Q03] 增加列
来源：http://www.m.share.tarul.cn/Article/details/gzxgsbwkt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.bbcook.cn/Article/details/gcryuujih.sHtML

[Q04] 修改列类型
来源：http://blog.bbcook.cn/Article/details/gzpqwptwj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.tarul.cn/Article/details/gqncbawsz.sHtML

[Q05] 重命名列
来源：http://blog.sjlbkw.cn/Article/details/glfzpnhev.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fktsv.cn/Article/details/gyfhfwlcs.sHtML

[Q06] 删除列
来源：http://www.m.share.fktsv.cn/Article/details/gqbdhthlu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fktsv.cn/Article/details/gdezllsap.sHtML

[Q07] 删除表
来源：http://read.share.sjlbkw.cn/Article/details/grgunzozn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.bbcook.cn/Article/details/gbsrvjsuk.sHtML

[Q08] 创建普通索引
来源：http://mobile.sjlbkw.cn/Article/details/gmdtmxmum.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.epnwcf.com/Article/details/gngwlvjms.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.bbcook.cn/Article/details/geayhwhfr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.yfazqb.com/Article/details/glyyoekks.sHtML

[Q10] 插入单行
来源：http://mobile.fktsv.cn/Article/details/gncikixdy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gwpyorclh.sHtML

[Q11] 一次插入多行
来源：http://www.blog.vehdjk.com/Article/details/gsusextsk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.vehdjk.com/Article/details/gvyblhbyq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fktsv.cn/Article/details/gfptvpqhs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fktsv.cn/Article/details/gaaioepcz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fktsv.cn/Article/details/gejibqvnm.sHtML

[Q13] 忽略重复插入
来源：http://baike.yfazqb.com/Article/details/ghzeykkhd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.bbcook.cn/Article/details/goiuovivv.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fktsv.cn/Article/details/gshnvdnzn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fktsv.cn/Article/details/gglqqyelt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.epnwcf.com/Article/details/gxpqzoshg.sHtML

[Q15] 查询全部
来源：http://blog.yfazqb.com/Article/details/gbnxfhaib.sHtML

SELECT * FROM users;
来源：http://mobile.vehdjk.com/Article/details/ghncissrb.sHtML

[Q16] 查询指定列
来源：http://baike.epnwcf.com/Article/details/ghcvyigrj.sHtML

SELECT id, name FROM users;
来源：http://mobile.yfazqb.com/Article/details/gqtyzvfvv.sHtML

[Q17] 条件查询
来源：http://www.m.share.epnwcf.com/Article/details/geycowvaq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.sjlbkw.cn/Article/details/giivtksqt.sHtML

[Q18] 模糊匹配
来源：http://www.share.tarul.cn/Article/details/gvljdznwy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.epnwcf.com/Article/details/gptlscodc.sHtML

[Q19] 范围查询
来源：http://baike.tarul.cn/Article/details/gscnwuhjh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.bbcook.cn/Article/details/ghorlbjfr.sHtML

[Q20] IN 列表
来源：http://read.share.sjlbkw.cn/Article/details/gcejlzust.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.tarul.cn/Article/details/gpvunzxrs.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/genfsoyiq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.bbcook.cn/Article/details/gcfrvhdiy.sHtML

[Q22] 排序
来源：http://m.share.bbcook.cn/Article/details/gapsuwrxr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.bbcook.cn/Article/details/ghfsarhrg.sHtML

[Q23] 分页
来源：http://www.blog.yfazqb.com/Article/details/gbapupeib.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.vehdjk.com/Article/details/gfdxhbtra.sHtML

[Q24] 去重
来源：http://www.m.share.tarul.cn/Article/details/gnnqdhmbn.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.tarul.cn/Article/details/gjzehxthe.sHtML

[Q25] 只取前 N 条
来源：http://3g.sjlbkw.cn/Article/details/gsdgrfztg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.yfazqb.com/Article/details/giixldujm.sHtML

[Q26] 计数
来源：http://baike.tarul.cn/Article/details/gzohshxof.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.tarul.cn/Article/details/gttywhgiy.sHtML

[Q27] 条件计数
来源：http://www.m.share.yfazqb.com/Article/details/gqmbftehf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.yfazqb.com/Article/details/gzycxynpr.sHtML

[Q28] 求和与平均
来源：http://3g.bbcook.cn/Article/details/gfyipssmu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gdvrrkhag.sHtML

[Q29] 最大最小值
来源：http://blog.sjlbkw.cn/Article/details/gpnesdqwp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fktsv.cn/Article/details/gozqlgmlo.sHtML

[Q30] 分组统计
来源：http://www.m.share.vehdjk.com/Article/details/gjwbyenrd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/geyqdxqef.sHtML

[Q31] 分组后过滤
来源：http://blog.tarul.cn/Article/details/gmolzhduh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fktsv.cn/Article/details/ggpiwialc.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/gfrtgyofj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gqxiucvzm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fktsv.cn/Article/details/gyqkztliu.sHtML

[Q33] 多列分组
来源：http://blog.epnwcf.com/Article/details/gdjertaer.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.sjlbkw.cn/Article/details/gmzwoyzid.sHtML

[Q34] 每组取第一条
来源：http://3g.epnwcf.com/Article/details/grzsddwap.sHtML

SELECT * FROM (
来源：http://wap.fktsv.cn/Article/details/glbhyhsos.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.epnwcf.com/Article/details/gstzflbnu.sHtML

) t WHERE rn = 1;
来源：http://read.share.tarul.cn/Article/details/gvvvamjce.sHtML

[Q35] 内连接
来源：http://www.m.share.tarul.cn/Article/details/gwscmyfct.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fktsv.cn/Article/details/glvwdalom.sHtML

[Q36] 左连接
来源：http://blog.vehdjk.com/Article/details/gxckpvhpz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.yfazqb.com/Article/details/gatqypnnz.sHtML

[Q37] 右连接
来源：http://www.share.bbcook.cn/Article/details/gpdutmhgg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.tarul.cn/Article/details/gwdlkpzex.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.epnwcf.com/Article/details/gdyerjzvr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.yfazqb.com/Article/details/girwxphpe.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.epnwcf.com/Article/details/gxjejedcp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fktsv.cn/Article/details/gzwhinngl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.yfazqb.com/Article/details/gncwwbbmm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.sjlbkw.cn/Article/details/gcaegfrfq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.yfazqb.com/Article/details/gtiyzmaeu.sHtML

[Q41] 多表连接
来源：http://www.share.bbcook.cn/Article/details/gvjssvwqy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.sjlbkw.cn/Article/details/gudpzgqbm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.sjlbkw.cn/Article/details/gpzrzltaf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.tarul.cn/Article/details/gotmdnseo.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fktsv.cn/Article/details/gydcbeqrm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fktsv.cn/Article/details/gidwhxjea.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.tarul.cn/Article/details/ggtbmenve.sHtML

[Q43] 标量子查询
来源：http://www.blog.vehdjk.com/Article/details/groolwqvj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.yfazqb.com/Article/details/gbmrvifnj.sHtML

[Q44] IN 子查询
来源：http://3g.sjlbkw.cn/Article/details/gtoksdhfw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.vehdjk.com/Article/details/gvscdmxab.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.yfazqb.com/Article/details/gjghawlji.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.bbcook.cn/Article/details/gnebqyhix.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.tarul.cn/Article/details/ghppxjgdx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.vehdjk.com/Article/details/ginxzcpwl.sHtML

[Q47] 与平均值比较
来源：http://mobile.sjlbkw.cn/Article/details/gfvjyvzku.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fktsv.cn/Article/details/gekizxrwe.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.tarul.cn/Article/details/gvxlkibyl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fktsv.cn/Article/details/gjpwxbrpq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.vehdjk.com/Article/details/gpxiaobwl.sHtML

[Q49] 更新单行
来源：http://www.blog.vehdjk.com/Article/details/gizarddeb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.tarul.cn/Article/details/gafrhuaqo.sHtML

[Q50] 批量更新
来源：http://read.share.fktsv.cn/Article/details/gdfvhncyl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fktsv.cn/Article/details/ghuzxvhch.sHtML

[Q51] 用子查询更新
来源：http://blog.bbcook.cn/Article/details/gccdxqrwj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.tarul.cn/Article/details/gtmsfarzs.sHtML

[Q52] 删除指定行
来源：http://www.m.share.epnwcf.com/Article/details/gfhokbasf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.bbcook.cn/Article/details/ghdvcnwsu.sHtML

[Q53] 按条件删除
来源：http://blog.tarul.cn/Article/details/gookfrdar.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.tarul.cn/Article/details/guqdngyxc.sHtML

[Q54] 清空表
来源：http://baike.tarul.cn/Article/details/glmamwjtc.sHtML

TRUNCATE TABLE logs;
来源：http://3g.tarul.cn/Article/details/glaeaidfm.sHtML

[Q55] 排名（并列占位）
来源：http://wap.sjlbkw.cn/Article/details/gmmrncqar.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.epnwcf.com/Article/details/gsrrpcbet.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.yfazqb.com/Article/details/gtvmmxqpb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.tarul.cn/Article/details/gnmdhxsis.sHtML

[Q57] 行号
来源：http://www.m.share.yfazqb.com/Article/details/gyfksivwz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.bbcook.cn/Article/details/govjsdsag.sHtML

[Q58] 累计求和
来源：http://m.share.yfazqb.com/Article/details/gqbikjrhe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gjiizrnmc.sHtML

[Q59] 分组内累计
来源：http://wap.fktsv.cn/Article/details/gdwgxpckk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gjmeiogmi.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.tarul.cn/Article/details/grlsnxhua.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.yfazqb.com/Article/details/gjezvmivj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gapdxjydj.sHtML

[Q61] 移动平均
来源：http://wap.vehdjk.com/Article/details/grehhucyn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.vehdjk.com/Article/details/gbxxhkxrk.sHtML

[Q62] 分组占比
来源：http://wap.vehdjk.com/Article/details/gibnnrbmf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gcdzfpnmh.sHtML

[Q63] 开启事务
来源：http://3g.bbcook.cn/Article/details/gltvpunoo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.yfazqb.com/Article/details/goyifkyyg.sHtML

[Q64] 提交事务
来源：http://m.share.fktsv.cn/Article/details/gubpqdfpv.sHtML

COMMIT;
来源：http://m.share.vehdjk.com/Article/details/gddrtxbaw.sHtML

[Q65] 回滚事务
来源：http://www.share.vehdjk.com/Article/details/giylervgx.sHtML

ROLLBACK;
来源：http://blog.bbcook.cn/Article/details/gvfnsogco.sHtML

[Q66] 行锁查询
来源：http://wap.tarul.cn/Article/details/gpbepgfdw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.yfazqb.com/Article/details/gimxtpxji.sHtML

[Q67] 设置隔离级别
来源：http://read.share.vehdjk.com/Article/details/gnkadrbtk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.sjlbkw.cn/Article/details/grlseitkl.sHtML

[Q68] 保存点
来源：http://baike.tarul.cn/Article/details/gdcgodiol.sHtML

SAVEPOINT sp1;
来源：http://read.share.yfazqb.com/Article/details/gqyzuyifh.sHtML

ROLLBACK TO sp1;
来源：http://www.share.epnwcf.com/Article/details/gxktbjcsa.sHtML

[Q69] 查看执行计划
来源：http://3g.tarul.cn/Article/details/gfclxmgtq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.vehdjk.com/Article/details/gjmsrefat.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fktsv.cn/Article/details/gvkvweeag.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fktsv.cn/Article/details/gkuvmqitd.sHtML

[Q71] 查看建表语句
来源：http://baike.sjlbkw.cn/Article/details/gylyewgii.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.vehdjk.com/Article/details/giadrughj.sHtML

[Q72] 查看索引
来源：http://mobile.vehdjk.com/Article/details/gsohmgvzy.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fktsv.cn/Article/details/ghoofttap.sHtML

[Q73] 查看表状态
来源：http://www.share.fktsv.cn/Article/details/glllmkgzh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.vehdjk.com/Article/details/goohboags.sHtML

[Q74] 强制使用索引
来源：http://read.share.yfazqb.com/Article/details/gzzfydgss.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.yfazqb.com/Article/details/gksfxjeqw.sHtML

[Q75] 日期格式化
来源：http://www.m.share.yfazqb.com/Article/details/gnuixjpkw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gpjzuvhyw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.yfazqb.com/Article/details/gnqyxwcph.sHtML

[Q76] 按天统计
来源：http://read.share.bbcook.cn/Article/details/geidilymt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.vehdjk.com/Article/details/guyleowgg.sHtML

[Q77] 时间加减
来源：http://www.m.share.fktsv.cn/Article/details/giynlxgqk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.epnwcf.com/Article/details/gzubdsmuy.sHtML

[Q78] 当前时间
来源：http://3g.epnwcf.com/Article/details/gfinrljfq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.vehdjk.com/Article/details/gbeyzmjrd.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/gzxkfrlml.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.bbcook.cn/Article/details/gxtnbhkwk.sHtML

[Q80] 字符串截取
来源：http://m.share.vehdjk.com/Article/details/gocwmbnzp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.tarul.cn/Article/details/gjlgsmbpi.sHtML

[Q81] 字符串替换
来源：http://m.share.vehdjk.com/Article/details/gbahoztij.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/glgvzrirl.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.bbcook.cn/Article/details/gohbizsbj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gqejhgget.sHtML

[Q83] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gjvcveyad.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gogsprxpw.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.bbcook.cn/Article/details/girrkoiiq.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gizppkair.sHtML

[Q85] 数值取整
来源：http://baike.sjlbkw.cn/Article/details/gqvgzztah.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.epnwcf.com/Article/details/gecthvjyb.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.sjlbkw.cn/Article/details/gcnwsfega.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.yfazqb.com/Article/details/gaumgqfes.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.vehdjk.com/Article/details/gbmuymoyh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.tarul.cn/Article/details/gagpkhvyy.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.epnwcf.com/Article/details/gcfldjrla.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.sjlbkw.cn/Article/details/gonvvmkje.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.epnwcf.com/Article/details/ghtjxrxxp.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fktsv.cn/Article/details/gqyasnboq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.bbcook.cn/Article/details/gjkusjxzp.sHtML

[Q90] 生成序号列
来源：http://wap.sjlbkw.cn/Article/details/gkhkkujyb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.yfazqb.com/Article/details/gpmnozgvt.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gooqrlqav.sHtML

R. Bash 专题
来源：http://read.share.epnwcf.com/Article/details/gdydlvuts.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gwhbgjszj.sHtML

[R01] shebang 与严格模式
来源：http://mobile.tarul.cn/Article/details/gcjuawxio.sHtML

#!/usr/bin/env bash
来源：http://mobile.epnwcf.com/Article/details/glctwywpq.sHtML

set -euo pipefail
来源：http://www.blog.yfazqb.com/Article/details/gywjpgcam.sHtML

[R02] 变量赋值与使用
来源：http://www.share.vehdjk.com/Article/details/gnujjcqux.sHtML

name="Tom"; echo "$name"
来源：http://www.share.bbcook.cn/Article/details/gxgmjczjo.sHtML

[R03] 只读变量
来源：http://www.m.share.fktsv.cn/Article/details/gejvakpvm.sHtML

readonly PI=3.14
来源：http://3g.tarul.cn/Article/details/gljwpdwvh.sHtML

[R04] 位置参数
来源：http://m.share.epnwcf.com/Article/details/gxzuhkhik.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.sjlbkw.cn/Article/details/gtioswvpn.sHtML

[R05] 参数默认值
来源：http://baike.vehdjk.com/Article/details/gpsqymjru.sHtML

name="${1:-default}"
来源：http://mobile.bbcook.cn/Article/details/gmbmktkqi.sHtML

[R06] 判断命令是否存在
来源：http://blog.sjlbkw.cn/Article/details/gcgwqoyeb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.tarul.cn/Article/details/gmcnhuagh.sHtML

[R07] if 判断文件
来源：http://www.blog.epnwcf.com/Article/details/gzggiabeb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.bbcook.cn/Article/details/gmwzclvfa.sHtML

[R08] 数值比较
来源：http://www.share.fktsv.cn/Article/details/gdlffpnyk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.yfazqb.com/Article/details/gojosgczv.sHtML

[R09] 字符串比较
来源：http://read.share.fktsv.cn/Article/details/ggcluhtsf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.epnwcf.com/Article/details/grgrlwodu.sHtML

[R10] 正则匹配
来源：http://m.share.vehdjk.com/Article/details/gddvpswfy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gaocosyuc.sHtML

[R11] case 多分支
来源：http://mobile.epnwcf.com/Article/details/giysyfrik.sHtML

case "$1" in
来源：http://mobile.yfazqb.com/Article/details/ghvahrmff.sHtML

start) echo "启动" ;;
来源：http://wap.tarul.cn/Article/details/gasnpcgjk.sHtML

stop)  echo "停止" ;;
来源：http://blog.fktsv.cn/Article/details/gkfruxzuc.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.vehdjk.com/Article/details/guhkujcdu.sHtML

esac
来源：http://blog.fktsv.cn/Article/details/guibrsouk.sHtML

[R12] for 遍历文件
来源：http://baike.tarul.cn/Article/details/gmxauuyhm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.vehdjk.com/Article/details/gkoxygrnc.sHtML

[R13] for 计数循环
来源：http://3g.fktsv.cn/Article/details/gxcrtkoko.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.bbcook.cn/Article/details/giikogeul.sHtML

[R14] C 风格 for
来源：http://3g.tarul.cn/Article/details/gzbumiscj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/gxpfwmthe.sHtML

[R15] while 逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gocoytaun.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.vehdjk.com/Article/details/gkthdspko.sHtML

[R16] until 等待条件
来源：http://mobile.fktsv.cn/Article/details/ghexhjegs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/gaxmblqrw.sHtML

[R17] 数组定义与取值
来源：http://3g.sjlbkw.cn/Article/details/gmgeawcjl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.sjlbkw.cn/Article/details/gdhovesqn.sHtML

[R18] 遍历数组
来源：http://mobile.fktsv.cn/Article/details/gvzxjjimw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fktsv.cn/Article/details/gmcyjstxu.sHtML

[R19] 数组长度
来源：http://mobile.tarul.cn/Article/details/gryjwmudc.sHtML

echo "${#arr[@]}"
来源：http://baike.sjlbkw.cn/Article/details/gsnywvqra.sHtML

[R20] 关联数组（字典）
来源：http://read.share.tarul.cn/Article/details/gxdspiiqy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gasarlolu.sHtML

[R21] 字符串长度
来源：http://mobile.fktsv.cn/Article/details/ghymcmlol.sHtML

echo "${#s}"
来源：http://m.share.bbcook.cn/Article/details/gnqanhggj.sHtML

[R22] 截取子串
来源：http://mobile.fktsv.cn/Article/details/gwoqclqsj.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fktsv.cn/Article/details/glbucdgcl.sHtML

[R23] 字符串替换
来源：http://3g.epnwcf.com/Article/details/gwctvoycm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.yfazqb.com/Article/details/gslyxzxcy.sHtML

[R24] 大小写转换
来源：http://m.share.sjlbkw.cn/Article/details/gcycqewuf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.tarul.cn/Article/details/gzxjnzhsl.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.yfazqb.com/Article/details/glmyhlfdd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.tarul.cn/Article/details/gyhwanjwo.sHtML

[R26] 命令替换
来源：http://read.share.tarul.cn/Article/details/gyahehlhd.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.tarul.cn/Article/details/goukktajo.sHtML

[R27] 算术展开
来源：http://www.blog.bbcook.cn/Article/details/gqygmklew.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.vehdjk.com/Article/details/gplipyyjy.sHtML

[R28] 浮点运算
来源：http://blog.yfazqb.com/Article/details/gxzgocyfr.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.bbcook.cn/Article/details/glphmojvi.sHtML

[R29] 定义函数
来源：http://baike.bbcook.cn/Article/details/gwqnqprsx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fktsv.cn/Article/details/gamnfmvuc.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgqyqqpq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.yfazqb.com/Article/details/gsgnuwipv.sHtML

[R31] 局部变量
来源：http://read.share.tarul.cn/Article/details/gflkwvwcs.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.tarul.cn/Article/details/gwksthalk.sHtML

[R32] 参数个数校验
来源：http://www.m.share.bbcook.cn/Article/details/gluregilv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.epnwcf.com/Article/details/ghakewhis.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.bbcook.cn/Article/details/gjfoezchm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.yfazqb.com/Article/details/gnthwcobb.sHtML

[R34] 退出时清理
来源：http://3g.epnwcf.com/Article/details/grsmkmdax.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.sjlbkw.cn/Article/details/gfcortgiq.sHtML

[R35] 后台执行并等待
来源：http://blog.epnwcf.com/Article/details/gplnttkxi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.tarul.cn/Article/details/gtnydiojk.sHtML

[R36] 并发执行多个任务
来源：http://mobile.yfazqb.com/Article/details/gjnlbbrfj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.yfazqb.com/Article/details/gaxfjozsu.sHtML

[R37] 把输出赋给变量
来源：http://wap.fktsv.cn/Article/details/giopvdebu.sHtML

files=$(ls -1)
来源：http://www.blog.yfazqb.com/Article/details/gtxvlalfe.sHtML

[R38] 管道串联
来源：http://mobile.epnwcf.com/Article/details/gmffvjidb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.bbcook.cn/Article/details/gamqdtowt.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.sjlbkw.cn/Article/details/gkanbyzfh.sHtML

cmd > out.log 2>&1
来源：http://read.share.vehdjk.com/Article/details/gyadtvmyd.sHtML

[R40] 追加写日志
来源：http://3g.yfazqb.com/Article/details/grxwnnfhu.sHtML

echo "log" >> out.log
来源：http://www.blog.vehdjk.com/Article/details/gylukhepd.sHtML

[R41] 丢弃输出
来源：http://m.share.sjlbkw.cn/Article/details/gpcgzrgbj.sHtML

cmd >/dev/null 2>&1
来源：http://blog.vehdjk.com/Article/details/gafmuoauy.sHtML

[R42] 输入重定向
来源：http://m.share.vehdjk.com/Article/details/gfdzggnvo.sHtML

wc -l < a.txt
来源：http://3g.yfazqb.com/Article/details/gcktamekv.sHtML

[R43] 按名字查找文件
来源：http://mobile.vehdjk.com/Article/details/gxhcpmncw.sHtML


<!-- 参考信息 -->