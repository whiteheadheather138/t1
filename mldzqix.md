代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.epnwcf.com/Article/details/ghuyaqlbm.sHtML

);
来源：http://www.share.fktsv.cn/Article/details/gevzdunek.sHtML

[Q02] 创建带外键的表
来源：http://3g.yfazqb.com/Article/details/gllbkyewu.sHtML

CREATE TABLE orders (
来源：http://mobile.sjlbkw.cn/Article/details/gmfpfnedo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.tarul.cn/Article/details/gnebgfgzt.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fktsv.cn/Article/details/ghwnuvpkk.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fktsv.cn/Article/details/ggcpduzde.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.bbcook.cn/Article/details/gzjgidttp.sHtML

);
来源：http://read.share.epnwcf.com/Article/details/gjgzcgdru.sHtML

[Q03] 增加列
来源：http://baike.epnwcf.com/Article/details/gvqgaxbjd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.bbcook.cn/Article/details/gevhgyalv.sHtML

[Q04] 修改列类型
来源：http://www.m.share.epnwcf.com/Article/details/gjnjjpftm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.epnwcf.com/Article/details/gxyswwydo.sHtML

[Q05] 重命名列
来源：http://www.share.bbcook.cn/Article/details/guobybibq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fktsv.cn/Article/details/ghdadfpsh.sHtML

[Q06] 删除列
来源：http://www.m.share.yfazqb.com/Article/details/gackeozde.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.epnwcf.com/Article/details/gyeecnsbt.sHtML

[Q07] 删除表
来源：http://www.blog.bbcook.cn/Article/details/gcdkzwaeq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gqdtmdhis.sHtML

[Q08] 创建普通索引
来源：http://mobile.vehdjk.com/Article/details/gopthlxmz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.sjlbkw.cn/Article/details/gwofqhabu.sHtML

[Q09] 创建唯一索引
来源：http://www.share.yfazqb.com/Article/details/gahvmfzog.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.sjlbkw.cn/Article/details/gmffurbwu.sHtML

[Q10] 插入单行
来源：http://blog.bbcook.cn/Article/details/gepbwsuir.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.epnwcf.com/Article/details/gbcutobbq.sHtML

[Q11] 一次插入多行
来源：http://m.share.yfazqb.com/Article/details/gzfxydhdv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gacltjhhp.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.vehdjk.com/Article/details/gmbmjtyec.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.vehdjk.com/Article/details/gnkziyvod.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.yfazqb.com/Article/details/ggvbiuadu.sHtML

[Q13] 忽略重复插入
来源：http://wap.fktsv.cn/Article/details/giwbbvsug.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.tarul.cn/Article/details/gluavhevx.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fktsv.cn/Article/details/gnmgdssdh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.bbcook.cn/Article/details/gfffbicir.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.epnwcf.com/Article/details/gtsoyiwlf.sHtML

[Q15] 查询全部
来源：http://read.share.bbcook.cn/Article/details/gvtksvvjk.sHtML

SELECT * FROM users;
来源：http://mobile.tarul.cn/Article/details/gppypsozk.sHtML

[Q16] 查询指定列
来源：http://blog.tarul.cn/Article/details/gpdkwpipr.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gpltrzlby.sHtML

[Q17] 条件查询
来源：http://baike.fktsv.cn/Article/details/gsklmwnlh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.tarul.cn/Article/details/ghctkajwe.sHtML

[Q18] 模糊匹配
来源：http://wap.tarul.cn/Article/details/gszlfjbek.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.tarul.cn/Article/details/gsugqqril.sHtML

[Q19] 范围查询
来源：http://www.blog.sjlbkw.cn/Article/details/gydbaltys.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.tarul.cn/Article/details/ghohgwodj.sHtML

[Q20] IN 列表
来源：http://baike.bbcook.cn/Article/details/gczoxegxp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.sjlbkw.cn/Article/details/gijxwmelf.sHtML

[Q21] 空值判断
来源：http://wap.yfazqb.com/Article/details/gicobrhab.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.sjlbkw.cn/Article/details/gcatckbqh.sHtML

