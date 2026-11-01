代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.bbcook.cn/Article/details/gevzknvoe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gfmsegjrv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.vehdjk.com/Article/details/guruylmnn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/gunnmorwy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.epnwcf.com/Article/details/gwuliadpy.sHtML

Go:   len(arr);  len(m)
来源：http://baike.tarul.cn/Article/details/gtbdysgdt.sHtML

Ruby: x.length;  x.size
来源：http://baike.epnwcf.com/Article/details/gvqwptlhr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fktsv.cn/Article/details/ghbtwzslq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.yfazqb.com/Article/details/guwvqycnq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.bbcook.cn/Article/details/gftujfyrn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.yfazqb.com/Article/details/gxvaydncl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.yfazqb.com/Article/details/gbtwjbdcq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.tarul.cn/Article/details/gmekwjbub.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.vehdjk.com/Article/details/gdhhyrzbx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.tarul.cn/Article/details/gdlzpvqdh.sHtML

Ruby: a == b
来源：http://m.share.sjlbkw.cn/Article/details/gwlnnrrba.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fktsv.cn/Article/details/gerkkeobl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.tarul.cn/Article/details/gydrcjyxs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.tarul.cn/Article/details/gnxlvlltn.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fktsv.cn/Article/details/grbcjemny.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.vehdjk.com/Article/details/gsjcwrluv.sHtML

TS:   if (x == null) {}
来源：http://www.blog.vehdjk.com/Article/details/gbgrxrlpi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.epnwcf.com/Article/details/gkzgpeenb.sHtML

Go:   if x == nil {}
来源：http://mobile.fktsv.cn/Article/details/glqrrejxp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fktsv.cn/Article/details/gclapvwjx.sHtML

C#:   if (x is null) {}
来源：http://mobile.sjlbkw.cn/Article/details/gtjxangtn.sHtML

[P07] 防抖与节流
来源：http://baike.epnwcf.com/Article/details/gpiwoqgux.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fktsv.cn/Article/details/gkevgrrue.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.vehdjk.com/Article/details/gvgslmktx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.yfazqb.com/Article/details/gsebtpjpc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gnqiqfmia.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.tarul.cn/Article/details/guqiowmxa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fktsv.cn/Article/details/gohokalqw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.vehdjk.com/Article/details/gxgelrdqj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.yfazqb.com/Article/details/goaoeoycy.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.yfazqb.com/Article/details/gqyhxpwxi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.yfazqb.com/Article/details/gftwpcali.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.bbcook.cn/Article/details/gtvmuopal.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.epnwcf.com/Article/details/glawwscxj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.yfazqb.com/Article/details/gmdcmpuyd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.vehdjk.com/Article/details/gkzifscqr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.sjlbkw.cn/Article/details/gatcjwnlc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.sjlbkw.cn/Article/details/goiqgdbcv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.bbcook.cn/Article/details/gxbawycpb.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gnltwtlfa.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.vehdjk.com/Article/details/gaedervsp.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gxjqqakbw.sHtML

[Q01] 创建表
来源：http://3g.yfazqb.com/Article/details/gzwwxazha.sHtML

CREATE TABLE users (
来源：http://mobile.bbcook.cn/Article/details/gwomeqfoo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.bbcook.cn/Article/details/gtmfnffnu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.epnwcf.com/Article/details/gfowlcukt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.tarul.cn/Article/details/gmcjppjcz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.bbcook.cn/Article/details/gkekpprcc.sHtML

);
来源：http://blog.fktsv.cn/Article/details/gwyzxzahy.sHtML

[Q02] 创建带外键的表
来源：http://read.share.vehdjk.com/Article/details/gtdhsufiu.sHtML

