代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://read.share.fktsv.cn/Article/details/ggdlrofdn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fktsv.cn/Article/details/gnvrgwkia.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.epnwcf.com/Article/details/gmzgfvaib.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.yfazqb.com/Article/details/gzhkdqngc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/gkzikkwjs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.bbcook.cn/Article/details/ghytfiubd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gbiwizkns.sHtML

Ruby: a == b
来源：http://m.share.vehdjk.com/Article/details/gluljkabr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.vehdjk.com/Article/details/gzcyuisqd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.sjlbkw.cn/Article/details/ganrkikif.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.yfazqb.com/Article/details/gfyhwroak.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.epnwcf.com/Article/details/gdggwfywd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.bbcook.cn/Article/details/gznhbznuv.sHtML

TS:   if (x == null) {}
来源：http://www.blog.yfazqb.com/Article/details/gilndngom.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.sjlbkw.cn/Article/details/gpkmjhldo.sHtML

Go:   if x == nil {}
来源：http://www.share.bbcook.cn/Article/details/gmaydxkur.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.vehdjk.com/Article/details/gkiilrudx.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.bbcook.cn/Article/details/gemeqallk.sHtML

[P07] 防抖与节流
来源：http://www.blog.tarul.cn/Article/details/gdcjvoaay.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fktsv.cn/Article/details/gfhpsfeti.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.yfazqb.com/Article/details/gwghlpotr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.epnwcf.com/Article/details/gtciplocm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/ghuxcknzf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.yfazqb.com/Article/details/gglprrczv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.sjlbkw.cn/Article/details/giijusghf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.tarul.cn/Article/details/galpgllta.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.sjlbkw.cn/Article/details/gurqchlae.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.sjlbkw.cn/Article/details/gkrgqfoar.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.yfazqb.com/Article/details/gzjheyryj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.yfazqb.com/Article/details/gejspyxsp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.bbcook.cn/Article/details/gnexntfbi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.yfazqb.com/Article/details/geoadvsyg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.sjlbkw.cn/Article/details/gzxqyqnyi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.bbcook.cn/Article/details/gdepzszly.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fktsv.cn/Article/details/gcxlppack.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.vehdjk.com/Article/details/gangckkbw.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gmpxxxhan.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.tarul.cn/Article/details/gkgeadrda.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gwoteusiw.sHtML

[Q01] 创建表
来源：http://read.share.yfazqb.com/Article/details/gwbxwaksd.sHtML

CREATE TABLE users (
来源：http://read.share.yfazqb.com/Article/details/gmxnaiktf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.vehdjk.com/Article/details/gygpmyrcj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fktsv.cn/Article/details/gcjqbbvdi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.sjlbkw.cn/Article/details/gknhnenqt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.sjlbkw.cn/Article/details/gabripwyd.sHtML

);
来源：http://m.share.bbcook.cn/Article/details/glcdurswl.sHtML

[Q02] 创建带外键的表
来源：http://m.share.tarul.cn/Article/details/gyhylthlf.sHtML

CREATE TABLE orders (
来源：http://www.share.fktsv.cn/Article/details/gfvzyuvnh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/gzwpxyjwf.sHtML

user_id INT NOT NULL,
来源：http://mobile.epnwcf.com/Article/details/gavxosyug.sHtML

amount DECIMAL(10, 2),
来源：http://wap.sjlbkw.cn/Article/details/gsxlvdztj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.bbcook.cn/Article/details/gxawmnfey.sHtML

);
来源：http://read.share.epnwcf.com/Article/details/gmwkrlxus.sHtML

[Q03] 增加列
来源：http://3g.tarul.cn/Article/details/gzxdmvwdx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.bbcook.cn/Article/details/gjolfjsrv.sHtML

[Q04] 修改列类型
来源：http://blog.yfazqb.com/Article/details/gzwqgbeak.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.sjlbkw.cn/Article/details/gcxurhuka.sHtML

