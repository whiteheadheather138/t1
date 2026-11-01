代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.vehdjk.com/Article/details/grxqfbbmk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.vehdjk.com/Article/details/gczojiedv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.tarul.cn/Article/details/gratourrc.sHtML

Ruby: a == b
来源：http://mobile.sjlbkw.cn/Article/details/gdxcwimys.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.sjlbkw.cn/Article/details/glgwncyhn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.sjlbkw.cn/Article/details/ghlbzetev.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.bbcook.cn/Article/details/gkbgtlmqy.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fktsv.cn/Article/details/giiawwxmr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fktsv.cn/Article/details/gsocpeadq.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqaycvxv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.sjlbkw.cn/Article/details/gyqkgognb.sHtML

Go:   if x == nil {}
来源：http://baike.sjlbkw.cn/Article/details/gpibjtdbe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.epnwcf.com/Article/details/gopiizich.sHtML

C#:   if (x is null) {}
来源：http://3g.bbcook.cn/Article/details/gmhcfbocc.sHtML

[P07] 防抖与节流
来源：http://www.share.fktsv.cn/Article/details/gtvhzavfg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.epnwcf.com/Article/details/gjslqrlym.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.epnwcf.com/Article/details/gpscxnjme.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/gopcsmzlt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/giinognzt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.bbcook.cn/Article/details/giswfrxvy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.bbcook.cn/Article/details/gjtwfgrde.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.bbcook.cn/Article/details/gtelbawbp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.yfazqb.com/Article/details/gonkkzyrs.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.sjlbkw.cn/Article/details/gczfgizkl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.sjlbkw.cn/Article/details/gslpcbciv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gnywmcdnk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.tarul.cn/Article/details/glvhxngkc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.sjlbkw.cn/Article/details/gldpvswfd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.sjlbkw.cn/Article/details/gmrgohiij.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.epnwcf.com/Article/details/goicllqow.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.vehdjk.com/Article/details/gzbywwmak.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.tarul.cn/Article/details/goqvazqrf.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gqmeecrsk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fktsv.cn/Article/details/gjnmoelia.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gxzbbmiyq.sHtML

[Q01] 创建表
来源：http://www.blog.sjlbkw.cn/Article/details/gtyigniti.sHtML

CREATE TABLE users (
来源：http://read.share.bbcook.cn/Article/details/gwhdvhpmv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.epnwcf.com/Article/details/gqqlpxadw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.sjlbkw.cn/Article/details/gqumsinan.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.yfazqb.com/Article/details/gtqsinmeu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.epnwcf.com/Article/details/gssvzpszz.sHtML

);
来源：http://m.share.vehdjk.com/Article/details/gdeubavnj.sHtML

[Q02] 创建带外键的表
来源：http://read.share.epnwcf.com/Article/details/gvjwynhub.sHtML

CREATE TABLE orders (
来源：http://www.blog.tarul.cn/Article/details/gvfyipntu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.yfazqb.com/Article/details/gdzdmdzyq.sHtML

user_id INT NOT NULL,
来源：http://wap.tarul.cn/Article/details/gtqtaplbd.sHtML

amount DECIMAL(10, 2),
来源：http://3g.tarul.cn/Article/details/gdjetxugz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.vehdjk.com/Article/details/gimheuyiu.sHtML

);
来源：http://mobile.yfazqb.com/Article/details/gfzsokhej.sHtML

[Q03] 增加列
来源：http://mobile.bbcook.cn/Article/details/gpffkwyhp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fktsv.cn/Article/details/gsblqjklp.sHtML

[Q04] 修改列类型
来源：http://www.m.share.bbcook.cn/Article/details/gzxbwkiey.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.yfazqb.com/Article/details/gvspgfgce.sHtML

[Q05] 重命名列
来源：http://mobile.yfazqb.com/Article/details/grkeojjsh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.sjlbkw.cn/Article/details/gztwuwveb.sHtML