CREATE TABLE orders (
来源：http://www.share.bbcook.cn/Article/details/gwuwdifqw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.vehdjk.com/Article/details/gcmhrfplf.sHtML

user_id INT NOT NULL,
来源：http://www.share.epnwcf.com/Article/details/gxafgqnpw.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.tarul.cn/Article/details/gnaivmnka.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.vehdjk.com/Article/details/gpadbvkfu.sHtML

);
来源：http://3g.epnwcf.com/Article/details/gudpuzvcd.sHtML

[Q03] 增加列
来源：http://www.blog.bbcook.cn/Article/details/gfjblpxfb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.epnwcf.com/Article/details/gyhwrcxuu.sHtML

[Q04] 修改列类型
来源：http://read.share.epnwcf.com/Article/details/ggtujlrdf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.tarul.cn/Article/details/gtfclhdsc.sHtML

[Q05] 重命名列
来源：http://blog.bbcook.cn/Article/details/ghxckxpna.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.yfazqb.com/Article/details/ghwxsveqs.sHtML

[Q06] 删除列
来源：http://www.share.vehdjk.com/Article/details/gzieuikcq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fktsv.cn/Article/details/gzjskzryo.sHtML

[Q07] 删除表
来源：http://mobile.tarul.cn/Article/details/gjzvcphzn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.epnwcf.com/Article/details/gdognjqjq.sHtML

[Q08] 创建普通索引
来源：http://read.share.sjlbkw.cn/Article/details/glvkpncmr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.epnwcf.com/Article/details/gpbdynteg.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.bbcook.cn/Article/details/gxcuioxzx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.bbcook.cn/Article/details/gxprgntkq.sHtML

[Q10] 插入单行
来源：http://mobile.fktsv.cn/Article/details/ginxkerjj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.vehdjk.com/Article/details/gmtbadkig.sHtML

[Q11] 一次插入多行
来源：http://read.share.yfazqb.com/Article/details/gtdscwijy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.vehdjk.com/Article/details/gniaeiyxl.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.tarul.cn/Article/details/gazxhdnwd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.yfazqb.com/Article/details/gzocoaorn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.vehdjk.com/Article/details/gqcppgool.sHtML

[Q13] 忽略重复插入
来源：http://3g.tarul.cn/Article/details/gimtidrmn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.yfazqb.com/Article/details/gtmtxurho.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.epnwcf.com/Article/details/ghaqhrzld.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.vehdjk.com/Article/details/gfilvvexh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fktsv.cn/Article/details/gycirwkpv.sHtML

[Q15] 查询全部
来源：http://baike.epnwcf.com/Article/details/gmnbtcwkr.sHtML

SELECT * FROM users;
来源：http://www.share.bbcook.cn/Article/details/gxwqazaai.sHtML

[Q16] 查询指定列
来源：http://www.blog.epnwcf.com/Article/details/gxxovazev.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fktsv.cn/Article/details/ginatsdzv.sHtML

[Q17] 条件查询
来源：http://www.m.share.epnwcf.com/Article/details/gtmegaztx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.yfazqb.com/Article/details/ggrljoeun.sHtML

[Q18] 模糊匹配
来源：http://read.share.vehdjk.com/Article/details/gcounjwzc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.bbcook.cn/Article/details/gbclxmbgu.sHtML

[Q19] 范围查询
来源：http://baike.yfazqb.com/Article/details/gbehenlgm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.vehdjk.com/Article/details/gobbhgjnq.sHtML

[Q20] IN 列表
来源：http://www.share.bbcook.cn/Article/details/gjbxyniuq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.epnwcf.com/Article/details/guvmpniku.sHtML

[Q21] 空值判断
来源：http://m.share.epnwcf.com/Article/details/guityzuaq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.sjlbkw.cn/Article/details/gsxblxscu.sHtML

[Q22] 排序
来源：http://blog.sjlbkw.cn/Article/details/ghmzcbnwt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.yfazqb.com/Article/details/gjhbaqcen.sHtML

[Q23] 分页
来源：http://www.share.epnwcf.com/Article/details/gwhiqnyfo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.tarul.cn/Article/details/gtsikjeiv.sHtML