[Q05] 重命名列
来源：http://m.share.sjlbkw.cn/Article/details/gzfatxbnw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.bbcook.cn/Article/details/gjftfqypo.sHtML

[Q06] 删除列
来源：http://read.share.fktsv.cn/Article/details/gwygmjykh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.yfazqb.com/Article/details/gfnqwbwrr.sHtML

[Q07] 删除表
来源：http://www.blog.vehdjk.com/Article/details/gqpvhlhvp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.epnwcf.com/Article/details/ggvcyjigw.sHtML

[Q08] 创建普通索引
来源：http://baike.fktsv.cn/Article/details/gdhrogjsg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.epnwcf.com/Article/details/gepkouqtf.sHtML

[Q09] 创建唯一索引
来源：http://m.share.sjlbkw.cn/Article/details/goynuojfh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.yfazqb.com/Article/details/goygdpdsq.sHtML

[Q10] 插入单行
来源：http://wap.sjlbkw.cn/Article/details/gdlflgzkg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.sjlbkw.cn/Article/details/gluotzqim.sHtML

[Q11] 一次插入多行
来源：http://baike.bbcook.cn/Article/details/gwpwkxlkh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.sjlbkw.cn/Article/details/geaxtyaoj.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.bbcook.cn/Article/details/goeyflsos.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.yfazqb.com/Article/details/gtzevfkkk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.tarul.cn/Article/details/gzoglkukg.sHtML

[Q13] 忽略重复插入
来源：http://m.share.bbcook.cn/Article/details/gzhoqrpga.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.yfazqb.com/Article/details/gvwwvrdrs.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.sjlbkw.cn/Article/details/gaeqgneqc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.epnwcf.com/Article/details/gnqjhyoow.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.bbcook.cn/Article/details/gigpqkrps.sHtML

[Q15] 查询全部
来源：http://3g.bbcook.cn/Article/details/gsiesuoak.sHtML

SELECT * FROM users;
来源：http://3g.fktsv.cn/Article/details/glebhnndf.sHtML

[Q16] 查询指定列
来源：http://www.blog.bbcook.cn/Article/details/grhwbfuud.sHtML

SELECT id, name FROM users;
来源：http://wap.vehdjk.com/Article/details/gynjkvbys.sHtML

[Q17] 条件查询
来源：http://www.m.share.tarul.cn/Article/details/gshnexyts.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.tarul.cn/Article/details/gdobkjmha.sHtML

[Q18] 模糊匹配
来源：http://baike.bbcook.cn/Article/details/grhjlnbfm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.vehdjk.com/Article/details/gwqxnyzyy.sHtML

[Q19] 范围查询
来源：http://mobile.bbcook.cn/Article/details/gvnlqanyn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.bbcook.cn/Article/details/gpgxskqxt.sHtML

[Q20] IN 列表
来源：http://mobile.epnwcf.com/Article/details/geliubixe.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.tarul.cn/Article/details/guleuygrh.sHtML

[Q21] 空值判断
来源：http://baike.epnwcf.com/Article/details/gldtmzaod.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghewijred.sHtML

[Q22] 排序
来源：http://read.share.tarul.cn/Article/details/gpuohamld.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.yfazqb.com/Article/details/gglaaxwmr.sHtML

[Q23] 分页
来源：http://wap.vehdjk.com/Article/details/gfdjbpubn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.bbcook.cn/Article/details/gtochjhst.sHtML

[Q24] 去重
来源：http://read.share.vehdjk.com/Article/details/gbpivzfrc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gjsjxyqbq.sHtML

[Q25] 只取前 N 条
来源：http://m.share.epnwcf.com/Article/details/gdbordyec.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.tarul.cn/Article/details/grsucmmuz.sHtML

[Q26] 计数
来源：http://m.share.vehdjk.com/Article/details/glbkxyjps.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gxfwuqjrc.sHtML

[Q27] 条件计数
来源：http://m.share.bbcook.cn/Article/details/gbnqrxspe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.yfazqb.com/Article/details/gjsvxeven.sHtML

