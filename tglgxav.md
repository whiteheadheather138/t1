代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.sjlbkw.cn/Article/details/gqmslgpge.sHtML

user_id INT NOT NULL,
来源：http://www.share.tarul.cn/Article/details/gsehwbwgr.sHtML

amount DECIMAL(10, 2),
来源：http://blog.vehdjk.com/Article/details/gficudefg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.vehdjk.com/Article/details/gumwvaynb.sHtML

);
来源：http://www.share.yfazqb.com/Article/details/gfxannjzz.sHtML

[Q03] 增加列
来源：http://mobile.yfazqb.com/Article/details/gbgrkaork.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.bbcook.cn/Article/details/guegrqdxg.sHtML

[Q04] 修改列类型
来源：http://www.share.yfazqb.com/Article/details/golaxfeza.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/gffaludll.sHtML

[Q05] 重命名列
来源：http://3g.yfazqb.com/Article/details/gygpvbqmv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.tarul.cn/Article/details/gjyybpxmx.sHtML

[Q06] 删除列
来源：http://mobile.fktsv.cn/Article/details/gerssbukp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fktsv.cn/Article/details/gexwcajum.sHtML

[Q07] 删除表
来源：http://m.share.bbcook.cn/Article/details/glxhilzou.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.bbcook.cn/Article/details/gocrivdei.sHtML

[Q08] 创建普通索引
来源：http://blog.sjlbkw.cn/Article/details/gatuexspx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.sjlbkw.cn/Article/details/gdaiwqwjt.sHtML

[Q09] 创建唯一索引
来源：http://blog.sjlbkw.cn/Article/details/ggyfubmww.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.vehdjk.com/Article/details/gnlvpiebr.sHtML

[Q10] 插入单行
来源：http://m.share.tarul.cn/Article/details/gvjovaubl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.sjlbkw.cn/Article/details/gkgwrpfxr.sHtML

[Q11] 一次插入多行
来源：http://mobile.vehdjk.com/Article/details/gojbabcro.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.epnwcf.com/Article/details/ggzonzffj.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.tarul.cn/Article/details/gnblikyfy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.yfazqb.com/Article/details/gascqgaaj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.tarul.cn/Article/details/gpbpcssqs.sHtML

[Q13] 忽略重复插入
来源：http://blog.yfazqb.com/Article/details/gdjwauizo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gcudboqsy.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.tarul.cn/Article/details/gfcanghhi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.tarul.cn/Article/details/gwivmnokx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.vehdjk.com/Article/details/ghtvyveve.sHtML

[Q15] 查询全部
来源：http://read.share.fktsv.cn/Article/details/gmhimsbdy.sHtML

SELECT * FROM users;
来源：http://mobile.bbcook.cn/Article/details/gnqfjbgug.sHtML

[Q16] 查询指定列
来源：http://3g.vehdjk.com/Article/details/gywqkoqar.sHtML

SELECT id, name FROM users;
来源：http://mobile.epnwcf.com/Article/details/ghwmqovhb.sHtML

[Q17] 条件查询
来源：http://blog.tarul.cn/Article/details/gymihiykn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.vehdjk.com/Article/details/gfynccrmq.sHtML

[Q18] 模糊匹配
来源：http://wap.tarul.cn/Article/details/gynswttcs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.tarul.cn/Article/details/gxjmmfshj.sHtML

[Q19] 范围查询
来源：http://www.share.bbcook.cn/Article/details/ghopebdbl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.epnwcf.com/Article/details/gtvvuiuug.sHtML

[Q20] IN 列表
来源：http://www.share.tarul.cn/Article/details/granldcga.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.bbcook.cn/Article/details/gumeirnab.sHtML

[Q21] 空值判断
来源：http://mobile.yfazqb.com/Article/details/ggmysdvno.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.sjlbkw.cn/Article/details/guxnxhvzr.sHtML

[Q22] 排序
来源：http://wap.fktsv.cn/Article/details/gtfulpmme.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.bbcook.cn/Article/details/gtefofdev.sHtML

[Q23] 分页
来源：http://www.blog.fktsv.cn/Article/details/gzbxwrjop.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.vehdjk.com/Article/details/ghlouovfr.sHtML