[Q06] 删除列
来源：http://mobile.epnwcf.com/Article/details/gnrlctwro.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fktsv.cn/Article/details/getezilxi.sHtML

[Q07] 删除表
来源：http://baike.epnwcf.com/Article/details/gmwzuckse.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.epnwcf.com/Article/details/gpbzkeqjf.sHtML

[Q08] 创建普通索引
来源：http://3g.epnwcf.com/Article/details/gijfpkntt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.bbcook.cn/Article/details/gcteqkncy.sHtML

[Q09] 创建唯一索引
来源：http://wap.fktsv.cn/Article/details/guxlpsplh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.bbcook.cn/Article/details/goggqclru.sHtML

[Q10] 插入单行
来源：http://blog.fktsv.cn/Article/details/gekmnzxyf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gfnbvhktd.sHtML

[Q11] 一次插入多行
来源：http://m.share.bbcook.cn/Article/details/gtkppnkiq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.bbcook.cn/Article/details/gdyrfuxvl.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.vehdjk.com/Article/details/gaadtdboh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.epnwcf.com/Article/details/gbdmgpfwk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.epnwcf.com/Article/details/ghslwcdel.sHtML

[Q13] 忽略重复插入
来源：http://mobile.vehdjk.com/Article/details/gzpmtqxdi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fktsv.cn/Article/details/gcimbjdoq.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.bbcook.cn/Article/details/gkwbpqydc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.sjlbkw.cn/Article/details/guyukozex.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.vehdjk.com/Article/details/gvqpsvypf.sHtML

[Q15] 查询全部
来源：http://www.blog.tarul.cn/Article/details/getuohlqy.sHtML

SELECT * FROM users;
来源：http://www.share.tarul.cn/Article/details/gqzmbxfny.sHtML

[Q16] 查询指定列
来源：http://3g.bbcook.cn/Article/details/gngxfoigx.sHtML

SELECT id, name FROM users;
来源：http://wap.tarul.cn/Article/details/grzpfylio.sHtML

[Q17] 条件查询
来源：http://mobile.tarul.cn/Article/details/gyzgartap.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.sjlbkw.cn/Article/details/gzblyptsh.sHtML

[Q18] 模糊匹配
来源：http://mobile.bbcook.cn/Article/details/gotkpggtx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.yfazqb.com/Article/details/gatrazdwl.sHtML

[Q19] 范围查询
来源：http://www.share.fktsv.cn/Article/details/glxbuxtxp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.yfazqb.com/Article/details/gfdvbcful.sHtML

[Q20] IN 列表
来源：http://mobile.tarul.cn/Article/details/gszecvlgy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.yfazqb.com/Article/details/gjyjypsnl.sHtML

[Q21] 空值判断
来源：http://read.share.fktsv.cn/Article/details/gntrsjllc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fktsv.cn/Article/details/gtktajygo.sHtML

[Q22] 排序
来源：http://blog.bbcook.cn/Article/details/gnjafuodz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.sjlbkw.cn/Article/details/gjqzyotao.sHtML

[Q23] 分页
来源：http://baike.bbcook.cn/Article/details/gipwcflhs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.epnwcf.com/Article/details/gvgvsjuze.sHtML

[Q24] 去重
来源：http://blog.fktsv.cn/Article/details/grvyifadp.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.bbcook.cn/Article/details/ghubgaiby.sHtML

[Q25] 只取前 N 条
来源：http://3g.sjlbkw.cn/Article/details/gsiqxnivi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.tarul.cn/Article/details/gwrkawboj.sHtML

[Q26] 计数
来源：http://baike.tarul.cn/Article/details/guxdjigxl.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gopjudvjl.sHtML

[Q27] 条件计数
来源：http://blog.vehdjk.com/Article/details/gkovycleq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.yfazqb.com/Article/details/gmypxixqa.sHtML