[Q28] 求和与平均
来源：http://wap.fktsv.cn/Article/details/gvkhqztbz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fktsv.cn/Article/details/ghckmmntb.sHtML

[Q29] 最大最小值
来源：http://mobile.sjlbkw.cn/Article/details/gutbmtnbb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.tarul.cn/Article/details/ghmbtznth.sHtML

[Q30] 分组统计
来源：http://m.share.vehdjk.com/Article/details/gaxyvlgey.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gvdodmfpm.sHtML

[Q31] 分组后过滤
来源：http://3g.fktsv.cn/Article/details/gqqoedpza.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.bbcook.cn/Article/details/gsoqasahh.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gdbnpmggw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/gordkvaoz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fktsv.cn/Article/details/ggujsbmne.sHtML

[Q33] 多列分组
来源：http://www.blog.tarul.cn/Article/details/gtllggrwi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.bbcook.cn/Article/details/glkevsehm.sHtML

[Q34] 每组取第一条
来源：http://baike.tarul.cn/Article/details/gqsggckzf.sHtML

SELECT * FROM (
来源：http://3g.fktsv.cn/Article/details/gkbriisqn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.tarul.cn/Article/details/gonljnqgv.sHtML

) t WHERE rn = 1;
来源：http://baike.sjlbkw.cn/Article/details/gsvwgyavh.sHtML

[Q35] 内连接
来源：http://mobile.fktsv.cn/Article/details/gqeudehba.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.bbcook.cn/Article/details/gdgwbzsbh.sHtML

[Q36] 左连接
来源：http://blog.fktsv.cn/Article/details/gaexznsfr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.epnwcf.com/Article/details/gohqczuqa.sHtML

[Q37] 右连接
来源：http://m.share.yfazqb.com/Article/details/gilqtkbie.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.epnwcf.com/Article/details/gehetktmy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.bbcook.cn/Article/details/gsklzegdw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fktsv.cn/Article/details/gvoczcgon.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.yfazqb.com/Article/details/gvjnsgncz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.tarul.cn/Article/details/gvjdykbww.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.vehdjk.com/Article/details/gkgzfogon.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.sjlbkw.cn/Article/details/gyloztuhc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fktsv.cn/Article/details/gcjimmlex.sHtML

[Q41] 多表连接
来源：http://www.share.vehdjk.com/Article/details/gemncepuj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.sjlbkw.cn/Article/details/gaijftarv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fktsv.cn/Article/details/gqmhqoqyn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.tarul.cn/Article/details/ggcwwxgpy.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.sjlbkw.cn/Article/details/gtzqcgrua.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.epnwcf.com/Article/details/gmhfvwqhe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.sjlbkw.cn/Article/details/glybfzniy.sHtML

[Q43] 标量子查询
来源：http://www.share.vehdjk.com/Article/details/gbxqjyino.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.vehdjk.com/Article/details/gyqfutcnv.sHtML

[Q44] IN 子查询
来源：http://blog.sjlbkw.cn/Article/details/gcjauelal.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.vehdjk.com/Article/details/gqkajwyyd.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.tarul.cn/Article/details/glmgeiyhw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.bbcook.cn/Article/details/gtnplvacu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.yfazqb.com/Article/details/gqldyvtjl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.sjlbkw.cn/Article/details/guvfbsxow.sHtML

[Q47] 与平均值比较
来源：http://m.share.sjlbkw.cn/Article/details/gvblndgjl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fktsv.cn/Article/details/gxqxekwkf.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.epnwcf.com/Article/details/gjcudumth.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.vehdjk.com/Article/details/gkcsjyent.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.vehdjk.com/Article/details/gljwwaber.sHtML

[Q49] 更新单行
来源：http://www.m.share.bbcook.cn/Article/details/gswnzncia.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.sjlbkw.cn/Article/details/geuauecko.sHtML