[Q24] 去重
来源：http://mobile.sjlbkw.cn/Article/details/gwsocsgkt.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.vehdjk.com/Article/details/gciqmotbw.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fktsv.cn/Article/details/gzmnvewzk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.tarul.cn/Article/details/gnvjgdnyu.sHtML

[Q26] 计数
来源：http://blog.vehdjk.com/Article/details/gespbiphp.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gitgwoqou.sHtML

[Q27] 条件计数
来源：http://read.share.yfazqb.com/Article/details/ggrxklepw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.tarul.cn/Article/details/geclzmrwf.sHtML

[Q28] 求和与平均
来源：http://www.blog.fktsv.cn/Article/details/gkmyhocrw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gldbjdxdj.sHtML

[Q29] 最大最小值
来源：http://www.blog.yfazqb.com/Article/details/geileibiu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gxsmdpdzb.sHtML

[Q30] 分组统计
来源：http://www.m.share.vehdjk.com/Article/details/gmvpzrcek.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/gbwgvbkzh.sHtML

[Q31] 分组后过滤
来源：http://baike.tarul.cn/Article/details/gwrtgyxzt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.sjlbkw.cn/Article/details/grouugyuo.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gqjnvppza.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.epnwcf.com/Article/details/gmiuyfhvl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.vehdjk.com/Article/details/gedxoutxo.sHtML

[Q33] 多列分组
来源：http://www.blog.yfazqb.com/Article/details/gjqitapwd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.bbcook.cn/Article/details/gbxekizjb.sHtML

[Q34] 每组取第一条
来源：http://baike.vehdjk.com/Article/details/gzxdeicjc.sHtML

