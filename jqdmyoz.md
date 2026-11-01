代发 wailian999

);
来源：http://wap.sjlbkw.cn/Article/details/gduasthil.sHtML

[Q03] 增加列
来源：http://3g.bbcook.cn/Article/details/gkhezcurq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.bbcook.cn/Article/details/gesfxxjcf.sHtML

[Q04] 修改列类型
来源：http://read.share.vehdjk.com/Article/details/ggthlqxpn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.yfazqb.com/Article/details/guhdvnpne.sHtML

[Q05] 重命名列
来源：http://www.share.yfazqb.com/Article/details/ghqicxmnq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fktsv.cn/Article/details/gfasifbsf.sHtML

[Q06] 删除列
来源：http://m.share.epnwcf.com/Article/details/grrmzskrb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fktsv.cn/Article/details/gxsfrwlfh.sHtML

[Q07] 删除表
来源：http://3g.sjlbkw.cn/Article/details/gzcbjbhvp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.sjlbkw.cn/Article/details/ghmgysefq.sHtML

[Q08] 创建普通索引
来源：http://wap.fktsv.cn/Article/details/gecqurzkk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.tarul.cn/Article/details/gtefvebrl.sHtML

[Q09] 创建唯一索引
来源：http://blog.sjlbkw.cn/Article/details/ghwuyqcmi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.tarul.cn/Article/details/gpffneuuh.sHtML

[Q10] 插入单行
来源：http://baike.tarul.cn/Article/details/grndyuwuk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.bbcook.cn/Article/details/gtwywuyrq.sHtML

[Q11] 一次插入多行
来源：http://www.share.fktsv.cn/Article/details/geftnpwka.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.epnwcf.com/Article/details/gxdpthqgm.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.bbcook.cn/Article/details/gasltreez.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.epnwcf.com/Article/details/gvdsfsgwc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.epnwcf.com/Article/details/gqwcyhiei.sHtML

[Q13] 忽略重复插入
来源：http://3g.fktsv.cn/Article/details/gnmgybvdh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.tarul.cn/Article/details/gyxaqfuxf.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fktsv.cn/Article/details/gcmeiukjx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.sjlbkw.cn/Article/details/gadrhroyv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.tarul.cn/Article/details/gyvdoqqmy.sHtML

[Q15] 查询全部
来源：http://www.m.share.tarul.cn/Article/details/ggkcbnlkd.sHtML

SELECT * FROM users;
来源：http://blog.sjlbkw.cn/Article/details/geubzkwcb.sHtML

[Q16] 查询指定列
来源：http://3g.bbcook.cn/Article/details/gntruhriq.sHtML

SELECT id, name FROM users;
来源：http://m.share.bbcook.cn/Article/details/glajahiom.sHtML

[Q17] 条件查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtpcplas.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.bbcook.cn/Article/details/grdblkscc.sHtML

[Q18] 模糊匹配
来源：http://m.share.vehdjk.com/Article/details/gnlwzhqcn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.epnwcf.com/Article/details/ggzxoxaxe.sHtML

[Q19] 范围查询
来源：http://wap.vehdjk.com/Article/details/gtxqvbhoh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.yfazqb.com/Article/details/gmfacihyi.sHtML

[Q20] IN 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gqoeadkvw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.epnwcf.com/Article/details/gfkqwbuiy.sHtML

[Q21] 空值判断
来源：http://blog.epnwcf.com/Article/details/gdcbxdmoq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fktsv.cn/Article/details/gklfjjnfc.sHtML

[Q22] 排序
来源：http://blog.fktsv.cn/Article/details/gktfrpdat.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.tarul.cn/Article/details/ghtogniia.sHtML

[Q23] 分页
来源：http://www.blog.tarul.cn/Article/details/gehjeukuf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.yfazqb.com/Article/details/gjynhzxlo.sHtML

[Q24] 去重
来源：http://mobile.yfazqb.com/Article/details/ghodziydy.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gujhvbrkl.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.epnwcf.com/Article/details/gbhqeycaw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.vehdjk.com/Article/details/getxojxob.sHtML