[Q50] 批量更新
来源：http://wap.vehdjk.com/Article/details/gtvwqlpgx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.tarul.cn/Article/details/gehiynoxi.sHtML

[Q51] 用子查询更新
来源：http://blog.yfazqb.com/Article/details/gjuccbzqv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fktsv.cn/Article/details/gdbqhkfjs.sHtML

[Q52] 删除指定行
来源：http://baike.yfazqb.com/Article/details/gihzxdfkn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.bbcook.cn/Article/details/gkeauizhh.sHtML

[Q53] 按条件删除
来源：http://wap.epnwcf.com/Article/details/gyjmxrbxj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fktsv.cn/Article/details/gsxsegffu.sHtML

[Q54] 清空表
来源：http://baike.sjlbkw.cn/Article/details/gaxsgadec.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.sjlbkw.cn/Article/details/gfwqcdlrk.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.sjlbkw.cn/Article/details/gwijzclwa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.yfazqb.com/Article/details/glocbdutg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fktsv.cn/Article/details/gmqjcphwu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.bbcook.cn/Article/details/gwvfzhmwr.sHtML

[Q57] 行号
来源：http://www.blog.tarul.cn/Article/details/gbrglbgif.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gbajnkswh.sHtML

[Q58] 累计求和
来源：http://read.share.epnwcf.com/Article/details/gevbyibhe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/grlbpceqa.sHtML

[Q59] 分组内累计
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqipetwc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/grvybyidv.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.epnwcf.com/Article/details/gxzvapqri.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.epnwcf.com/Article/details/gykukwbxi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.bbcook.cn/Article/details/gseiovcew.sHtML

[Q61] 移动平均
来源：http://www.m.share.bbcook.cn/Article/details/glnjoalbg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.tarul.cn/Article/details/grsqbzgvn.sHtML

[Q62] 分组占比
来源：http://mobile.epnwcf.com/Article/details/gkjopyqbg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/guwheywwz.sHtML

[Q63] 开启事务
来源：http://www.share.bbcook.cn/Article/details/gfvvdpfzr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.vehdjk.com/Article/details/gelireznw.sHtML

[Q64] 提交事务
来源：http://m.share.sjlbkw.cn/Article/details/gqdnqgfye.sHtML

COMMIT;
来源：http://3g.epnwcf.com/Article/details/gqhiafxco.sHtML

[Q65] 回滚事务
来源：http://www.share.tarul.cn/Article/details/gxouirdlz.sHtML

ROLLBACK;
来源：http://m.share.yfazqb.com/Article/details/gvftsirhk.sHtML

[Q66] 行锁查询
来源：http://read.share.yfazqb.com/Article/details/gsxpvnwnj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.yfazqb.com/Article/details/gggqzjrgh.sHtML

[Q67] 设置隔离级别
来源：http://read.share.bbcook.cn/Article/details/gttapfetu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.bbcook.cn/Article/details/gpqelkyvd.sHtML

[Q68] 保存点
来源：http://baike.fktsv.cn/Article/details/gohfktjya.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.vehdjk.com/Article/details/grzmsryau.sHtML

ROLLBACK TO sp1;
来源：http://read.share.yfazqb.com/Article/details/gnszklffp.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fktsv.cn/Article/details/gldrvnpmb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.sjlbkw.cn/Article/details/gakpygatw.sHtML

[Q70] 更新统计信息
来源：http://m.share.sjlbkw.cn/Article/details/gxiyexizj.sHtML

ANALYZE TABLE users;
来源：http://mobile.bbcook.cn/Article/details/gnosgnghv.sHtML

[Q71] 查看建表语句
来源：http://www.share.yfazqb.com/Article/details/gusgbuooz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.bbcook.cn/Article/details/gvjmscopj.sHtML

[Q72] 查看索引
来源：http://blog.yfazqb.com/Article/details/gocazgnkf.sHtML

SHOW INDEX FROM users;
来源：http://blog.vehdjk.com/Article/details/gfnsctknu.sHtML