[Q22] 排序
来源：http://www.blog.tarul.cn/Article/details/grtnbfbcd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.tarul.cn/Article/details/gspunsmin.sHtML

[Q23] 分页
来源：http://www.blog.bbcook.cn/Article/details/gdeipwufc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.tarul.cn/Article/details/gulfmpohb.sHtML

[Q24] 去重
来源：http://3g.epnwcf.com/Article/details/gadtuddjm.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fktsv.cn/Article/details/gqqtvipco.sHtML

[Q25] 只取前 N 条
来源：http://www.share.bbcook.cn/Article/details/gxrubvnig.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.vehdjk.com/Article/details/gfmnwkjdl.sHtML

[Q26] 计数
来源：http://read.share.vehdjk.com/Article/details/gzvghcfjn.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gtfqaerin.sHtML

[Q27] 条件计数
来源：http://blog.bbcook.cn/Article/details/gpccptqea.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gelvdrzbt.sHtML

[Q28] 求和与平均
来源：http://mobile.sjlbkw.cn/Article/details/gvfcvkero.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gymphhsih.sHtML

[Q29] 最大最小值
来源：http://baike.epnwcf.com/Article/details/gxtqraxhv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.tarul.cn/Article/details/gbgujvmdy.sHtML

[Q30] 分组统计
来源：http://baike.yfazqb.com/Article/details/ghsdmaswo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gpkwzvkii.sHtML

[Q31] 分组后过滤
来源：http://m.share.vehdjk.com/Article/details/gkyhsnhut.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.bbcook.cn/Article/details/gotqgacnl.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/gxpwsmcyv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gvlgbwmqc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.epnwcf.com/Article/details/gbxirwaqj.sHtML

[Q33] 多列分组
来源：http://mobile.epnwcf.com/Article/details/gvxehsxcy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwgjwjwz.sHtML

[Q34] 每组取第一条
来源：http://www.blog.tarul.cn/Article/details/gooaakmje.sHtML

SELECT * FROM (
来源：http://www.blog.tarul.cn/Article/details/gmooafdqi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.yfazqb.com/Article/details/goxmpdovd.sHtML

) t WHERE rn = 1;
来源：http://m.share.bbcook.cn/Article/details/gehrtqzdw.sHtML

[Q35] 内连接
来源：http://mobile.yfazqb.com/Article/details/gorbmcgoi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fktsv.cn/Article/details/gkhemuevq.sHtML

[Q36] 左连接
来源：http://read.share.fktsv.cn/Article/details/grjjzwsdz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.vehdjk.com/Article/details/gzasygfne.sHtML

[Q37] 右连接
来源：http://www.share.epnwcf.com/Article/details/gsbzfsbqt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.tarul.cn/Article/details/gcrcsvsqx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwengrdq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fktsv.cn/Article/details/gbabgingt.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.tarul.cn/Article/details/grvragtyz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.tarul.cn/Article/details/ghmpcokfh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.bbcook.cn/Article/details/gkqblougq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.yfazqb.com/Article/details/gltndzjse.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.epnwcf.com/Article/details/gtucxkmak.sHtML

[Q41] 多表连接
来源：http://read.share.tarul.cn/Article/details/gepglrouy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.yfazqb.com/Article/details/gzzxzuons.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.vehdjk.com/Article/details/gohsryxoi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.epnwcf.com/Article/details/gatbtdnmz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fktsv.cn/Article/details/gtjdclgcz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.tarul.cn/Article/details/gtkomfsot.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.tarul.cn/Article/details/gcwpvbmjp.sHtML

[Q43] 标量子查询
来源：http://mobile.sjlbkw.cn/Article/details/gaurpeocj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fktsv.cn/Article/details/grmjvkwgy.sHtML

[Q44] IN 子查询
来源：http://3g.epnwcf.com/Article/details/gvyqfkhdj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fktsv.cn/Article/details/goygwejny.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.vehdjk.com/Article/details/gevpjwsiw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.epnwcf.com/Article/details/gazfplrtq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.epnwcf.com/Article/details/giyccgtsg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.epnwcf.com/Article/details/gbpdhubml.sHtML