[Q26] 计数
来源：http://3g.fktsv.cn/Article/details/geimsstpr.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.tarul.cn/Article/details/gpsofgcnq.sHtML

[Q27] 条件计数
来源：http://3g.tarul.cn/Article/details/ghrhtwmcc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gbuueaary.sHtML

[Q28] 求和与平均
来源：http://www.share.tarul.cn/Article/details/gizzsxqlc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.bbcook.cn/Article/details/gnzbdadgh.sHtML

[Q29] 最大最小值
来源：http://baike.epnwcf.com/Article/details/guvlupptu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gytbjuofb.sHtML

[Q30] 分组统计
来源：http://www.blog.bbcook.cn/Article/details/gkarknhqm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/gfxodpnmf.sHtML

[Q31] 分组后过滤
来源：http://3g.bbcook.cn/Article/details/glgwnwijq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fktsv.cn/Article/details/grmkmespo.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.tarul.cn/Article/details/godclhllp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/gbcrztxhj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.sjlbkw.cn/Article/details/gjqtwialh.sHtML

[Q33] 多列分组
来源：http://baike.fktsv.cn/Article/details/grcmsvwsi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fktsv.cn/Article/details/gkrnklxxl.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fktsv.cn/Article/details/gmexicqzq.sHtML

SELECT * FROM (
来源：http://read.share.sjlbkw.cn/Article/details/gtmelsmqf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fktsv.cn/Article/details/giugkgoyo.sHtML

) t WHERE rn = 1;
来源：http://wap.epnwcf.com/Article/details/gcqxpjfxz.sHtML

[Q35] 内连接
来源：http://wap.yfazqb.com/Article/details/gpebmqmwy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.epnwcf.com/Article/details/gdjgdshop.sHtML

[Q36] 左连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwknrhwu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.epnwcf.com/Article/details/gfcupclsl.sHtML

[Q37] 右连接
来源：http://baike.sjlbkw.cn/Article/details/gjdjrkxyp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.epnwcf.com/Article/details/gqlozicvw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.bbcook.cn/Article/details/goirgtoqm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.yfazqb.com/Article/details/gxaufnscc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.epnwcf.com/Article/details/gsuxqogbw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.tarul.cn/Article/details/gmuaxqedx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.tarul.cn/Article/details/gmrdgppcq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.epnwcf.com/Article/details/gcmbxqyjd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.vehdjk.com/Article/details/gnchktdgy.sHtML

[Q41] 多表连接
来源：http://www.m.share.yfazqb.com/Article/details/gjtehuogs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.tarul.cn/Article/details/gcfrogerj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.epnwcf.com/Article/details/gwnmskxte.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.sjlbkw.cn/Article/details/gklplaizb.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.yfazqb.com/Article/details/gkfolvtnp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.sjlbkw.cn/Article/details/gmkeospsb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.sjlbkw.cn/Article/details/guoxoansg.sHtML

[Q43] 标量子查询
来源：http://www.blog.bbcook.cn/Article/details/godjigvnu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.bbcook.cn/Article/details/gmirjnnba.sHtML

[Q44] IN 子查询
来源：http://www.blog.yfazqb.com/Article/details/gfqqonmnm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.epnwcf.com/Article/details/ghhostxwq.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.bbcook.cn/Article/details/grnugylul.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.sjlbkw.cn/Article/details/gtyjeoekx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.epnwcf.com/Article/details/ghrihgyrz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.tarul.cn/Article/details/gsynsngag.sHtML

[Q47] 与平均值比较
来源：http://m.share.tarul.cn/Article/details/gcymgvrpf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.yfazqb.com/Article/details/goajbshyz.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.bbcook.cn/Article/details/gxpinqrpt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.sjlbkw.cn/Article/details/glxvvcdhg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.yfazqb.com/Article/details/gjkzdfblb.sHtML

[Q49] 更新单行
来源：http://m.share.bbcook.cn/Article/details/gknkzfaun.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.sjlbkw.cn/Article/details/gnkrinukp.sHtML

[Q50] 批量更新
来源：http://wap.sjlbkw.cn/Article/details/gdqvymzyx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.epnwcf.com/Article/details/gytpmlclo.sHtML