SELECT * FROM (
来源：http://www.m.share.epnwcf.com/Article/details/gdydpnkhj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.bbcook.cn/Article/details/gxkryxcud.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gkkaxbjsy.sHtML

[Q35] 内连接
来源：http://www.m.share.vehdjk.com/Article/details/gqzowamoq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/geispqcjx.sHtML

[Q36] 左连接
来源：http://wap.sjlbkw.cn/Article/details/gdbjrkrks.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/gzedoangx.sHtML

[Q37] 右连接
来源：http://wap.vehdjk.com/Article/details/gwsupbgnf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.sjlbkw.cn/Article/details/gqutcgibk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.sjlbkw.cn/Article/details/ggehszxgh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.epnwcf.com/Article/details/gybkgjuhg.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.epnwcf.com/Article/details/gkctqkhze.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.epnwcf.com/Article/details/gcpooyyji.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.vehdjk.com/Article/details/guuazaspp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.yfazqb.com/Article/details/gpuupyawn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.bbcook.cn/Article/details/gaphoqaoh.sHtML

[Q41] 多表连接
来源：http://wap.vehdjk.com/Article/details/guquvnwni.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzxtmmdo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.bbcook.cn/Article/details/gousmjscp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.epnwcf.com/Article/details/gnqbrmpii.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.tarul.cn/Article/details/gnkcwfdif.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.epnwcf.com/Article/details/ghjkspmga.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.yfazqb.com/Article/details/gnbjjqmjo.sHtML

[Q43] 标量子查询
来源：http://www.share.yfazqb.com/Article/details/gbdkgbpwi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fktsv.cn/Article/details/grzehayft.sHtML

[Q44] IN 子查询
来源：http://blog.fktsv.cn/Article/details/gowztrhmn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fktsv.cn/Article/details/gnfwbgydp.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.bbcook.cn/Article/details/gaivelmnh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.sjlbkw.cn/Article/details/gaivbbsbl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.sjlbkw.cn/Article/details/gucgxyywx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.epnwcf.com/Article/details/glutgrios.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.vehdjk.com/Article/details/ggiomvmxv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.bbcook.cn/Article/details/gggvbpoms.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.vehdjk.com/Article/details/gpxwofdbe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.epnwcf.com/Article/details/gpeotipcn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.sjlbkw.cn/Article/details/ghocubfdv.sHtML

[Q49] 更新单行
来源：http://wap.tarul.cn/Article/details/gxabmpiur.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.vehdjk.com/Article/details/gjxjykejm.sHtML

[Q50] 批量更新
来源：http://baike.yfazqb.com/Article/details/gpeaxoryj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.tarul.cn/Article/details/gxeihgzkf.sHtML

[Q51] 用子查询更新
来源：http://m.share.sjlbkw.cn/Article/details/gndsogcih.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.vehdjk.com/Article/details/gnuzwzmoo.sHtML

[Q52] 删除指定行
来源：http://www.blog.sjlbkw.cn/Article/details/gcwvifvtl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/gjwlrtldp.sHtML

[Q53] 按条件删除
来源：http://blog.fktsv.cn/Article/details/gdshhrvzc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.epnwcf.com/Article/details/gxuoahskf.sHtML

[Q54] 清空表
来源：http://blog.yfazqb.com/Article/details/gbvechbry.sHtML

TRUNCATE TABLE logs;
来源：http://baike.bbcook.cn/Article/details/gyjqapojo.sHtML

[Q55] 排名（并列占位）
来源：http://baike.yfazqb.com/Article/details/gcgwjdoev.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.tarul.cn/Article/details/guwqxrrkc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.yfazqb.com/Article/details/gfthftrjk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.yfazqb.com/Article/details/gnagitfov.sHtML

[Q57] 行号
来源：http://read.share.sjlbkw.cn/Article/details/gklyvncto.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.bbcook.cn/Article/details/gsedohaop.sHtML

[Q58] 累计求和
来源：http://www.blog.vehdjk.com/Article/details/gkozfxqvv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gmkoiltvc.sHtML

[Q59] 分组内累计
来源：http://3g.vehdjk.com/Article/details/gksdrzjnp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.bbcook.cn/Article/details/ggbckbmdw.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.sjlbkw.cn/Article/details/govjydrfn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.yfazqb.com/Article/details/ggyswjdec.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fktsv.cn/Article/details/gxgtiqvbq.sHtML

[Q61] 移动平均
来源：http://blog.tarul.cn/Article/details/gsnyhcadk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gaoqeztoa.sHtML

[Q62] 分组占比
来源：http://www.blog.yfazqb.com/Article/details/gnlufmjyf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/geadrajea.sHtML

[Q63] 开启事务
来源：http://www.share.bbcook.cn/Article/details/gcstpqvnt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fktsv.cn/Article/details/gtfnbygfz.sHtML

[Q64] 提交事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gwruizaqx.sHtML

COMMIT;
来源：http://www.share.epnwcf.com/Article/details/gupjnhhou.sHtML

[Q65] 回滚事务
来源：http://mobile.epnwcf.com/Article/details/grqostznb.sHtML

ROLLBACK;
来源：http://www.m.share.fktsv.cn/Article/details/gvndzmugr.sHtML

[Q66] 行锁查询
来源：http://mobile.tarul.cn/Article/details/gntvwsktp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.tarul.cn/Article/details/grxewobgb.sHtML

[Q67] 设置隔离级别
来源：http://3g.sjlbkw.cn/Article/details/gvetwqsac.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.epnwcf.com/Article/details/gbcbhugzg.sHtML

[Q68] 保存点
来源：http://read.share.epnwcf.com/Article/details/gokaurofs.sHtML

SAVEPOINT sp1;
来源：http://www.blog.yfazqb.com/Article/details/glntytojq.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fktsv.cn/Article/details/gncbzxyvh.sHtML

[Q69] 查看执行计划
来源：http://wap.yfazqb.com/Article/details/gvtnbeqkq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.tarul.cn/Article/details/gvsehswyn.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fktsv.cn/Article/details/gjfsismbg.sHtML

ANALYZE TABLE users;
来源：http://3g.fktsv.cn/Article/details/gqxqzxwta.sHtML

[Q71] 查看建表语句
来源：http://blog.yfazqb.com/Article/details/gioqddqca.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fktsv.cn/Article/details/gyjfuabhf.sHtML

[Q72] 查看索引
来源：http://www.blog.yfazqb.com/Article/details/ghscniwzj.sHtML

SHOW INDEX FROM users;
来源：http://read.share.yfazqb.com/Article/details/gkfccwcvx.sHtML

[Q73] 查看表状态
来源：http://read.share.bbcook.cn/Article/details/gdrjiktju.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.yfazqb.com/Article/details/gzvpjxdyk.sHtML

[Q74] 强制使用索引
来源：http://baike.bbcook.cn/Article/details/grhjwvekq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fktsv.cn/Article/details/gzrugqyka.sHtML

[Q75] 日期格式化
来源：http://m.share.tarul.cn/Article/details/gtjvvdflc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gqhgaxzqi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.epnwcf.com/Article/details/grgogvnpr.sHtML

[Q76] 按天统计
来源：http://www.share.sjlbkw.cn/Article/details/gahrbiazh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.bbcook.cn/Article/details/gsdfsdumj.sHtML

[Q77] 时间加减
来源：http://www.share.vehdjk.com/Article/details/gkbbdeghn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.vehdjk.com/Article/details/gqgjiqnkj.sHtML

[Q78] 当前时间
来源：http://mobile.epnwcf.com/Article/details/gnixbhsjc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.yfazqb.com/Article/details/gmubaeqho.sHtML

[Q79] 字符串拼接
来源：http://www.share.epnwcf.com/Article/details/gundyrmct.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.epnwcf.com/Article/details/gfysyqhck.sHtML

[Q80] 字符串截取
来源：http://mobile.vehdjk.com/Article/details/gbvutfohk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.vehdjk.com/Article/details/gjbrwvlom.sHtML

[Q81] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/gvvsaurwj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.tarul.cn/Article/details/glsmvbxao.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.sjlbkw.cn/Article/details/goiothakd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gwzttaels.sHtML

[Q83] 大小写转换
来源：http://blog.yfazqb.com/Article/details/gtewcnpcg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/ghodidlcb.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fktsv.cn/Article/details/ggdhllwgi.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gxndeabmt.sHtML

[Q85] 数值取整
来源：http://3g.yfazqb.com/Article/details/gduwncntq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.epnwcf.com/Article/details/gydmmuyfg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.yfazqb.com/Article/details/gwzgkrulg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.tarul.cn/Article/details/gcicrggtt.sHtML

[Q87] JSON 字段做条件
来源：http://wap.sjlbkw.cn/Article/details/gusygeizo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.tarul.cn/Article/details/gakxmeckw.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.sjlbkw.cn/Article/details/gsuuipblk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.epnwcf.com/Article/details/gwmaooxtm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.epnwcf.com/Article/details/gdyyertft.sHtML

[Q89] 判断表是否存在
来源：http://www.share.sjlbkw.cn/Article/details/gikfysbvt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.sjlbkw.cn/Article/details/gyjxxfoks.sHtML

[Q90] 生成序号列
来源：http://baike.sjlbkw.cn/Article/details/gzqzcvutx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.vehdjk.com/Article/details/gcgsozzvi.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gqylyavxr.sHtML

R. Bash 专题
来源：http://mobile.vehdjk.com/Article/details/goocvobne.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gjsoktldk.sHtML

[R01] shebang 与严格模式
来源：http://read.share.yfazqb.com/Article/details/gfdivwoyc.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fktsv.cn/Article/details/gvledddtx.sHtML

set -euo pipefail
来源：http://read.share.sjlbkw.cn/Article/details/gszjtrgrj.sHtML

[R02] 变量赋值与使用
来源：http://m.share.bbcook.cn/Article/details/gcthoewxr.sHtML

name="Tom"; echo "$name"
来源：http://3g.vehdjk.com/Article/details/ghsrlxdum.sHtML

[R03] 只读变量
来源：http://m.share.bbcook.cn/Article/details/gtcsabzlh.sHtML

readonly PI=3.14
来源：http://wap.yfazqb.com/Article/details/gzlyuqypx.sHtML

[R04] 位置参数
来源：http://3g.vehdjk.com/Article/details/gnjpouxei.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdkayaru.sHtML

[R05] 参数默认值
来源：http://www.share.fktsv.cn/Article/details/gbjqcawvh.sHtML

name="${1:-default}"
来源：http://3g.tarul.cn/Article/details/gzwnyvbph.sHtML

[R06] 判断命令是否存在
来源：http://read.share.yfazqb.com/Article/details/ghlbkxzld.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.epnwcf.com/Article/details/gycqrbmym.sHtML

[R07] if 判断文件
来源：http://www.share.vehdjk.com/Article/details/gggvypscd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.epnwcf.com/Article/details/gfvdfpmsu.sHtML

[R08] 数值比较
来源：http://3g.sjlbkw.cn/Article/details/gtxfitjdj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gbvysnzyz.sHtML

[R09] 字符串比较
来源：http://www.blog.vehdjk.com/Article/details/gppwcwpwr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fktsv.cn/Article/details/gfrurpgfu.sHtML

[R10] 正则匹配
来源：http://3g.sjlbkw.cn/Article/details/grgwdgdxo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.tarul.cn/Article/details/geqelzwqj.sHtML

[R11] case 多分支
来源：http://mobile.sjlbkw.cn/Article/details/ggspmwovq.sHtML

case "$1" in
来源：http://www.blog.epnwcf.com/Article/details/gtlvbilsj.sHtML

start) echo "启动" ;;
来源：http://read.share.yfazqb.com/Article/details/gurfkuyrp.sHtML

