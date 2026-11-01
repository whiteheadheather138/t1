代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://blog.tarul.cn/Article/details/guqrkecun.sHtML

Go:   len(arr);  len(m)
来源：http://blog.yfazqb.com/Article/details/gzyqzxtja.sHtML

Ruby: x.length;  x.size
来源：http://3g.sjlbkw.cn/Article/details/gveefspvg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.bbcook.cn/Article/details/gcscacofz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.vehdjk.com/Article/details/gvosykuqo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.sjlbkw.cn/Article/details/gllklsxsc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.bbcook.cn/Article/details/gyvvycigr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.sjlbkw.cn/Article/details/gqcoeuofv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.bbcook.cn/Article/details/gqyqvmcvs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.bbcook.cn/Article/details/gfnwxbsxv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gvwhzvzsm.sHtML

Ruby: a == b
来源：http://www.blog.fktsv.cn/Article/details/ghxwyzxke.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.vehdjk.com/Article/details/ghntgplbg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.epnwcf.com/Article/details/gucpvijay.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.yfazqb.com/Article/details/gruqwqyht.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fktsv.cn/Article/details/gyvhneaum.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.vehdjk.com/Article/details/gypzizhsp.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fktsv.cn/Article/details/gobavopad.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.tarul.cn/Article/details/gilqngvcp.sHtML

Go:   if x == nil {}
来源：http://read.share.epnwcf.com/Article/details/gqtprglqu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.tarul.cn/Article/details/gnjejhqyg.sHtML

C#:   if (x is null) {}
来源：http://3g.yfazqb.com/Article/details/gzepgdlvy.sHtML

[P07] 防抖与节流
来源：http://www.share.yfazqb.com/Article/details/gysqftaoi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.vehdjk.com/Article/details/gkevcujse.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.tarul.cn/Article/details/gjwtjhtlj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.vehdjk.com/Article/details/ghsnqsgqz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/gswwbwrci.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.tarul.cn/Article/details/gmnpazdkv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.yfazqb.com/Article/details/gsoznhowu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.vehdjk.com/Article/details/gatfarzdy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.sjlbkw.cn/Article/details/gcndrsnvo.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.epnwcf.com/Article/details/gsfygbsho.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.tarul.cn/Article/details/gledxqsyi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.tarul.cn/Article/details/gknqqwdih.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.vehdjk.com/Article/details/gdbunmqdo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/glbldzqzt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.sjlbkw.cn/Article/details/gyofnlwlb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.sjlbkw.cn/Article/details/gwntmhflm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.sjlbkw.cn/Article/details/gpljmhksa.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fktsv.cn/Article/details/goilnyzvr.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gxjjkgofy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.tarul.cn/Article/details/gzunrmnzj.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/goihjbkdw.sHtML

[Q01] 创建表
来源：http://m.share.epnwcf.com/Article/details/ggymjyyfl.sHtML

CREATE TABLE users (
来源：http://www.blog.vehdjk.com/Article/details/gwfexjbbm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.vehdjk.com/Article/details/grmflweac.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.tarul.cn/Article/details/gswjdidsy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.vehdjk.com/Article/details/ggbouqskz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.tarul.cn/Article/details/gilfvrfbd.sHtML

);
来源：http://www.m.share.fktsv.cn/Article/details/gjgcwlgpc.sHtML

[Q02] 创建带外键的表
来源：http://read.share.tarul.cn/Article/details/gkpmxssgf.sHtML