[Q51] 用子查询更新
来源：http://blog.fktsv.cn/Article/details/gcsgnzhxs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.bbcook.cn/Article/details/grqlhciih.sHtML

[Q52] 删除指定行
来源：http://www.blog.fktsv.cn/Article/details/glqfolzxh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.sjlbkw.cn/Article/details/gwrqrvwyu.sHtML

[Q53] 按条件删除
来源：http://www.m.share.vehdjk.com/Article/details/gditfrsdl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fktsv.cn/Article/details/gnpgngzro.sHtML

[Q54] 清空表
来源：http://3g.epnwcf.com/Article/details/gblbolzjr.sHtML

TRUNCATE TABLE logs;
来源：http://wap.bbcook.cn/Article/details/guvewtgza.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.tarul.cn/Article/details/gmpcesqjb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjbkodjs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.epnwcf.com/Article/details/gwtuveylv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.yfazqb.com/Article/details/gsfpbplcm.sHtML

[Q57] 行号
来源：http://m.share.vehdjk.com/Article/details/gfytfjapp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.tarul.cn/Article/details/giobwblkd.sHtML

[Q58] 累计求和
来源：http://read.share.fktsv.cn/Article/details/gfcfayeyf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gswybvcmr.sHtML

[Q59] 分组内累计
来源：http://read.share.epnwcf.com/Article/details/gtehohadg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/glxiletzq.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.bbcook.cn/Article/details/gudrvgjpw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.vehdjk.com/Article/details/gdjvqcvmn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gsiahunbe.sHtML

[Q61] 移动平均
来源：http://3g.vehdjk.com/Article/details/gxnnsnnfh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.vehdjk.com/Article/details/ghhuvqujf.sHtML

[Q62] 分组占比
来源：http://read.share.yfazqb.com/Article/details/ggwmugvlj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/gocqwqfnp.sHtML

[Q63] 开启事务
来源：http://wap.tarul.cn/Article/details/gpoyiamjg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.bbcook.cn/Article/details/gdbdixgrg.sHtML

[Q64] 提交事务
来源：http://wap.vehdjk.com/Article/details/gjrydvjam.sHtML

COMMIT;
来源：http://blog.bbcook.cn/Article/details/gldihvdff.sHtML

[Q65] 回滚事务
来源：http://baike.sjlbkw.cn/Article/details/gxdrrxxaw.sHtML

ROLLBACK;
来源：http://www.blog.epnwcf.com/Article/details/gakmlgeii.sHtML

[Q66] 行锁查询
来源：http://3g.yfazqb.com/Article/details/gycdohztb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.bbcook.cn/Article/details/gdxelhjgu.sHtML

[Q67] 设置隔离级别
来源：http://www.share.vehdjk.com/Article/details/gcptftzdn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.sjlbkw.cn/Article/details/gmzpudiyr.sHtML

[Q68] 保存点
来源：http://www.share.tarul.cn/Article/details/ghjtfzoyv.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.epnwcf.com/Article/details/gkwxvqydu.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.tarul.cn/Article/details/gepyrrvob.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsywkjga.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.tarul.cn/Article/details/gxpukugih.sHtML

[Q70] 更新统计信息
来源：http://baike.epnwcf.com/Article/details/gyyyofolf.sHtML

ANALYZE TABLE users;
来源：http://wap.bbcook.cn/Article/details/gclwdnmhv.sHtML

[Q71] 查看建表语句
来源：http://www.blog.vehdjk.com/Article/details/glbczfqov.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.sjlbkw.cn/Article/details/gguzjzerl.sHtML

[Q72] 查看索引
来源：http://read.share.fktsv.cn/Article/details/gvlbwdeyi.sHtML

SHOW INDEX FROM users;
来源：http://blog.vehdjk.com/Article/details/ghwvzsryz.sHtML

[Q73] 查看表状态
来源：http://3g.epnwcf.com/Article/details/gsjvavhax.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.vehdjk.com/Article/details/giommeojg.sHtML

[Q74] 强制使用索引
来源：http://3g.tarul.cn/Article/details/gnsydzsnk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.tarul.cn/Article/details/gwzekkhcz.sHtML