stop)  echo "停止" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gtkjgzhfc.sHtML

*)     echo "未知命令" ;;
来源：http://wap.tarul.cn/Article/details/glpkdodgf.sHtML

esac
来源：http://www.blog.tarul.cn/Article/details/gznnpvyup.sHtML

[R12] for 遍历文件
来源：http://blog.yfazqb.com/Article/details/gahgmcchq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.yfazqb.com/Article/details/gjmgmthcz.sHtML

[R13] for 计数循环
来源：http://www.m.share.fktsv.cn/Article/details/gjsvlgrnw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.sjlbkw.cn/Article/details/gyfvmwfij.sHtML

[R14] C 风格 for
来源：http://www.m.share.sjlbkw.cn/Article/details/gbdpjbbrp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.epnwcf.com/Article/details/gchkchfrr.sHtML

[R15] while 逐行读文件
来源：http://3g.tarul.cn/Article/details/gsmxpqozk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.tarul.cn/Article/details/gwzwgwqby.sHtML

[R16] until 等待条件
来源：http://baike.fktsv.cn/Article/details/gzxippytc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.sjlbkw.cn/Article/details/gruwzhbpi.sHtML

[R17] 数组定义与取值
来源：http://3g.tarul.cn/Article/details/gembsnqpq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.epnwcf.com/Article/details/gznjkvlbe.sHtML