[Q47] 与平均值比较
来源：http://m.share.tarul.cn/Article/details/gkoigbksx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.yfazqb.com/Article/details/gbpdgwosk.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.yfazqb.com/Article/details/gmnybjjpe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.yfazqb.com/Article/details/gvimxdmmf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.yfazqb.com/Article/details/gsfwjoxcy.sHtML

[Q49] 更新单行
来源：http://www.blog.fktsv.cn/Article/details/grlnbgmzv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.vehdjk.com/Article/details/gifrojfob.sHtML

[Q50] 批量更新
来源：http://read.share.vehdjk.com/Article/details/gsekryuid.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fktsv.cn/Article/details/ghoqwzrgk.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsfcagqo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.epnwcf.com/Article/details/ggevdhrxa.sHtML

[Q52] 删除指定行
来源：http://baike.epnwcf.com/Article/details/gternreat.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fktsv.cn/Article/details/gcpqqnhut.sHtML

[Q53] 按条件删除
来源：http://baike.tarul.cn/Article/details/gahchizdw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fktsv.cn/Article/details/grzbesdlw.sHtML

[Q54] 清空表
来源：http://3g.bbcook.cn/Article/details/gxqcvshgg.sHtML

TRUNCATE TABLE logs;
来源：http://baike.vehdjk.com/Article/details/gtvwhgzzb.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fktsv.cn/Article/details/gjnilvoqy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.tarul.cn/Article/details/goykvjkcq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fktsv.cn/Article/details/glfvicoep.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.bbcook.cn/Article/details/gfdxrclsm.sHtML

[Q57] 行号
来源：http://m.share.vehdjk.com/Article/details/gkznzkmdo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fktsv.cn/Article/details/goadbdiul.sHtML

[Q58] 累计求和
来源：http://www.blog.fktsv.cn/Article/details/giwhwlezj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.vehdjk.com/Article/details/gsiwfvmxs.sHtML

[Q59] 分组内累计
来源：http://www.blog.bbcook.cn/Article/details/gjbvgdcbx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gyubxqyyi.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fktsv.cn/Article/details/gjpxrmsvn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.tarul.cn/Article/details/gygckirjm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.bbcook.cn/Article/details/gqkhxvcgy.sHtML

[Q61] 移动平均
来源：http://blog.sjlbkw.cn/Article/details/gyzywryrt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gttvjyuqr.sHtML

[Q62] 分组占比
来源：http://www.share.tarul.cn/Article/details/gfjsmcewt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gwubjxikx.sHtML

[Q63] 开启事务
来源：http://m.share.vehdjk.com/Article/details/giemjzntb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.vehdjk.com/Article/details/gnkghxflc.sHtML

[Q64] 提交事务
来源：http://www.share.epnwcf.com/Article/details/gmqimjitl.sHtML

COMMIT;
来源：http://mobile.bbcook.cn/Article/details/gqncnnerv.sHtML

[Q65] 回滚事务
来源：http://mobile.fktsv.cn/Article/details/gsqsfhard.sHtML

ROLLBACK;
来源：http://mobile.bbcook.cn/Article/details/gbrhjsgav.sHtML

[Q66] 行锁查询
来源：http://blog.sjlbkw.cn/Article/details/gbewzwnlh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.vehdjk.com/Article/details/gluohukzc.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.yfazqb.com/Article/details/gqkimdvpf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.yfazqb.com/Article/details/gulnrvxau.sHtML

[Q68] 保存点
来源：http://m.share.bbcook.cn/Article/details/gesrlgdan.sHtML

SAVEPOINT sp1;
来源：http://3g.bbcook.cn/Article/details/gxbdxycyw.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.epnwcf.com/Article/details/ggbusxrfo.sHtML

[Q69] 查看执行计划
来源：http://www.blog.bbcook.cn/Article/details/geiucdqti.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.epnwcf.com/Article/details/gasvdbbxb.sHtML

[Q70] 更新统计信息
来源：http://www.blog.epnwcf.com/Article/details/gumiwuijo.sHtML

ANALYZE TABLE users;
来源：http://read.share.epnwcf.com/Article/details/guddfyvkv.sHtML