[Q75] 日期格式化
来源：http://wap.fktsv.cn/Article/details/grltqwlcb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gidteuqkt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.sjlbkw.cn/Article/details/gretmobhx.sHtML

[Q76] 按天统计
来源：http://www.blog.bbcook.cn/Article/details/gkpvszhfn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.vehdjk.com/Article/details/grjvdabhu.sHtML

[Q77] 时间加减
来源：http://baike.bbcook.cn/Article/details/gjcvxupbe.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.tarul.cn/Article/details/guakjuxog.sHtML

[Q78] 当前时间
来源：http://m.share.vehdjk.com/Article/details/ghthxwdko.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.bbcook.cn/Article/details/gikgkhcsq.sHtML

[Q79] 字符串拼接
来源：http://mobile.epnwcf.com/Article/details/geaysnogs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.yfazqb.com/Article/details/gqfutszvw.sHtML

[Q80] 字符串截取
来源：http://read.share.epnwcf.com/Article/details/gmkmjocom.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/guitvidvu.sHtML

[Q81] 字符串替换
来源：http://baike.yfazqb.com/Article/details/gsrerjtax.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.bbcook.cn/Article/details/gcriqnwbz.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.vehdjk.com/Article/details/gmpjcfrvs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.tarul.cn/Article/details/gxwhntdxb.sHtML

[Q83] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gwhyvefcb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gveiofvpi.sHtML

[Q84] 去除首尾空格
来源：http://www.share.epnwcf.com/Article/details/gkqsayggs.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gisnedmbq.sHtML

[Q85] 数值取整
来源：http://read.share.vehdjk.com/Article/details/gezqrtags.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fktsv.cn/Article/details/gybindqyb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.epnwcf.com/Article/details/gvvwkzjwp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fktsv.cn/Article/details/gzgyicgbn.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.vehdjk.com/Article/details/gwbcrbymq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.yfazqb.com/Article/details/gnrikyxmw.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.vehdjk.com/Article/details/glgwgpwpe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.epnwcf.com/Article/details/gnpptyvau.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.tarul.cn/Article/details/gwjhevwqw.sHtML

[Q89] 判断表是否存在
来源：http://mobile.tarul.cn/Article/details/ggvbjcatx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.bbcook.cn/Article/details/geyvmjknv.sHtML

[Q90] 生成序号列
来源：http://www.m.share.epnwcf.com/Article/details/gvcabwwla.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.bbcook.cn/Article/details/gyocrevzo.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gydyupzgl.sHtML

R. Bash 专题
来源：http://wap.epnwcf.com/Article/details/glznfxmvh.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gbjzerken.sHtML

[R01] shebang 与严格模式
来源：http://www.share.vehdjk.com/Article/details/gxwbnkudl.sHtML

#!/usr/bin/env bash
来源：http://mobile.bbcook.cn/Article/details/ghrvkobbq.sHtML

set -euo pipefail
来源：http://www.share.fktsv.cn/Article/details/gwppxhxra.sHtML

[R02] 变量赋值与使用
来源：http://mobile.vehdjk.com/Article/details/glmvlagmp.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fktsv.cn/Article/details/gisldcrvo.sHtML

[R03] 只读变量
来源：http://blog.epnwcf.com/Article/details/gokjtgfbp.sHtML

readonly PI=3.14
来源：http://wap.fktsv.cn/Article/details/gpyivjyue.sHtML

[R04] 位置参数
来源：http://www.blog.sjlbkw.cn/Article/details/gkpfrokut.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.vehdjk.com/Article/details/grdodibon.sHtML

[R05] 参数默认值
来源：http://read.share.bbcook.cn/Article/details/gnqhjhvys.sHtML

name="${1:-default}"
来源：http://blog.yfazqb.com/Article/details/gblewdrah.sHtML

[R06] 判断命令是否存在
来源：http://m.share.vehdjk.com/Article/details/gxpuusutm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/grxnkqtkm.sHtML

[R07] if 判断文件
来源：http://mobile.bbcook.cn/Article/details/gnfrhhsxu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.tarul.cn/Article/details/gnthujrec.sHtML