[R18] 遍历数组
来源：http://read.share.vehdjk.com/Article/details/ghisehtag.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.epnwcf.com/Article/details/gwzpysbvj.sHtML

[R19] 数组长度
来源：http://blog.bbcook.cn/Article/details/gbyhqfjtn.sHtML

echo "${#arr[@]}"
来源：http://baike.fktsv.cn/Article/details/gqopoowik.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.sjlbkw.cn/Article/details/gufjvscsl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.epnwcf.com/Article/details/gpykafffp.sHtML

[R21] 字符串长度
来源：http://read.share.bbcook.cn/Article/details/gnrjjgzfe.sHtML

echo "${#s}"
来源：http://mobile.bbcook.cn/Article/details/gwhdxdidn.sHtML

[R22] 截取子串
来源：http://m.share.yfazqb.com/Article/details/gfedyvxlu.sHtML

echo "${s:0:5}"
来源：http://m.share.yfazqb.com/Article/details/gxafoypxz.sHtML

[R23] 字符串替换
来源：http://m.share.yfazqb.com/Article/details/gaegeyrti.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fktsv.cn/Article/details/gmilggpzs.sHtML

[R24] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/gbpeskcib.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.yfazqb.com/Article/details/glbczufmu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmrcxynm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.bbcook.cn/Article/details/gucheyxlx.sHtML

[R26] 命令替换
来源：http://m.share.bbcook.cn/Article/details/gjmclxhfd.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.bbcook.cn/Article/details/gipogntlc.sHtML