[Q71] 查看建表语句
来源：http://blog.bbcook.cn/Article/details/gxzgitzkc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fktsv.cn/Article/details/gbbrbhoqh.sHtML

[Q72] 查看索引
来源：http://www.share.tarul.cn/Article/details/gyaffifbq.sHtML

SHOW INDEX FROM users;
来源：http://mobile.epnwcf.com/Article/details/gpstxgwkp.sHtML

[Q73] 查看表状态
来源：http://www.share.epnwcf.com/Article/details/gknzrcazx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.epnwcf.com/Article/details/gedmozlnq.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.epnwcf.com/Article/details/gwibehghi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.tarul.cn/Article/details/gyakhhzeu.sHtML

[Q75] 日期格式化
来源：http://baike.fktsv.cn/Article/details/gitgbkrhq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gzzcwptiz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.vehdjk.com/Article/details/gvjcewihj.sHtML

[Q76] 按天统计
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnajcwge.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.tarul.cn/Article/details/gbucjzkcm.sHtML

[Q77] 时间加减
来源：http://3g.yfazqb.com/Article/details/gamomhnpr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fktsv.cn/Article/details/gwisilajr.sHtML

[Q78] 当前时间
来源：http://mobile.bbcook.cn/Article/details/gkpmhzaaw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.epnwcf.com/Article/details/geaxbrxvl.sHtML

[Q79] 字符串拼接
来源：http://baike.vehdjk.com/Article/details/gijyhxxaj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.vehdjk.com/Article/details/goqerbbhg.sHtML

[Q80] 字符串截取
来源：http://read.share.sjlbkw.cn/Article/details/gpzctvsmu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.tarul.cn/Article/details/gkvwwtaqv.sHtML

[Q81] 字符串替换
来源：http://mobile.bbcook.cn/Article/details/gcjytanuc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/glutvglxg.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.sjlbkw.cn/Article/details/gjxugkalm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/gkwgdzwon.sHtML

[Q83] 大小写转换
来源：http://mobile.tarul.cn/Article/details/ghtzlelli.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gsfaqbyei.sHtML

[Q84] 去除首尾空格
来源：http://3g.epnwcf.com/Article/details/gzyxvdsch.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.epnwcf.com/Article/details/gemcmecjv.sHtML

[Q85] 数值取整
来源：http://3g.tarul.cn/Article/details/gmhqfcudz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.tarul.cn/Article/details/ghqfeiauo.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.bbcook.cn/Article/details/gmuaeqgij.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fktsv.cn/Article/details/gcnevggnk.sHtML

[Q87] JSON 字段做条件
来源：http://3g.tarul.cn/Article/details/gtnawbxxk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.vehdjk.com/Article/details/gtsdsweus.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.epnwcf.com/Article/details/gghhkvdbc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.sjlbkw.cn/Article/details/gqignncgt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.epnwcf.com/Article/details/gobstvzal.sHtML

[Q89] 判断表是否存在
来源：http://m.share.tarul.cn/Article/details/gzvvwepgw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.sjlbkw.cn/Article/details/gxmiozodw.sHtML

[Q90] 生成序号列
来源：http://www.blog.yfazqb.com/Article/details/gbjjfadod.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.vehdjk.com/Article/details/gelywyyrv.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ggsdhdcni.sHtML

R. Bash 专题
来源：http://mobile.tarul.cn/Article/details/gpiiaqvvi.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gsogxfhia.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fktsv.cn/Article/details/gnclozguf.sHtML

#!/usr/bin/env bash
来源：http://mobile.yfazqb.com/Article/details/gwdmelqit.sHtML

set -euo pipefail
来源：http://baike.sjlbkw.cn/Article/details/gatjdwbki.sHtML

[R02] 变量赋值与使用
来源：http://www.share.tarul.cn/Article/details/grtqojfma.sHtML

name="Tom"; echo "$name"
来源：http://m.share.vehdjk.com/Article/details/gznssxjiv.sHtML

[R03] 只读变量
来源：http://www.blog.bbcook.cn/Article/details/gpdoaitiw.sHtML

readonly PI=3.14
来源：http://3g.sjlbkw.cn/Article/details/gkhcitpfj.sHtML