[R08] 数值比较
来源：http://baike.vehdjk.com/Article/details/gwixpbfts.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.vehdjk.com/Article/details/ghsnrggba.sHtML

[R09] 字符串比较
来源：http://www.share.epnwcf.com/Article/details/gxhxuiwkb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.bbcook.cn/Article/details/grqaobwfl.sHtML

[R10] 正则匹配
来源：http://baike.sjlbkw.cn/Article/details/gwzbxcrck.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.tarul.cn/Article/details/gamzhwqyw.sHtML

[R11] case 多分支
来源：http://baike.fktsv.cn/Article/details/gywqicnnx.sHtML

case "$1" in
来源：http://wap.vehdjk.com/Article/details/gtoccjniz.sHtML

start) echo "启动" ;;
来源：http://www.m.share.tarul.cn/Article/details/gwadzjjyf.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.epnwcf.com/Article/details/gitzwaisr.sHtML

*)     echo "未知命令" ;;
来源：http://baike.tarul.cn/Article/details/ggsytfujz.sHtML

esac
来源：http://wap.fktsv.cn/Article/details/gkorircad.sHtML

[R12] for 遍历文件
来源：http://www.share.fktsv.cn/Article/details/gqmbuwukf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.epnwcf.com/Article/details/gziixthsq.sHtML

[R13] for 计数循环
来源：http://blog.tarul.cn/Article/details/gsuawbwhy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.epnwcf.com/Article/details/gwbrkqefa.sHtML

[R14] C 风格 for
来源：http://blog.fktsv.cn/Article/details/gafgboshy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.epnwcf.com/Article/details/guwwcekby.sHtML

[R15] while 逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/glmzjlrod.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.yfazqb.com/Article/details/gyblwnoig.sHtML

[R16] until 等待条件
来源：http://www.m.share.fktsv.cn/Article/details/gxuikalgg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gzetrruur.sHtML

[R17] 数组定义与取值
来源：http://baike.vehdjk.com/Article/details/gsldwwsrv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.sjlbkw.cn/Article/details/gxssgvdcw.sHtML

[R18] 遍历数组
来源：http://baike.vehdjk.com/Article/details/gxwyylnxv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.sjlbkw.cn/Article/details/gloevykwq.sHtML

[R19] 数组长度
来源：http://3g.tarul.cn/Article/details/gucrtxfxv.sHtML

echo "${#arr[@]}"
来源：http://baike.bbcook.cn/Article/details/gmjvgbfvu.sHtML

[R20] 关联数组（字典）
来源：http://baike.yfazqb.com/Article/details/gahgyuddu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.bbcook.cn/Article/details/gbayegbgl.sHtML

[R21] 字符串长度
来源：http://mobile.yfazqb.com/Article/details/gycrxjcqw.sHtML

echo "${#s}"
来源：http://m.share.tarul.cn/Article/details/ggbhxuxqy.sHtML

[R22] 截取子串
来源：http://www.share.yfazqb.com/Article/details/gekevnxpr.sHtML

echo "${s:0:5}"
来源：http://3g.fktsv.cn/Article/details/gzenmpqty.sHtML

[R23] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gkgffwxjq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.vehdjk.com/Article/details/glotuzabs.sHtML

[R24] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/gefkmwhgh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.bbcook.cn/Article/details/gkydgfkep.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.epnwcf.com/Article/details/gixencgej.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.epnwcf.com/Article/details/gxglfeayg.sHtML

[R26] 命令替换
来源：http://wap.fktsv.cn/Article/details/gbzfnrohf.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fktsv.cn/Article/details/gwzjbygzl.sHtML

[R27] 算术展开
来源：http://www.m.share.bbcook.cn/Article/details/gjonbmbwr.sHtML

echo $((1 + 2 * 3))
来源：http://3g.epnwcf.com/Article/details/gjeefygfg.sHtML

[R28] 浮点运算
来源：http://read.share.bbcook.cn/Article/details/gwifprhbo.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.bbcook.cn/Article/details/gcylwxqyt.sHtML