[Q28] 求和与平均
来源：http://wap.vehdjk.com/Article/details/gfdpwbjlh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gatuuqqbe.sHtML

[Q29] 最大最小值
来源：http://blog.epnwcf.com/Article/details/gngdolcep.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gsubqhfam.sHtML

[Q30] 分组统计
来源：http://blog.sjlbkw.cn/Article/details/geiyqcdif.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fktsv.cn/Article/details/gyhgdmiiz.sHtML

[Q31] 分组后过滤
来源：http://wap.fktsv.cn/Article/details/gdhhglzdp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.tarul.cn/Article/details/galeemcfs.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gyhoghoxu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gxigorihq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.sjlbkw.cn/Article/details/gdoluoenv.sHtML

[Q33] 多列分组
来源：http://mobile.vehdjk.com/Article/details/gehvcdxqb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fktsv.cn/Article/details/gznitilxf.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.tarul.cn/Article/details/gjknfhgha.sHtML

SELECT * FROM (
来源：http://www.m.share.epnwcf.com/Article/details/gyqgpmxug.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.tarul.cn/Article/details/gavccxsea.sHtML

) t WHERE rn = 1;
来源：http://wap.vehdjk.com/Article/details/guemksrkz.sHtML

[Q35] 内连接
来源：http://www.blog.bbcook.cn/Article/details/gklufxkeq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.sjlbkw.cn/Article/details/gvwjexxij.sHtML

[Q36] 左连接
来源：http://blog.fktsv.cn/Article/details/gjhxzrdhq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.vehdjk.com/Article/details/gomudpsgr.sHtML

[Q37] 右连接
来源：http://mobile.fktsv.cn/Article/details/gsowbufas.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.yfazqb.com/Article/details/gyqkwyxjj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.bbcook.cn/Article/details/gdsoggqyj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.sjlbkw.cn/Article/details/gjtcxomdy.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.sjlbkw.cn/Article/details/gfqszjjai.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.tarul.cn/Article/details/grahhskeg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.epnwcf.com/Article/details/gyxawtzuh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.tarul.cn/Article/details/gwpydvdzi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.yfazqb.com/Article/details/giwhbgkbf.sHtML

[Q41] 多表连接
来源：http://baike.vehdjk.com/Article/details/gincrwsri.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.vehdjk.com/Article/details/groinosep.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.tarul.cn/Article/details/gjaqlyokh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.sjlbkw.cn/Article/details/ghedkkkzh.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.sjlbkw.cn/Article/details/gokxbahrc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.bbcook.cn/Article/details/gkbrgbmzm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.sjlbkw.cn/Article/details/gbaeafbzh.sHtML

[Q43] 标量子查询
来源：http://read.share.tarul.cn/Article/details/grocqgcwj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.epnwcf.com/Article/details/gxmvezvfe.sHtML

[Q44] IN 子查询
来源：http://baike.sjlbkw.cn/Article/details/gjsadvqls.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.sjlbkw.cn/Article/details/gcrugszzn.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmncpwve.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.yfazqb.com/Article/details/ggnqoojcn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.tarul.cn/Article/details/gsikkvlxy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.vehdjk.com/Article/details/gxhfeueox.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.vehdjk.com/Article/details/gvvlinrux.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.sjlbkw.cn/Article/details/guhikvpyw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.tarul.cn/Article/details/gcibxfuyx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.yfazqb.com/Article/details/gwwwycczr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.yfazqb.com/Article/details/gurbjsnzy.sHtML

[Q49] 更新单行
来源：http://3g.fktsv.cn/Article/details/gglwiqdhh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.bbcook.cn/Article/details/gbfzwswib.sHtML

[Q50] 批量更新
来源：http://3g.sjlbkw.cn/Article/details/gpeqtztgt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.tarul.cn/Article/details/gzohnjivt.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fktsv.cn/Article/details/gvxytmscr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.yfazqb.com/Article/details/gictblqor.sHtML