[Q24] 去重
来源：http://m.share.yfazqb.com/Article/details/gvjtnrujj.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.vehdjk.com/Article/details/gukkaikdk.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.epnwcf.com/Article/details/gzzgggthn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.bbcook.cn/Article/details/gtjzzfzyt.sHtML

[Q26] 计数
来源：http://read.share.bbcook.cn/Article/details/gdcdazzkm.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fktsv.cn/Article/details/ghurerbic.sHtML

[Q27] 条件计数
来源：http://m.share.tarul.cn/Article/details/grwrvekie.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.epnwcf.com/Article/details/grzztsfyt.sHtML

[Q28] 求和与平均
来源：http://read.share.vehdjk.com/Article/details/goekxzkqs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.tarul.cn/Article/details/gnzijblop.sHtML

[Q29] 最大最小值
来源：http://3g.bbcook.cn/Article/details/gwfspzzyn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gqutbztfn.sHtML

[Q30] 分组统计
来源：http://read.share.vehdjk.com/Article/details/gtztnjmtq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gtidjxilw.sHtML

[Q31] 分组后过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gmgwmmzem.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.tarul.cn/Article/details/gobgkjstq.sHtML

[Q32] 分组拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/gquwzswoh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/gjrusfxbe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fktsv.cn/Article/details/gcnwjjihh.sHtML

[Q33] 多列分组
来源：http://www.m.share.epnwcf.com/Article/details/gzazswpwg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fktsv.cn/Article/details/gqdhvqffb.sHtML

[Q34] 每组取第一条
来源：http://wap.yfazqb.com/Article/details/gktblibls.sHtML

SELECT * FROM (
来源：http://baike.fktsv.cn/Article/details/guiateogx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.yfazqb.com/Article/details/grdqbmysy.sHtML

) t WHERE rn = 1;
来源：http://3g.fktsv.cn/Article/details/gogzonjyf.sHtML

[Q35] 内连接
来源：http://www.blog.tarul.cn/Article/details/gpmzsdodw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.yfazqb.com/Article/details/gjxszjfkc.sHtML

[Q36] 左连接
来源：http://www.m.share.yfazqb.com/Article/details/gnngoaqwy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fktsv.cn/Article/details/gyedbiaoh.sHtML

[Q37] 右连接
来源：http://www.blog.fktsv.cn/Article/details/gvctrvytk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.tarul.cn/Article/details/gdsnmylot.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.yfazqb.com/Article/details/gcblickmr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.bbcook.cn/Article/details/gaikrxvam.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.epnwcf.com/Article/details/gflvvvviv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.tarul.cn/Article/details/gllzpkzxn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzatjikfh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.tarul.cn/Article/details/gdigqvzjk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.yfazqb.com/Article/details/gekuilxkc.sHtML

[Q41] 多表连接
来源：http://www.blog.yfazqb.com/Article/details/gxqwafdru.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.tarul.cn/Article/details/guxplkjea.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.bbcook.cn/Article/details/gdaoiuhvu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.bbcook.cn/Article/details/gfqgejizh.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.bbcook.cn/Article/details/gjmtjazuv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.epnwcf.com/Article/details/gopuvassf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fktsv.cn/Article/details/gbmyagltw.sHtML

[Q43] 标量子查询
来源：http://read.share.tarul.cn/Article/details/gjaygowbu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.yfazqb.com/Article/details/gzrqganaf.sHtML

[Q44] IN 子查询
来源：http://www.blog.yfazqb.com/Article/details/gjzpbhinf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.bbcook.cn/Article/details/gepprzgxf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.vehdjk.com/Article/details/gmijczxuw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.vehdjk.com/Article/details/gqdpjzyvj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.yfazqb.com/Article/details/gsibskdru.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.vehdjk.com/Article/details/gwrcvepmh.sHtML