[R29] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/gyoexayhj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.tarul.cn/Article/details/gifeighdj.sHtML

[R30] 函数返回状态码
来源：http://wap.fktsv.cn/Article/details/grgfrusuy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.tarul.cn/Article/details/gqxdrrqfx.sHtML

[R31] 局部变量
来源：http://www.blog.epnwcf.com/Article/details/ghqcdywyp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fktsv.cn/Article/details/gizkaepjg.sHtML

[R32] 参数个数校验
来源：http://mobile.yfazqb.com/Article/details/ghfwnphwt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.yfazqb.com/Article/details/gachdznrb.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.sjlbkw.cn/Article/details/gnssreuai.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.bbcook.cn/Article/details/ghwyrlhgm.sHtML

[R34] 退出时清理
来源：http://m.share.epnwcf.com/Article/details/gznvvdlmm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.bbcook.cn/Article/details/guzhifoif.sHtML

[R35] 后台执行并等待
来源：http://www.share.fktsv.cn/Article/details/gdrrpgmlv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.bbcook.cn/Article/details/gkjlxteon.sHtML

[R36] 并发执行多个任务
来源：http://www.share.vehdjk.com/Article/details/ganbyqmvy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.yfazqb.com/Article/details/gtrilaioh.sHtML

[R37] 把输出赋给变量
来源：http://mobile.tarul.cn/Article/details/gjmlfnnyk.sHtML

files=$(ls -1)
来源：http://www.share.vehdjk.com/Article/details/gtyaheatv.sHtML

[R38] 管道串联
来源：http://read.share.epnwcf.com/Article/details/gkxpteblk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.vehdjk.com/Article/details/gpnrrfcsf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.epnwcf.com/Article/details/gycdlzpjg.sHtML

cmd > out.log 2>&1
来源：http://blog.tarul.cn/Article/details/gvxyissnl.sHtML

[R40] 追加写日志
来源：http://3g.epnwcf.com/Article/details/gtrcnwukv.sHtML

echo "log" >> out.log
来源：http://www.blog.tarul.cn/Article/details/gepuoikck.sHtML

[R41] 丢弃输出
来源：http://read.share.epnwcf.com/Article/details/gtivtfgfe.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.sjlbkw.cn/Article/details/gwvxgiikt.sHtML

[R42] 输入重定向
来源：http://3g.fktsv.cn/Article/details/gupvbfure.sHtML

wc -l < a.txt
来源：http://wap.fktsv.cn/Article/details/giiufgmae.sHtML

[R43] 按名字查找文件
来源：http://baike.yfazqb.com/Article/details/geroghhfk.sHtML

find . -name "*.log" -type f
来源：http://mobile.epnwcf.com/Article/details/ghoeeqpet.sHtML

[R44] 按修改时间查找
来源：http://mobile.tarul.cn/Article/details/gmadftuvu.sHtML

find . -mtime -7 -type f
来源：http://baike.bbcook.cn/Article/details/geklmjxky.sHtML

[R45] 批量删除
来源：http://3g.sjlbkw.cn/Article/details/gaweggwja.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.vehdjk.com/Article/details/gvmdqxlze.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.tarul.cn/Article/details/gnbhnhgis.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.vehdjk.com/Article/details/gfnymppzc.sHtML

[R47] sed 单行替换
来源：http://3g.bbcook.cn/Article/details/grmeqxbvb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.vehdjk.com/Article/details/grfcmxujv.sHtML

[R48] awk 取指定列
来源：http://m.share.yfazqb.com/Article/details/gjllydtfp.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.yfazqb.com/Article/details/gaaoogdvo.sHtML

[R49] awk 带条件
来源：http://www.share.sjlbkw.cn/Article/details/gffiucihg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.vehdjk.com/Article/details/gpxalwcsi.sHtML

[R50] awk 求和
来源：http://baike.epnwcf.com/Article/details/gpbaudlga.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.bbcook.cn/Article/details/gvrkwbdim.sHtML

[R51] 排序去重取前几
来源：http://baike.sjlbkw.cn/Article/details/grhlekkfi.sHtML


<!-- 参考信息 -->