[Q73] 查看表状态
来源：http://read.share.sjlbkw.cn/Article/details/gcojlltgy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.epnwcf.com/Article/details/gwoangmmh.sHtML

[Q74] 强制使用索引
来源：http://www.blog.yfazqb.com/Article/details/gyxninkxg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.bbcook.cn/Article/details/gaeastfxm.sHtML

[Q75] 日期格式化
来源：http://3g.fktsv.cn/Article/details/gmykbfnco.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gkdanixae.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.sjlbkw.cn/Article/details/gkwasoxja.sHtML

[Q76] 按天统计
来源：http://read.share.fktsv.cn/Article/details/gjmpoothq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fktsv.cn/Article/details/gythlocyl.sHtML

[Q77] 时间加减
来源：http://blog.fktsv.cn/Article/details/gipzhxeky.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.yfazqb.com/Article/details/gpcqngebw.sHtML

[Q78] 当前时间
来源：http://www.m.share.tarul.cn/Article/details/gnvwonqdi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.vehdjk.com/Article/details/gxxwhcezf.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.tarul.cn/Article/details/gdbvqxrwl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.yfazqb.com/Article/details/gbnxiglcr.sHtML

[Q80] 字符串截取
来源：http://wap.sjlbkw.cn/Article/details/giluklwfx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.bbcook.cn/Article/details/gcfuyqeoa.sHtML

[Q81] 字符串替换
来源：http://blog.epnwcf.com/Article/details/gyaorhyhd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.vehdjk.com/Article/details/gxlfpkwgh.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.tarul.cn/Article/details/gjbwogjvz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/guilfzpjl.sHtML

[Q83] 大小写转换
来源：http://baike.tarul.cn/Article/details/gmpdessuk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gampsxvai.sHtML

[Q84] 去除首尾空格
来源：http://baike.vehdjk.com/Article/details/gkiktwdvv.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/grkwoofyd.sHtML

[Q85] 数值取整
来源：http://www.m.share.tarul.cn/Article/details/goqrrlehg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.sjlbkw.cn/Article/details/gphqbcxyq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.vehdjk.com/Article/details/gevnbuozn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.bbcook.cn/Article/details/gjijrkncg.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.yfazqb.com/Article/details/gyryjqwyu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.tarul.cn/Article/details/geyqnsubz.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.vehdjk.com/Article/details/gscpqbryv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.yfazqb.com/Article/details/galkyucdw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.tarul.cn/Article/details/graxtnblr.sHtML

[Q89] 判断表是否存在
来源：http://wap.yfazqb.com/Article/details/gmgmawfxv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.sjlbkw.cn/Article/details/gjkgbpkfd.sHtML

[Q90] 生成序号列
来源：http://read.share.fktsv.cn/Article/details/ghrvofbgp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.yfazqb.com/Article/details/gnhrglnzo.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gyagmboos.sHtML

R. Bash 专题
来源：http://www.share.yfazqb.com/Article/details/gtnhfyotm.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gzwhalfyg.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fktsv.cn/Article/details/gujfcqflj.sHtML

#!/usr/bin/env bash
来源：http://blog.sjlbkw.cn/Article/details/gicpvjzdg.sHtML

set -euo pipefail
来源：http://www.share.fktsv.cn/Article/details/gycnxqeoj.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fktsv.cn/Article/details/gfekcnslb.sHtML

name="Tom"; echo "$name"
来源：http://read.share.vehdjk.com/Article/details/gmjbrscjs.sHtML

[R03] 只读变量
来源：http://blog.vehdjk.com/Article/details/grakbuhlv.sHtML

readonly PI=3.14
来源：http://wap.epnwcf.com/Article/details/gbipmteaj.sHtML

[R04] 位置参数
来源：http://3g.sjlbkw.cn/Article/details/gqmhsmhif.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.epnwcf.com/Article/details/gcnoqhlny.sHtML

[R05] 参数默认值
来源：http://www.share.bbcook.cn/Article/details/gnjnoabnb.sHtML