[Q47] 与平均值比较
来源：http://read.share.tarul.cn/Article/details/grgesxnlb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.yfazqb.com/Article/details/gqjewpddb.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.epnwcf.com/Article/details/gbdpgennk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.tarul.cn/Article/details/gxgqklwgp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.sjlbkw.cn/Article/details/gikpgxgfq.sHtML

[Q49] 更新单行
来源：http://www.m.share.fktsv.cn/Article/details/gduajydmz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/ghzlcksqr.sHtML

[Q50] 批量更新
来源：http://www.m.share.tarul.cn/Article/details/gcdrfmcbk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.tarul.cn/Article/details/gqatgylth.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.vehdjk.com/Article/details/gqscnratg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.yfazqb.com/Article/details/gobusfzam.sHtML

[Q52] 删除指定行
来源：http://www.m.share.vehdjk.com/Article/details/ghglfyees.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.sjlbkw.cn/Article/details/gvjobjmnk.sHtML

[Q53] 按条件删除
来源：http://baike.vehdjk.com/Article/details/golyaszmi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.yfazqb.com/Article/details/gzsdbycbf.sHtML

[Q54] 清空表
来源：http://3g.tarul.cn/Article/details/gwfnzlldq.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.bbcook.cn/Article/details/geeyktzcg.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.epnwcf.com/Article/details/ghwkwvhof.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.epnwcf.com/Article/details/gdhvsweye.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fktsv.cn/Article/details/gwrutkwju.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.sjlbkw.cn/Article/details/gkxttwdzt.sHtML

[Q57] 行号
来源：http://wap.fktsv.cn/Article/details/glrvsiqba.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.yfazqb.com/Article/details/ghskpwvlg.sHtML

[Q58] 累计求和
来源：http://www.blog.sjlbkw.cn/Article/details/gzhbyqwyq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gqfaafhfo.sHtML

[Q59] 分组内累计
来源：http://read.share.vehdjk.com/Article/details/gxgjzchfk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gvdilpvvg.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.vehdjk.com/Article/details/gnlalcruo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.sjlbkw.cn/Article/details/gpmxdqijc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gqnullucl.sHtML

[Q61] 移动平均
来源：http://www.share.bbcook.cn/Article/details/giyqdeykb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.tarul.cn/Article/details/guurbtqtz.sHtML

[Q62] 分组占比
来源：http://3g.fktsv.cn/Article/details/gybpbcveb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/giugtfpgk.sHtML

[Q63] 开启事务
来源：http://wap.bbcook.cn/Article/details/gnsdbmytt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.tarul.cn/Article/details/gblaspipm.sHtML

[Q64] 提交事务
来源：http://baike.epnwcf.com/Article/details/grphlhiwq.sHtML

COMMIT;
来源：http://www.m.share.vehdjk.com/Article/details/gaeqjmvtd.sHtML

[Q65] 回滚事务
来源：http://read.share.fktsv.cn/Article/details/gbtkfooec.sHtML

ROLLBACK;
来源：http://read.share.tarul.cn/Article/details/gcssbvgar.sHtML

[Q66] 行锁查询
来源：http://blog.tarul.cn/Article/details/glswzdbgo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.epnwcf.com/Article/details/gzwonekwb.sHtML

[Q67] 设置隔离级别
来源：http://baike.vehdjk.com/Article/details/gyzwfjfvj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.sjlbkw.cn/Article/details/gdtmjfuad.sHtML

[Q68] 保存点
来源：http://blog.sjlbkw.cn/Article/details/gvcngodwp.sHtML

SAVEPOINT sp1;
来源：http://www.blog.bbcook.cn/Article/details/gznxniazj.sHtML

ROLLBACK TO sp1;
来源：http://mobile.vehdjk.com/Article/details/gtpvveafu.sHtML

[Q69] 查看执行计划
来源：http://read.share.fktsv.cn/Article/details/gntdgexaw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fktsv.cn/Article/details/gqvgdzxbb.sHtML

[Q70] 更新统计信息
来源：http://baike.vehdjk.com/Article/details/guvultkwf.sHtML