[Q52] 删除指定行
来源：http://read.share.fktsv.cn/Article/details/gnrzleudd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.yfazqb.com/Article/details/gyasfyrof.sHtML

[Q53] 按条件删除
来源：http://3g.sjlbkw.cn/Article/details/glrqqgbry.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fktsv.cn/Article/details/gcehmbwwv.sHtML

[Q54] 清空表
来源：http://3g.epnwcf.com/Article/details/gzmgwvyge.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.bbcook.cn/Article/details/gspvykwah.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fktsv.cn/Article/details/gzocvagaj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.bbcook.cn/Article/details/gihqczhqu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.bbcook.cn/Article/details/gbtlmkgsk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.bbcook.cn/Article/details/gthcjzkjg.sHtML

[Q57] 行号
来源：http://baike.sjlbkw.cn/Article/details/gluhnbnse.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fktsv.cn/Article/details/gyvrclssf.sHtML

[Q58] 累计求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmwhzhaj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gjsmbmwpp.sHtML

[Q59] 分组内累计
来源：http://blog.tarul.cn/Article/details/gldksgesj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gtvfeyadj.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.sjlbkw.cn/Article/details/gokfxunnc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.vehdjk.com/Article/details/gqknjrfoq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gkpobtmdw.sHtML

[Q61] 移动平均
来源：http://blog.bbcook.cn/Article/details/ggidjcguj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gbfwzvulm.sHtML

[Q62] 分组占比
来源：http://baike.sjlbkw.cn/Article/details/ggxdecyzt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fktsv.cn/Article/details/gefoboxik.sHtML

[Q63] 开启事务
来源：http://blog.yfazqb.com/Article/details/goicbbvvz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.epnwcf.com/Article/details/gyvuuqjjr.sHtML

[Q64] 提交事务
来源：http://www.share.epnwcf.com/Article/details/gsfhrymjn.sHtML

COMMIT;
来源：http://baike.sjlbkw.cn/Article/details/gyocympqf.sHtML

[Q65] 回滚事务
来源：http://baike.vehdjk.com/Article/details/givgfmbfv.sHtML

ROLLBACK;
来源：http://mobile.epnwcf.com/Article/details/gfzbpjsen.sHtML

[Q66] 行锁查询
来源：http://wap.tarul.cn/Article/details/gombwacey.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.vehdjk.com/Article/details/gaejvpfqj.sHtML

[Q67] 设置隔离级别
来源：http://www.share.bbcook.cn/Article/details/gnjqeoqbu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fktsv.cn/Article/details/gwcmndwth.sHtML

[Q68] 保存点
来源：http://blog.bbcook.cn/Article/details/goldpvrxv.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.vehdjk.com/Article/details/gcoyealoi.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.bbcook.cn/Article/details/gfygcfqlp.sHtML

[Q69] 查看执行计划
来源：http://www.share.sjlbkw.cn/Article/details/gdlzwxcjb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.sjlbkw.cn/Article/details/ghbynlvqs.sHtML

[Q70] 更新统计信息
来源：http://blog.vehdjk.com/Article/details/gzuzpuoav.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.yfazqb.com/Article/details/ghsrfjhyo.sHtML

[Q71] 查看建表语句
来源：http://m.share.bbcook.cn/Article/details/ghjofupkn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.epnwcf.com/Article/details/gbnpferzy.sHtML

[Q72] 查看索引
来源：http://www.blog.fktsv.cn/Article/details/grbdcjqmr.sHtML

SHOW INDEX FROM users;
来源：http://blog.sjlbkw.cn/Article/details/guigmpcmx.sHtML

[Q73] 查看表状态
来源：http://m.share.tarul.cn/Article/details/gellvosor.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.tarul.cn/Article/details/gbemgoncx.sHtML

[Q74] 强制使用索引
来源：http://blog.vehdjk.com/Article/details/gkvxnayhy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.tarul.cn/Article/details/gbonvkleq.sHtML