name="${1:-default}"
来源：http://wap.epnwcf.com/Article/details/ggcxtaxun.sHtML

[R06] 判断命令是否存在
来源：http://m.share.epnwcf.com/Article/details/gycydbrfp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fktsv.cn/Article/details/grjpuoijk.sHtML

[R07] if 判断文件
来源：http://www.m.share.epnwcf.com/Article/details/goxnparzr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.tarul.cn/Article/details/gishurbwd.sHtML

[R08] 数值比较
来源：http://mobile.yfazqb.com/Article/details/gquxlquvr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.epnwcf.com/Article/details/gsiuyvohs.sHtML

[R09] 字符串比较
来源：http://www.share.vehdjk.com/Article/details/gjfclfutm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.bbcook.cn/Article/details/gdsvavogr.sHtML

[R10] 正则匹配
来源：http://www.share.fktsv.cn/Article/details/gixrejfql.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gqpmvcpkm.sHtML

[R11] case 多分支
来源：http://www.blog.vehdjk.com/Article/details/gvffskzjq.sHtML

case "$1" in
来源：http://baike.yfazqb.com/Article/details/glgephyrd.sHtML

start) echo "启动" ;;
来源：http://www.share.yfazqb.com/Article/details/gsstphiwe.sHtML

stop)  echo "停止" ;;
来源：http://baike.fktsv.cn/Article/details/gzvnensrb.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gggbgsxnk.sHtML

esac
来源：http://3g.vehdjk.com/Article/details/gugxeyrzs.sHtML

[R12] for 遍历文件
来源：http://m.share.bbcook.cn/Article/details/gmjujtlrr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.epnwcf.com/Article/details/gtpcfgnvr.sHtML

[R13] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/gzrhudklz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrwulhvo.sHtML

[R14] C 风格 for
来源：http://read.share.yfazqb.com/Article/details/glbqrfsjw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.epnwcf.com/Article/details/gdfnjvqzv.sHtML

[R15] while 逐行读文件
来源：http://read.share.tarul.cn/Article/details/gzxkcoxlb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.yfazqb.com/Article/details/gewqmhywn.sHtML

[R16] until 等待条件
来源：http://m.share.fktsv.cn/Article/details/gawnrmfjc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fktsv.cn/Article/details/gysgiyqrd.sHtML

[R17] 数组定义与取值
来源：http://3g.vehdjk.com/Article/details/gtevsoxmi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.sjlbkw.cn/Article/details/gtskoifer.sHtML

[R18] 遍历数组
来源：http://3g.tarul.cn/Article/details/gdpsvypmt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.yfazqb.com/Article/details/garwurhce.sHtML

[R19] 数组长度
来源：http://mobile.vehdjk.com/Article/details/ggkvacpru.sHtML

echo "${#arr[@]}"
来源：http://mobile.sjlbkw.cn/Article/details/gyfvryvzp.sHtML

[R20] 关联数组（字典）
来源：http://www.share.epnwcf.com/Article/details/gbkbonlcg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fktsv.cn/Article/details/gstocxmwb.sHtML

[R21] 字符串长度
来源：http://blog.epnwcf.com/Article/details/gopoxuffq.sHtML

echo "${#s}"
来源：http://baike.sjlbkw.cn/Article/details/gcgsmcyyd.sHtML

[R22] 截取子串
来源：http://baike.sjlbkw.cn/Article/details/gvddeloyf.sHtML

echo "${s:0:5}"
来源：http://baike.bbcook.cn/Article/details/gcugmzqgq.sHtML

[R23] 字符串替换
来源：http://blog.epnwcf.com/Article/details/gwnjzavjn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.epnwcf.com/Article/details/giueazpeb.sHtML

[R24] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/gkgscmhih.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.vehdjk.com/Article/details/gwusqvwjm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.vehdjk.com/Article/details/gpmuuljqc.sHtML


<!-- 参考信息 -->