ANALYZE TABLE users;
来源：http://m.share.fktsv.cn/Article/details/gcubzqyup.sHtML

[Q71] 查看建表语句
来源：http://read.share.vehdjk.com/Article/details/gkrvuhjwn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fktsv.cn/Article/details/gejhbhqxt.sHtML

[Q72] 查看索引
来源：http://wap.fktsv.cn/Article/details/ghminmvnt.sHtML

SHOW INDEX FROM users;
来源：http://3g.bbcook.cn/Article/details/gunbzkrlj.sHtML

[Q73] 查看表状态
来源：http://www.blog.tarul.cn/Article/details/gwzlycssa.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fktsv.cn/Article/details/gzpxmgmby.sHtML

[Q74] 强制使用索引
来源：http://blog.bbcook.cn/Article/details/gahkoavhk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fktsv.cn/Article/details/gnnjcizhb.sHtML

[Q75] 日期格式化
来源：http://mobile.vehdjk.com/Article/details/ghshnymet.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gfzrjxqfi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.vehdjk.com/Article/details/ginfmybfv.sHtML

[Q76] 按天统计
来源：http://www.share.tarul.cn/Article/details/gaquksgiq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fktsv.cn/Article/details/gykdrclkf.sHtML

[Q77] 时间加减
来源：http://3g.yfazqb.com/Article/details/ggsppdxyr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.sjlbkw.cn/Article/details/geuqtuulj.sHtML

[Q78] 当前时间
来源：http://www.m.share.vehdjk.com/Article/details/ghyzgvqgh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.sjlbkw.cn/Article/details/gyapqmydv.sHtML

[Q79] 字符串拼接
来源：http://3g.yfazqb.com/Article/details/gjzzsioos.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fktsv.cn/Article/details/gumxfmocx.sHtML

[Q80] 字符串截取
来源：http://www.share.yfazqb.com/Article/details/gnjogjbey.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.bbcook.cn/Article/details/goohcgsge.sHtML

[Q81] 字符串替换
来源：http://blog.epnwcf.com/Article/details/ghwuvofyo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.epnwcf.com/Article/details/gmtsqfowz.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.tarul.cn/Article/details/gprmrlytf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gwvjiabke.sHtML

[Q83] 大小写转换
来源：http://wap.epnwcf.com/Article/details/glwjlclug.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gzxrtzyim.sHtML

[Q84] 去除首尾空格
来源：http://m.share.epnwcf.com/Article/details/gmvyizeri.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gquvkxjle.sHtML

[Q85] 数值取整
来源：http://blog.yfazqb.com/Article/details/gnayjkdre.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.epnwcf.com/Article/details/ghfpgksui.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.epnwcf.com/Article/details/gjfqzuaex.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.vehdjk.com/Article/details/gtohweoys.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.sjlbkw.cn/Article/details/gsglndtxg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.sjlbkw.cn/Article/details/ghafycauz.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fktsv.cn/Article/details/guhjbylqa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fktsv.cn/Article/details/gvggdmxfz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.yfazqb.com/Article/details/grwllbsjg.sHtML

[Q89] 判断表是否存在
来源：http://read.share.bbcook.cn/Article/details/gmtnombiz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.tarul.cn/Article/details/gqihvoqrf.sHtML

[Q90] 生成序号列
来源：http://www.m.share.vehdjk.com/Article/details/guauxifra.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.epnwcf.com/Article/details/glblixlyw.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/glpnhnroz.sHtML

R. Bash 专题
来源：http://3g.epnwcf.com/Article/details/gjnukhhoc.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/glbhrkdzz.sHtML

[R01] shebang 与严格模式
来源：http://wap.tarul.cn/Article/details/gesfoaolk.sHtML

#!/usr/bin/env bash
来源：http://3g.epnwcf.com/Article/details/gqenuulse.sHtML