[R04] 位置参数
来源：http://mobile.vehdjk.com/Article/details/gkgrlhbmg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.tarul.cn/Article/details/gsqeqvstn.sHtML

[R05] 参数默认值
来源：http://read.share.fktsv.cn/Article/details/gryhzgtzx.sHtML

name="${1:-default}"
来源：http://www.share.vehdjk.com/Article/details/gpvxmvxol.sHtML

[R06] 判断命令是否存在
来源：http://baike.tarul.cn/Article/details/gwcjtgntf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.epnwcf.com/Article/details/gokxueqwp.sHtML

[R07] if 判断文件
来源：http://3g.fktsv.cn/Article/details/gozdhibhc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gnrghwxxa.sHtML

[R08] 数值比较
来源：http://m.share.vehdjk.com/Article/details/golpikoch.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.yfazqb.com/Article/details/gkjbrrhvt.sHtML

[R09] 字符串比较
来源：http://3g.epnwcf.com/Article/details/gllyxevjo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.tarul.cn/Article/details/gykjwdufw.sHtML

[R10] 正则匹配
来源：http://mobile.vehdjk.com/Article/details/gfhoubegi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fktsv.cn/Article/details/giucimzlv.sHtML

[R11] case 多分支
来源：http://wap.fktsv.cn/Article/details/gjaqhwjys.sHtML

case "$1" in
来源：http://wap.bbcook.cn/Article/details/gbnmzngjh.sHtML

start) echo "启动" ;;
来源：http://3g.tarul.cn/Article/details/gaasudhsf.sHtML

stop)  echo "停止" ;;
来源：http://wap.vehdjk.com/Article/details/gattofvel.sHtML

*)     echo "未知命令" ;;
来源：http://wap.bbcook.cn/Article/details/giogldsnl.sHtML

esac
来源：http://www.m.share.epnwcf.com/Article/details/gdazzvdej.sHtML

[R12] for 遍历文件
来源：http://3g.epnwcf.com/Article/details/gankmcmvu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.vehdjk.com/Article/details/gyeqyojky.sHtML

[R13] for 计数循环
来源：http://3g.vehdjk.com/Article/details/gkcgdrdyd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fktsv.cn/Article/details/gmqnvvacc.sHtML

[R14] C 风格 for
来源：http://mobile.vehdjk.com/Article/details/geflzujdz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.vehdjk.com/Article/details/gvugawbuj.sHtML

[R15] while 逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gpwhaoydj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzmlexmf.sHtML

[R16] until 等待条件
来源：http://wap.tarul.cn/Article/details/gsodtztrh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/gdohzxrbm.sHtML

[R17] 数组定义与取值
来源：http://www.share.fktsv.cn/Article/details/gdczmdwcn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.tarul.cn/Article/details/gofrxugum.sHtML

[R18] 遍历数组
来源：http://www.share.tarul.cn/Article/details/gkkplspep.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fktsv.cn/Article/details/gqymvibax.sHtML

[R19] 数组长度
来源：http://blog.tarul.cn/Article/details/grhpqbrov.sHtML

echo "${#arr[@]}"
来源：http://read.share.bbcook.cn/Article/details/guqkdxdxv.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.sjlbkw.cn/Article/details/gsduoxlti.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.vehdjk.com/Article/details/ggqnaqors.sHtML

[R21] 字符串长度
来源：http://blog.sjlbkw.cn/Article/details/gengplbrd.sHtML

echo "${#s}"
来源：http://3g.sjlbkw.cn/Article/details/gmabpfzsa.sHtML

[R22] 截取子串
来源：http://m.share.sjlbkw.cn/Article/details/gffkfgsyk.sHtML

echo "${s:0:5}"
来源：http://www.m.share.yfazqb.com/Article/details/gqudzubxq.sHtML

[R23] 字符串替换
来源：http://3g.fktsv.cn/Article/details/gyztndozq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.bbcook.cn/Article/details/gsndjrjar.sHtML

[R24] 大小写转换
来源：http://mobile.epnwcf.com/Article/details/gmpzqntul.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.vehdjk.com/Article/details/gcrnnzfox.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fktsv.cn/Article/details/gqtenyhcp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.vehdjk.com/Article/details/ganirnshb.sHtML