[R27] 算术展开
来源：http://3g.fktsv.cn/Article/details/grcsjglru.sHtML

echo $((1 + 2 * 3))
来源：http://baike.sjlbkw.cn/Article/details/ghumsulld.sHtML

[R28] 浮点运算
来源：http://www.m.share.yfazqb.com/Article/details/gaelquzbt.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.sjlbkw.cn/Article/details/gfdtxfzce.sHtML

[R29] 定义函数
来源：http://baike.vehdjk.com/Article/details/gfejnqqxb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.vehdjk.com/Article/details/ghupvawod.sHtML

[R30] 函数返回状态码
来源：http://www.blog.bbcook.cn/Article/details/gavhhdvui.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.tarul.cn/Article/details/gjrhhvbrw.sHtML

[R31] 局部变量
来源：http://wap.sjlbkw.cn/Article/details/gwvlvvmyr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.tarul.cn/Article/details/gpawaudbp.sHtML

[R32] 参数个数校验
来源：http://www.blog.bbcook.cn/Article/details/gjibybukn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/gicpkffjl.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.epnwcf.com/Article/details/gmqbugeey.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.tarul.cn/Article/details/goepwffed.sHtML

[R34] 退出时清理
来源：http://3g.tarul.cn/Article/details/gahqcdxbe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.vehdjk.com/Article/details/ggfzgxqgx.sHtML

[R35] 后台执行并等待
来源：http://3g.vehdjk.com/Article/details/gxnuershl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.yfazqb.com/Article/details/gktjeetwl.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.vehdjk.com/Article/details/gxdapypum.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.vehdjk.com/Article/details/gezlethnn.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.bbcook.cn/Article/details/gsuijzoss.sHtML

files=$(ls -1)
来源：http://m.share.sjlbkw.cn/Article/details/gwjspgitm.sHtML

[R38] 管道串联
来源：http://mobile.bbcook.cn/Article/details/gvlnjtnlz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.epnwcf.com/Article/details/gqlkewqbt.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.sjlbkw.cn/Article/details/govyxtmlh.sHtML

cmd > out.log 2>&1
来源：http://baike.sjlbkw.cn/Article/details/gstzmncnz.sHtML

[R40] 追加写日志
来源：http://baike.tarul.cn/Article/details/gkhqizmes.sHtML

echo "log" >> out.log
来源：http://3g.epnwcf.com/Article/details/ghjquievi.sHtML

[R41] 丢弃输出
来源：http://wap.vehdjk.com/Article/details/gjhalghko.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.bbcook.cn/Article/details/gnprfimjo.sHtML

[R42] 输入重定向
来源：http://wap.bbcook.cn/Article/details/gtzbtnnap.sHtML

wc -l < a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gkqsggcuq.sHtML

[R43] 按名字查找文件
来源：http://www.share.epnwcf.com/Article/details/ghvopyojf.sHtML

find . -name "*.log" -type f
来源：http://wap.epnwcf.com/Article/details/gbdniikhi.sHtML

[R44] 按修改时间查找
来源：http://m.share.tarul.cn/Article/details/gzlcgprqf.sHtML

find . -mtime -7 -type f
来源：http://read.share.tarul.cn/Article/details/gnwgxuwwq.sHtML

[R45] 批量删除
来源：http://www.share.tarul.cn/Article/details/gyqyruxub.sHtML

find . -name "*.tmp" -delete
来源：http://wap.sjlbkw.cn/Article/details/gfwcjgtxq.sHtML

[R46] 递归替换文件内容
来源：http://blog.sjlbkw.cn/Article/details/gkyyfexww.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fktsv.cn/Article/details/giqisbmhb.sHtML

[R47] sed 单行替换
来源：http://m.share.fktsv.cn/Article/details/gtqzzedae.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.sjlbkw.cn/Article/details/gkdgbtqil.sHtML

[R48] awk 取指定列
来源：http://3g.sjlbkw.cn/Article/details/grirmaykr.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.vehdjk.com/Article/details/gfttpzvtc.sHtML

[R49] awk 带条件
来源：http://wap.yfazqb.com/Article/details/gzkwaatfe.sHtML


<!-- 参考信息 -->