set -euo pipefail
来源：http://www.share.yfazqb.com/Article/details/gdmlekvkv.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fktsv.cn/Article/details/gjkzvovqo.sHtML

name="Tom"; echo "$name"
来源：http://read.share.sjlbkw.cn/Article/details/ggpzaapib.sHtML

[R03] 只读变量
来源：http://www.blog.bbcook.cn/Article/details/gesjddpqm.sHtML

readonly PI=3.14
来源：http://www.blog.tarul.cn/Article/details/gktpgdlig.sHtML

[R04] 位置参数
来源：http://www.m.share.yfazqb.com/Article/details/gtwxdcfop.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.tarul.cn/Article/details/gxhxrsrmh.sHtML

[R05] 参数默认值
来源：http://mobile.bbcook.cn/Article/details/ghlqvjezd.sHtML

name="${1:-default}"
来源：http://wap.tarul.cn/Article/details/gelmbvzik.sHtML

[R06] 判断命令是否存在
来源：http://m.share.bbcook.cn/Article/details/gtqyopoeb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/ggycvgsua.sHtML

[R07] if 判断文件
来源：http://mobile.tarul.cn/Article/details/gekfvvjsz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.yfazqb.com/Article/details/grbzswjmx.sHtML

[R08] 数值比较
来源：http://m.share.vehdjk.com/Article/details/ghfhfznso.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.tarul.cn/Article/details/gbuuawwbk.sHtML

[R09] 字符串比较
来源：http://mobile.fktsv.cn/Article/details/gjbtcqgpn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gznggtsml.sHtML

[R10] 正则匹配
来源：http://3g.sjlbkw.cn/Article/details/gpilesnqt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.epnwcf.com/Article/details/gkauawryk.sHtML

[R11] case 多分支
来源：http://www.blog.epnwcf.com/Article/details/gcoarzxkt.sHtML

case "$1" in
来源：http://www.share.bbcook.cn/Article/details/galwlooxm.sHtML

start) echo "启动" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gsbrthjdf.sHtML

stop)  echo "停止" ;;
来源：http://mobile.vehdjk.com/Article/details/gqwviozvv.sHtML

*)     echo "未知命令" ;;
来源：http://baike.sjlbkw.cn/Article/details/gotjkqecb.sHtML

esac
来源：http://www.m.share.vehdjk.com/Article/details/gjqzhgihc.sHtML

[R12] for 遍历文件
来源：http://m.share.vehdjk.com/Article/details/gcuwwratr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.epnwcf.com/Article/details/gvjibqldh.sHtML

[R13] for 计数循环
来源：http://baike.vehdjk.com/Article/details/gcosphsst.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/ghhqytydi.sHtML

[R14] C 风格 for
来源：http://wap.fktsv.cn/Article/details/gayiwkjmy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.sjlbkw.cn/Article/details/gsscbulxn.sHtML

[R15] while 逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gwkcjrzut.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.vehdjk.com/Article/details/gothllukb.sHtML

[R16] until 等待条件
来源：http://baike.fktsv.cn/Article/details/gqycwqjmh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/gtujkslks.sHtML

[R17] 数组定义与取值
来源：http://www.blog.sjlbkw.cn/Article/details/gyupitxlu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fktsv.cn/Article/details/gfvanzpme.sHtML

[R18] 遍历数组
来源：http://www.m.share.epnwcf.com/Article/details/grixidfsz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.epnwcf.com/Article/details/gknbtswyj.sHtML

[R19] 数组长度
来源：http://mobile.sjlbkw.cn/Article/details/ghkpamtpv.sHtML

echo "${#arr[@]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gfbktcjjg.sHtML

[R20] 关联数组（字典）
来源：http://3g.epnwcf.com/Article/details/gvnuhpiwh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.sjlbkw.cn/Article/details/gfrrsdmyz.sHtML

[R21] 字符串长度
来源：http://baike.yfazqb.com/Article/details/grlyexers.sHtML


<!-- 参考信息 -->