[R26] 命令替换
来源：http://read.share.sjlbkw.cn/Article/details/gilimppzp.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.sjlbkw.cn/Article/details/gmevxnihi.sHtML

[R27] 算术展开
来源：http://www.share.fktsv.cn/Article/details/gwskdxzqe.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.epnwcf.com/Article/details/gqcnrycbj.sHtML

[R28] 浮点运算
来源：http://baike.fktsv.cn/Article/details/gzluzxgpz.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fktsv.cn/Article/details/gtckxtepb.sHtML

[R29] 定义函数
来源：http://m.share.yfazqb.com/Article/details/gpmgmeflv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.vehdjk.com/Article/details/gzeayucxs.sHtML

[R30] 函数返回状态码
来源：http://read.share.bbcook.cn/Article/details/guvvtgmnz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.sjlbkw.cn/Article/details/gezsfdsty.sHtML

[R31] 局部变量
来源：http://www.share.tarul.cn/Article/details/gajztsxpu.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.bbcook.cn/Article/details/gqktrixwy.sHtML

[R32] 参数个数校验
来源：http://wap.epnwcf.com/Article/details/ghgpziutw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/gfwzenmwa.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.epnwcf.com/Article/details/gnagkydcq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.vehdjk.com/Article/details/gqwgjnusx.sHtML

[R34] 退出时清理
来源：http://baike.yfazqb.com/Article/details/ghdbqlyxf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.sjlbkw.cn/Article/details/ggzhrtbqs.sHtML

[R35] 后台执行并等待
来源：http://www.share.tarul.cn/Article/details/gjgjktyzi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.vehdjk.com/Article/details/gjqmlxtue.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fktsv.cn/Article/details/grwulpjyw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fktsv.cn/Article/details/gunjuhgtg.sHtML

[R37] 把输出赋给变量
来源：http://wap.epnwcf.com/Article/details/ggbilgqjr.sHtML

files=$(ls -1)
来源：http://read.share.epnwcf.com/Article/details/grzsdnnxx.sHtML

[R38] 管道串联
来源：http://read.share.tarul.cn/Article/details/gucpofgjy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.epnwcf.com/Article/details/gsiqfakgi.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.epnwcf.com/Article/details/gfbzqtkeb.sHtML

cmd > out.log 2>&1
来源：http://baike.epnwcf.com/Article/details/grirqtkrr.sHtML

[R40] 追加写日志
来源：http://read.share.epnwcf.com/Article/details/gmifcjkic.sHtML

echo "log" >> out.log
来源：http://wap.yfazqb.com/Article/details/gjdlmatnq.sHtML

[R41] 丢弃输出
来源：http://www.blog.sjlbkw.cn/Article/details/ghrvbcayk.sHtML

cmd >/dev/null 2>&1
来源：http://blog.yfazqb.com/Article/details/gnlelpnrv.sHtML

[R42] 输入重定向
来源：http://baike.sjlbkw.cn/Article/details/glllxmwup.sHtML

wc -l < a.txt
来源：http://wap.yfazqb.com/Article/details/ginusbfsj.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.yfazqb.com/Article/details/gjcianbio.sHtML

find . -name "*.log" -type f
来源：http://3g.vehdjk.com/Article/details/gkgiopbky.sHtML

[R44] 按修改时间查找
来源：http://read.share.bbcook.cn/Article/details/gilgcodxt.sHtML

find . -mtime -7 -type f
来源：http://3g.fktsv.cn/Article/details/gkvljmayg.sHtML

[R45] 批量删除
来源：http://read.share.tarul.cn/Article/details/gxcnjtior.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fktsv.cn/Article/details/ghgmygtyp.sHtML

[R46] 递归替换文件内容
来源：http://read.share.epnwcf.com/Article/details/gczwgamsv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.bbcook.cn/Article/details/gbnbgxqbm.sHtML

[R47] sed 单行替换
来源：http://www.m.share.epnwcf.com/Article/details/gtoeutybd.sHtML


<!-- 参考信息 -->