CREATE TABLE orders (
来源：http://blog.tarul.cn/Article/details/gfrcbqjzn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/gmxvjbnri.sHtML

user_id INT NOT NULL,
来源：http://mobile.bbcook.cn/Article/details/gglpaugkx.sHtML

amount DECIMAL(10, 2),
来源：http://baike.epnwcf.com/Article/details/gswaklcuu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.vehdjk.com/Article/details/ghtfoifyk.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/ggkfydrol.sHtML

[Q03] 增加列
来源：http://m.share.tarul.cn/Article/details/gryjtcfwc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fktsv.cn/Article/details/gkpaeifob.sHtML

[Q04] 修改列类型
来源：http://mobile.bbcook.cn/Article/details/gbepvauqu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.yfazqb.com/Article/details/gshbicaxk.sHtML

[Q05] 重命名列
来源：http://3g.sjlbkw.cn/Article/details/gvebtkydn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fktsv.cn/Article/details/ggiiiqyvl.sHtML

[Q06] 删除列
来源：http://read.share.yfazqb.com/Article/details/gakqqnlwq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.vehdjk.com/Article/details/guwakpzvk.sHtML

[Q07] 删除表
来源：http://www.share.epnwcf.com/Article/details/gnsyqlzqi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fktsv.cn/Article/details/ggmagcmcn.sHtML

[Q08] 创建普通索引
来源：http://www.share.sjlbkw.cn/Article/details/grjyzwzvb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.sjlbkw.cn/Article/details/gbhxaajqq.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.tarul.cn/Article/details/girliguew.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.sjlbkw.cn/Article/details/gsvvurgem.sHtML

[Q10] 插入单行
来源：http://www.blog.vehdjk.com/Article/details/ghdtaarub.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gkgoqotqi.sHtML

[Q11] 一次插入多行
来源：http://www.blog.sjlbkw.cn/Article/details/grdnazmyd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gpufsoyqz.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fktsv.cn/Article/details/gurtbgvrj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.bbcook.cn/Article/details/gsfqzyeax.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.sjlbkw.cn/Article/details/grktwaqsr.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fktsv.cn/Article/details/gltwnyqvk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fktsv.cn/Article/details/gwnkehpbo.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.tarul.cn/Article/details/glzyhsknw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.vehdjk.com/Article/details/ghcvobhfc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.yfazqb.com/Article/details/gyglwalft.sHtML

[Q15] 查询全部
来源：http://wap.fktsv.cn/Article/details/gepdkobka.sHtML

SELECT * FROM users;
来源：http://read.share.tarul.cn/Article/details/gwskdtqyq.sHtML

[Q16] 查询指定列
来源：http://blog.vehdjk.com/Article/details/gyyasbvub.sHtML

SELECT id, name FROM users;
来源：http://blog.epnwcf.com/Article/details/gczhxamnh.sHtML

[Q17] 条件查询
来源：http://baike.vehdjk.com/Article/details/gfzccukqe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.yfazqb.com/Article/details/gcushcatd.sHtML

[Q18] 模糊匹配
来源：http://www.share.sjlbkw.cn/Article/details/gpfvedcbe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.bbcook.cn/Article/details/gzfjrksjc.sHtML

[Q19] 范围查询
来源：http://read.share.bbcook.cn/Article/details/gajhtqapc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.yfazqb.com/Article/details/gkrfdbopf.sHtML

[Q20] IN 列表
来源：http://baike.epnwcf.com/Article/details/gjrnebjhh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.sjlbkw.cn/Article/details/gjuqrstoj.sHtML

[Q21] 空值判断
来源：http://read.share.epnwcf.com/Article/details/gyyoshzzm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.bbcook.cn/Article/details/gzyiuetku.sHtML

[Q22] 排序
来源：http://www.m.share.epnwcf.com/Article/details/gjqusytif.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.tarul.cn/Article/details/gygvuyhcy.sHtML

[Q23] 分页
来源：http://wap.vehdjk.com/Article/details/gunzvrokj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.bbcook.cn/Article/details/gnuvgwxus.sHtML

[Q24] 去重
来源：http://read.share.fktsv.cn/Article/details/gmdaumpku.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fktsv.cn/Article/details/ggimiylmq.sHtML

[Q25] 只取前 N 条
来源：http://mobile.tarul.cn/Article/details/gqrxoikbk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.tarul.cn/Article/details/gmvrkexni.sHtML

[Q26] 计数
来源：http://wap.tarul.cn/Article/details/gecmyabeb.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gprhcfpsa.sHtML

[Q27] 条件计数
来源：http://www.m.share.epnwcf.com/Article/details/gfszvuvsr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.bbcook.cn/Article/details/gqgqqprns.sHtML

[Q28] 求和与平均
来源：http://www.share.sjlbkw.cn/Article/details/gtsbrwuaq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.tarul.cn/Article/details/geikwucei.sHtML

[Q29] 最大最小值
来源：http://www.blog.vehdjk.com/Article/details/gxxszduqe.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gazlqxdju.sHtML

[Q30] 分组统计
来源：http://www.m.share.sjlbkw.cn/Article/details/gmiersjwp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/gghkarktp.sHtML

[Q31] 分组后过滤
来源：http://m.share.epnwcf.com/Article/details/gtugbzofu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.epnwcf.com/Article/details/gfstfnorh.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.yfazqb.com/Article/details/gcnvlddwo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gdvtvfxyl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.yfazqb.com/Article/details/gogorfckp.sHtML

[Q33] 多列分组
来源：http://3g.yfazqb.com/Article/details/guyxrjpdz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fktsv.cn/Article/details/gnldskqrt.sHtML

[Q34] 每组取第一条
来源：http://read.share.tarul.cn/Article/details/gpgzpvmkh.sHtML

SELECT * FROM (
来源：http://www.m.share.tarul.cn/Article/details/gcsmisdad.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.sjlbkw.cn/Article/details/gbhhotbdt.sHtML

) t WHERE rn = 1;
来源：http://m.share.bbcook.cn/Article/details/gpyvfodvf.sHtML

[Q35] 内连接
来源：http://mobile.bbcook.cn/Article/details/gslnnzxrd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.sjlbkw.cn/Article/details/girhrhxar.sHtML

[Q36] 左连接
来源：http://mobile.sjlbkw.cn/Article/details/getjavvjy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.epnwcf.com/Article/details/gviixgidc.sHtML

[Q37] 右连接
来源：http://blog.vehdjk.com/Article/details/gbhomiwkm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.sjlbkw.cn/Article/details/gxokpiqzg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fktsv.cn/Article/details/gmiunldjh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fktsv.cn/Article/details/gwyhapexa.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fktsv.cn/Article/details/golsvtoqt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.sjlbkw.cn/Article/details/grvatdmme.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.vehdjk.com/Article/details/grrpjlwhy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.sjlbkw.cn/Article/details/gqegznkai.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fktsv.cn/Article/details/gekzezhjm.sHtML

[Q41] 多表连接
来源：http://read.share.vehdjk.com/Article/details/gotisbdlz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.sjlbkw.cn/Article/details/gsggugneg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.epnwcf.com/Article/details/guwrhyqcw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fktsv.cn/Article/details/galgtctrz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.epnwcf.com/Article/details/grvehnrwl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.bbcook.cn/Article/details/gqwomfyzr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.yfazqb.com/Article/details/gdratwidr.sHtML

[Q43] 标量子查询
来源：http://www.blog.yfazqb.com/Article/details/ggwnorsig.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.tarul.cn/Article/details/gfeqpbnsm.sHtML

[Q44] IN 子查询
来源：http://blog.tarul.cn/Article/details/gnfxcrdji.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.tarul.cn/Article/details/ggbrblvua.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.tarul.cn/Article/details/ghtoldeub.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/glfhwgnwm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.vehdjk.com/Article/details/getbideun.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.tarul.cn/Article/details/ghgeyypdi.sHtML

[Q47] 与平均值比较
来源：http://blog.tarul.cn/Article/details/glxeuysie.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.vehdjk.com/Article/details/geyzawhnj.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.tarul.cn/Article/details/gyshmksjp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fktsv.cn/Article/details/gcnslwyxs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.epnwcf.com/Article/details/gxuehfelu.sHtML

[Q49] 更新单行
来源：http://www.m.share.yfazqb.com/Article/details/gmtzcrjvb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.epnwcf.com/Article/details/gsfplceia.sHtML

[Q50] 批量更新
来源：http://blog.tarul.cn/Article/details/gcpjqslib.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.vehdjk.com/Article/details/ghbuvwrjx.sHtML

[Q51] 用子查询更新
来源：http://read.share.yfazqb.com/Article/details/gohwsqhnr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.epnwcf.com/Article/details/gqqvyejpb.sHtML

[Q52] 删除指定行
来源：http://www.m.share.sjlbkw.cn/Article/details/gsimziedp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.epnwcf.com/Article/details/gmhndvelr.sHtML

[Q53] 按条件删除
来源：http://3g.bbcook.cn/Article/details/gzuvniavx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fktsv.cn/Article/details/gpmakdnxy.sHtML

[Q54] 清空表
来源：http://3g.yfazqb.com/Article/details/gvhxotwrw.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.bbcook.cn/Article/details/gtpyobbti.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.epnwcf.com/Article/details/gtigiebsb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.epnwcf.com/Article/details/gibnrtene.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.tarul.cn/Article/details/gjaghafjw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.tarul.cn/Article/details/gbwgnvmug.sHtML

[Q57] 行号
来源：http://www.share.sjlbkw.cn/Article/details/geexkuhwh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.yfazqb.com/Article/details/gsncdcnym.sHtML

[Q58] 累计求和
来源：http://blog.bbcook.cn/Article/details/gdbfcvtny.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gzlimbrll.sHtML

[Q59] 分组内累计
来源：http://3g.epnwcf.com/Article/details/gtovhuqhn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gqecrhuhi.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fktsv.cn/Article/details/gpvyxobyi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.bbcook.cn/Article/details/gaghccbjm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gjulmtnzn.sHtML

[Q61] 移动平均
来源：http://baike.yfazqb.com/Article/details/gvmhbkmsl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gykibtres.sHtML

[Q62] 分组占比
来源：http://3g.fktsv.cn/Article/details/glnlgykbe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/grqbcdxse.sHtML

[Q63] 开启事务
来源：http://www.blog.sjlbkw.cn/Article/details/gudbmulgp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.bbcook.cn/Article/details/ggfvtiejs.sHtML

[Q64] 提交事务
来源：http://mobile.yfazqb.com/Article/details/gqdrhyzrp.sHtML

COMMIT;
来源：http://m.share.fktsv.cn/Article/details/gjoiiqkrb.sHtML

[Q65] 回滚事务
来源：http://wap.vehdjk.com/Article/details/gypbwwldj.sHtML

ROLLBACK;
来源：http://www.blog.vehdjk.com/Article/details/gjpkoybol.sHtML

[Q66] 行锁查询
来源：http://read.share.tarul.cn/Article/details/gtglfknry.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.tarul.cn/Article/details/gjsvpiosu.sHtML

[Q67] 设置隔离级别
来源：http://3g.fktsv.cn/Article/details/gzxfsihcj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.epnwcf.com/Article/details/gxypwojof.sHtML

[Q68] 保存点
来源：http://blog.tarul.cn/Article/details/gtrjbxxaf.sHtML

SAVEPOINT sp1;
来源：http://read.share.yfazqb.com/Article/details/gwujtuvum.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.yfazqb.com/Article/details/gnjhswuju.sHtML

[Q69] 查看执行计划
来源：http://wap.tarul.cn/Article/details/geqocskic.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.yfazqb.com/Article/details/gltgbikdi.sHtML

[Q70] 更新统计信息
来源：http://wap.sjlbkw.cn/Article/details/gqxwkwfoz.sHtML

ANALYZE TABLE users;
来源：http://www.share.tarul.cn/Article/details/gxlasarux.sHtML

[Q71] 查看建表语句
来源：http://blog.tarul.cn/Article/details/grphlccnk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.epnwcf.com/Article/details/gpfpnwedh.sHtML

[Q72] 查看索引
来源：http://mobile.vehdjk.com/Article/details/gpfyfrtes.sHtML

SHOW INDEX FROM users;
来源：http://www.share.tarul.cn/Article/details/gaffvfabu.sHtML

[Q73] 查看表状态
来源：http://m.share.epnwcf.com/Article/details/gfnegemjw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.vehdjk.com/Article/details/gpizmjdxw.sHtML

[Q74] 强制使用索引
来源：http://m.share.sjlbkw.cn/Article/details/gfzngdizq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.epnwcf.com/Article/details/gpqxtuzpl.sHtML

[Q75] 日期格式化
来源：http://wap.tarul.cn/Article/details/giptkeghn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gkotuiayr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.sjlbkw.cn/Article/details/gdfvwdnlu.sHtML

[Q76] 按天统计
来源：http://baike.sjlbkw.cn/Article/details/gwdnxedsa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.tarul.cn/Article/details/gthxjswuz.sHtML

[Q77] 时间加减
来源：http://3g.yfazqb.com/Article/details/gvlpufqbz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.sjlbkw.cn/Article/details/gnuodvhga.sHtML

[Q78] 当前时间
来源：http://3g.vehdjk.com/Article/details/gocifgyds.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.yfazqb.com/Article/details/gugfjbajv.sHtML

[Q79] 字符串拼接
来源：http://baike.tarul.cn/Article/details/gpebvmgks.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.bbcook.cn/Article/details/giabexdvy.sHtML

[Q80] 字符串截取
来源：http://mobile.tarul.cn/Article/details/goqoyuaco.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gzyzeutfv.sHtML

[Q81] 字符串替换
来源：http://www.share.sjlbkw.cn/Article/details/gkcdcijfl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.yfazqb.com/Article/details/ggryvwdnq.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.vehdjk.com/Article/details/gevnzzpij.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.tarul.cn/Article/details/gmisnzaca.sHtML

[Q83] 大小写转换
来源：http://baike.vehdjk.com/Article/details/grjeuursx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gdbpewmyo.sHtML

[Q84] 去除首尾空格
来源：http://baike.bbcook.cn/Article/details/gepbisxxs.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gzhzcovol.sHtML

[Q85] 数值取整
来源：http://read.share.tarul.cn/Article/details/gmmacmapf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.tarul.cn/Article/details/glwswftty.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.yfazqb.com/Article/details/geypsvykt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.tarul.cn/Article/details/gachcijny.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fktsv.cn/Article/details/gvxyapdrf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.epnwcf.com/Article/details/gswtfnqsy.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fktsv.cn/Article/details/giigopboo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fktsv.cn/Article/details/gmxflweoq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.tarul.cn/Article/details/gkyshhbxk.sHtML

[Q89] 判断表是否存在
来源：http://3g.epnwcf.com/Article/details/glemqhbsi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.tarul.cn/Article/details/gluzungaw.sHtML

[Q90] 生成序号列
来源：http://wap.fktsv.cn/Article/details/gssczfthl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.sjlbkw.cn/Article/details/gdksnfnkz.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/ghdlcptig.sHtML

R. Bash 专题
来源：http://read.share.vehdjk.com/Article/details/grabxsrsw.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gjwypasah.sHtML

[R01] shebang 与严格模式
来源：http://baike.yfazqb.com/Article/details/ghidkcood.sHtML

#!/usr/bin/env bash
来源：http://mobile.sjlbkw.cn/Article/details/gdrwptzra.sHtML

set -euo pipefail
来源：http://m.share.vehdjk.com/Article/details/gqldpqrai.sHtML

[R02] 变量赋值与使用
来源：http://baike.sjlbkw.cn/Article/details/gpfzrynep.sHtML

name="Tom"; echo "$name"
来源：http://blog.vehdjk.com/Article/details/gjqoudjdl.sHtML

[R03] 只读变量
来源：http://mobile.fktsv.cn/Article/details/grsqewtfk.sHtML

readonly PI=3.14
来源：http://www.blog.bbcook.cn/Article/details/gubhlowsl.sHtML

[R04] 位置参数
来源：http://blog.sjlbkw.cn/Article/details/gwsanzuyn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.sjlbkw.cn/Article/details/ghwkklymk.sHtML

[R05] 参数默认值
来源：http://mobile.vehdjk.com/Article/details/gkjgqgsix.sHtML

name="${1:-default}"
来源：http://www.share.bbcook.cn/Article/details/gzzqxwcnr.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.epnwcf.com/Article/details/gfvwwyqrm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/grkpiopeb.sHtML

[R07] if 判断文件
来源：http://read.share.yfazqb.com/Article/details/gmzjtpkuz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.yfazqb.com/Article/details/ghhgxnrnr.sHtML

[R08] 数值比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmjgktxw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.vehdjk.com/Article/details/godvtzisc.sHtML

[R09] 字符串比较
来源：http://read.share.yfazqb.com/Article/details/gakdrqnhv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.epnwcf.com/Article/details/gqlzqfjag.sHtML

[R10] 正则匹配
来源：http://read.share.epnwcf.com/Article/details/gypqezjzt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.vehdjk.com/Article/details/guflrtjki.sHtML

[R11] case 多分支
来源：http://www.share.epnwcf.com/Article/details/gjfagpiyn.sHtML

case "$1" in
来源：http://3g.bbcook.cn/Article/details/gmuuqmxyl.sHtML

start) echo "启动" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gjcdppgbi.sHtML