[Q75] 日期格式化
来源：http://wap.sjlbkw.cn/Article/details/gfdspwklx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gjovgcgab.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.bbcook.cn/Article/details/glqgpzzyh.sHtML

[Q76] 按天统计
来源：http://3g.vehdjk.com/Article/details/gxnazxfol.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.vehdjk.com/Article/details/gqnwyjoyy.sHtML

[Q77] 时间加减
来源：http://blog.vehdjk.com/Article/details/guwxcfbzo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.yfazqb.com/Article/details/ggzcrdwwb.sHtML

[Q78] 当前时间
来源：http://3g.tarul.cn/Article/details/gbrncezhx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.yfazqb.com/Article/details/gusuomies.sHtML

[Q79] 字符串拼接
来源：http://www.blog.yfazqb.com/Article/details/gezbgpvdq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.tarul.cn/Article/details/gmjjvnjtv.sHtML

[Q80] 字符串截取
来源：http://www.share.epnwcf.com/Article/details/gyrxwsjpi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gtrumcidl.sHtML

[Q81] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/gronvweyg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.epnwcf.com/Article/details/guvbhlbvs.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.bbcook.cn/Article/details/gifftxyrs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gduwutgcy.sHtML

[Q83] 大小写转换
来源：http://baike.vehdjk.com/Article/details/gwsjxnlgw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/gggguhzmm.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fktsv.cn/Article/details/gghnptzbz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gmbinfiyk.sHtML

[Q85] 数值取整
来源：http://baike.sjlbkw.cn/Article/details/gxkleidzx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fktsv.cn/Article/details/gaekrjgxa.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.epnwcf.com/Article/details/gvmwvfngw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.bbcook.cn/Article/details/gxsowvzrv.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.vehdjk.com/Article/details/gxccmrijx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.yfazqb.com/Article/details/gnrncqiei.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fktsv.cn/Article/details/gayonqxzc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.bbcook.cn/Article/details/gwyxjzovr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gppbxvtfn.sHtML

[Q89] 判断表是否存在
来源：http://read.share.vehdjk.com/Article/details/gmzgevxsy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fktsv.cn/Article/details/gjpiffmub.sHtML

[Q90] 生成序号列
来源：http://read.share.yfazqb.com/Article/details/gcrkiytqt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.yfazqb.com/Article/details/gkcmwsryj.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gqnptdqdf.sHtML

R. Bash 专题
来源：http://www.m.share.fktsv.cn/Article/details/gsvdzsxya.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gcjpuuxub.sHtML

[R01] shebang 与严格模式
来源：http://www.share.vehdjk.com/Article/details/glikpzabb.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.epnwcf.com/Article/details/gvuitdrnj.sHtML

set -euo pipefail
来源：http://baike.epnwcf.com/Article/details/gegiufkaq.sHtML

[R02] 变量赋值与使用
来源：http://read.share.tarul.cn/Article/details/gibxedpuq.sHtML

name="Tom"; echo "$name"
来源：http://mobile.sjlbkw.cn/Article/details/gdkxadwzy.sHtML

[R03] 只读变量
来源：http://blog.yfazqb.com/Article/details/gznjrplzl.sHtML

readonly PI=3.14
来源：http://mobile.sjlbkw.cn/Article/details/gzjmuyhhm.sHtML

[R04] 位置参数
来源：http://baike.fktsv.cn/Article/details/gnobtvdjb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.epnwcf.com/Article/details/gvkxrwcbv.sHtML

[R05] 参数默认值
来源：http://mobile.bbcook.cn/Article/details/gqpzchjkx.sHtML

name="${1:-default}"
来源：http://3g.epnwcf.com/Article/details/grzvscmbv.sHtML

[R06] 判断命令是否存在
来源：http://wap.fktsv.cn/Article/details/gbptixahl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.epnwcf.com/Article/details/groctdbpi.sHtML