stop)  echo "停止" ;;
来源：http://www.share.vehdjk.com/Article/details/gqqnqatsy.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.epnwcf.com/Article/details/gxrrpsveh.sHtML

esac
来源：http://m.share.epnwcf.com/Article/details/gcpbatlry.sHtML

[R12] for 遍历文件
来源：http://baike.vehdjk.com/Article/details/gvpjjqkvu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.vehdjk.com/Article/details/gskpmofik.sHtML

[R13] for 计数循环
来源：http://read.share.fktsv.cn/Article/details/ghawsqvtw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.yfazqb.com/Article/details/gbriyforj.sHtML

[R14] C 风格 for
来源：http://www.m.share.sjlbkw.cn/Article/details/gzuawpdft.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.vehdjk.com/Article/details/guasqfbud.sHtML

[R15] while 逐行读文件
来源：http://blog.tarul.cn/Article/details/gjmcjoash.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.tarul.cn/Article/details/gjvbhtwix.sHtML

[R16] until 等待条件
来源：http://mobile.fktsv.cn/Article/details/glshtbjvl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.bbcook.cn/Article/details/gbcfdlwdq.sHtML

[R17] 数组定义与取值
来源：http://baike.vehdjk.com/Article/details/gbdjpbddo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.vehdjk.com/Article/details/gijlsjbii.sHtML

[R18] 遍历数组
来源：http://m.share.fktsv.cn/Article/details/gtpvzcvwb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fktsv.cn/Article/details/gpyasyfnx.sHtML

[R19] 数组长度
来源：http://www.share.bbcook.cn/Article/details/giljbjhlw.sHtML

echo "${#arr[@]}"
来源：http://www.share.sjlbkw.cn/Article/details/gcqxcbkra.sHtML

[R20] 关联数组（字典）
来源：http://www.share.bbcook.cn/Article/details/gxbmrvljf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.vehdjk.com/Article/details/gxbsfigps.sHtML

[R21] 字符串长度
来源：http://m.share.vehdjk.com/Article/details/gagmtaauz.sHtML

echo "${#s}"
来源：http://blog.sjlbkw.cn/Article/details/gfcjtfgjo.sHtML

[R22] 截取子串
来源：http://read.share.tarul.cn/Article/details/gahghyxqz.sHtML

echo "${s:0:5}"
来源：http://www.share.tarul.cn/Article/details/gkzzwrkwc.sHtML

[R23] 字符串替换
来源：http://m.share.fktsv.cn/Article/details/gvnaulecj.sHtML


<!-- 参考信息 -->