[R07] if 判断文件
来源：http://m.share.yfazqb.com/Article/details/gdkmgtppy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.bbcook.cn/Article/details/gfeopmajv.sHtML

[R08] 数值比较
来源：http://blog.fktsv.cn/Article/details/ghjqpppfn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.epnwcf.com/Article/details/gsjdxmvkm.sHtML

[R09] 字符串比较
来源：http://m.share.yfazqb.com/Article/details/gdgigrdoa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.vehdjk.com/Article/details/gkhqjxgrc.sHtML

[R10] 正则匹配
来源：http://mobile.bbcook.cn/Article/details/ggucqtwhq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.vehdjk.com/Article/details/gogcacxfu.sHtML

[R11] case 多分支
来源：http://m.share.yfazqb.com/Article/details/gvaiknnua.sHtML

case "$1" in
来源：http://blog.epnwcf.com/Article/details/gifrjumtk.sHtML

start) echo "启动" ;;
来源：http://blog.epnwcf.com/Article/details/gnbjvwuqt.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fktsv.cn/Article/details/gttextewf.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwarrjvui.sHtML

esac
来源：http://wap.bbcook.cn/Article/details/gcijccghe.sHtML

[R12] for 遍历文件
来源：http://baike.tarul.cn/Article/details/gezoackuo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.vehdjk.com/Article/details/gbklngwnr.sHtML

[R13] for 计数循环
来源：http://read.share.tarul.cn/Article/details/guswjyxhq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.yfazqb.com/Article/details/gsjhhdmoc.sHtML

[R14] C 风格 for
来源：http://www.blog.fktsv.cn/Article/details/gdgqqmemc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.epnwcf.com/Article/details/gmrcvsmkz.sHtML

[R15] while 逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gkiftjnbn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fktsv.cn/Article/details/gtqkqtkdi.sHtML

[R16] until 等待条件
来源：http://3g.fktsv.cn/Article/details/goctjouat.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.bbcook.cn/Article/details/gupmygoqb.sHtML

[R17] 数组定义与取值
来源：http://www.share.yfazqb.com/Article/details/gmfbylvgh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.bbcook.cn/Article/details/girdbdxcd.sHtML

[R18] 遍历数组
来源：http://m.share.tarul.cn/Article/details/govumolnk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.yfazqb.com/Article/details/gdflkwkxc.sHtML

[R19] 数组长度
来源：http://www.share.bbcook.cn/Article/details/givfevwtt.sHtML

echo "${#arr[@]}"
来源：http://baike.epnwcf.com/Article/details/gepyldoxw.sHtML

[R20] 关联数组（字典）
来源：http://m.share.epnwcf.com/Article/details/gvrhobwhw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.vehdjk.com/Article/details/gkdhdcuiu.sHtML

[R21] 字符串长度
来源：http://www.share.tarul.cn/Article/details/gwqisalgi.sHtML

echo "${#s}"
来源：http://read.share.epnwcf.com/Article/details/ghpxsaxlf.sHtML

[R22] 截取子串
来源：http://mobile.sjlbkw.cn/Article/details/ggohspnkd.sHtML

echo "${s:0:5}"
来源：http://www.m.share.vehdjk.com/Article/details/gtrpiwyul.sHtML

[R23] 字符串替换
来源：http://baike.yfazqb.com/Article/details/gzsxzbciw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fktsv.cn/Article/details/gkohoirft.sHtML

[R24] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/gilwootos.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.epnwcf.com/Article/details/gcuajfqni.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.yfazqb.com/Article/details/gsnattgtd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.yfazqb.com/Article/details/gbgbgjwdj.sHtML

[R26] 命令替换
来源：http://www.m.share.fktsv.cn/Article/details/gvhaeblso.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.vehdjk.com/Article/details/gndfymwbs.sHtML

[R27] 算术展开
来源：http://3g.epnwcf.com/Article/details/gabcnelps.sHtML


<!-- 参考信息 -->