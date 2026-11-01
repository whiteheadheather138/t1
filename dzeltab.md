代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.tarul.cn/Article/details/gkvjubkzy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gbymxdlod.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.epnwcf.com/Article/details/gnpwjilcl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/guhsalzmx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.tarul.cn/Article/details/gmzvottfy.sHtML

Go:   len(arr);  len(m)
来源：http://blog.yfazqb.com/Article/details/gumflbelq.sHtML

Ruby: x.length;  x.size
来源：http://blog.bbcook.cn/Article/details/gufuvxirj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.bbcook.cn/Article/details/gviqrvwxg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.tarul.cn/Article/details/gkqspprsi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.bbcook.cn/Article/details/gicmxzjce.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.tarul.cn/Article/details/gwpbgiwqy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.tarul.cn/Article/details/giioiisnm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.epnwcf.com/Article/details/gvwbxmzex.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.vehdjk.com/Article/details/gqjxojtsx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gwodkfaba.sHtML

Ruby: a == b
来源：http://m.share.sjlbkw.cn/Article/details/gwzbbfgsy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.bbcook.cn/Article/details/goqcdybmq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fktsv.cn/Article/details/ghknaziwt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.vehdjk.com/Article/details/ghdeoohok.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.yfazqb.com/Article/details/ghyreycfu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.epnwcf.com/Article/details/gautueggg.sHtML

TS:   if (x == null) {}
来源：http://www.blog.tarul.cn/Article/details/gpmatdcig.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.bbcook.cn/Article/details/ghrpmvfhx.sHtML

Go:   if x == nil {}
来源：http://3g.bbcook.cn/Article/details/gbvtuppys.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fktsv.cn/Article/details/gfmcrclqp.sHtML

C#:   if (x is null) {}
来源：http://wap.tarul.cn/Article/details/gaqbrpfeb.sHtML

[P07] 防抖与节流
来源：http://mobile.yfazqb.com/Article/details/gzwvuckhf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.bbcook.cn/Article/details/gkbwmfeam.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.yfazqb.com/Article/details/gmhfdlxbg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/gyuqudijs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gdaomkiha.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.tarul.cn/Article/details/gjwsavkot.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.yfazqb.com/Article/details/gxagxiefu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.epnwcf.com/Article/details/ghhysrerm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.bbcook.cn/Article/details/ghtckbctm.sHtML

[P08] 处理浮点精度问题
来源：http://wap.yfazqb.com/Article/details/gvwuwzzll.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.yfazqb.com/Article/details/gkdbqonch.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.vehdjk.com/Article/details/ggidgcfaz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fktsv.cn/Article/details/gdptjrxgb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.vehdjk.com/Article/details/gaidwzjxb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.tarul.cn/Article/details/gdnqvjdjg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.sjlbkw.cn/Article/details/gdcanlqck.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.sjlbkw.cn/Article/details/gowkidtpd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.bbcook.cn/Article/details/gjaybeuvp.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gkjyszgqp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.yfazqb.com/Article/details/gsymbcjos.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gacrovgyk.sHtML

[Q01] 创建表
来源：http://read.share.sjlbkw.cn/Article/details/gxgrzvpnk.sHtML

CREATE TABLE users (
来源：http://www.share.yfazqb.com/Article/details/gpwccbujq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fktsv.cn/Article/details/gkyhkwudt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/gwjzejkga.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.tarul.cn/Article/details/gdigsgrhg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fktsv.cn/Article/details/gixjvxeqa.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/ggonzsevb.sHtML

[Q02] 创建带外键的表
来源：http://wap.epnwcf.com/Article/details/gdnqfwjwx.sHtML

CREATE TABLE orders (
来源：http://www.share.bbcook.cn/Article/details/gipvcnahr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.sjlbkw.cn/Article/details/gfjesnspp.sHtML

user_id INT NOT NULL,
来源：http://baike.tarul.cn/Article/details/gtedakolr.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.epnwcf.com/Article/details/gaxvkgtof.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fktsv.cn/Article/details/goibkhjte.sHtML

);
来源：http://www.m.share.bbcook.cn/Article/details/gmgavohbh.sHtML

[Q03] 增加列
来源：http://baike.fktsv.cn/Article/details/gmqbiempp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.tarul.cn/Article/details/gplgyvpve.sHtML

[Q04] 修改列类型
来源：http://www.m.share.tarul.cn/Article/details/gkdxtinbl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.epnwcf.com/Article/details/gmpspsbbk.sHtML

[Q05] 重命名列
来源：http://www.m.share.vehdjk.com/Article/details/gqxwposoy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fktsv.cn/Article/details/gqegdtgol.sHtML

[Q06] 删除列
来源：http://www.m.share.yfazqb.com/Article/details/gnoavjytg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.epnwcf.com/Article/details/gxwgqpfql.sHtML

[Q07] 删除表
来源：http://www.m.share.bbcook.cn/Article/details/ggyynqmyr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fktsv.cn/Article/details/ggmgnfruu.sHtML

[Q08] 创建普通索引
来源：http://baike.vehdjk.com/Article/details/gxedrokir.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/ggefebtto.sHtML

[Q09] 创建唯一索引
来源：http://m.share.bbcook.cn/Article/details/gpbablsdm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.epnwcf.com/Article/details/gtyiswbew.sHtML

[Q10] 插入单行
来源：http://www.m.share.fktsv.cn/Article/details/gnlsxsykk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/gylhdsauz.sHtML

[Q11] 一次插入多行
来源：http://blog.epnwcf.com/Article/details/gjeaqcrcm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.bbcook.cn/Article/details/gdxokvfjf.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.yfazqb.com/Article/details/gnxruoodc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.tarul.cn/Article/details/gbtpbkclt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.epnwcf.com/Article/details/gvapfzinl.sHtML

[Q13] 忽略重复插入
来源：http://baike.fktsv.cn/Article/details/gfrpshiwy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.yfazqb.com/Article/details/gvxmvbpeu.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.epnwcf.com/Article/details/gicrkucgk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.vehdjk.com/Article/details/ggzzrzjjl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fktsv.cn/Article/details/gdcaortud.sHtML

[Q15] 查询全部
来源：http://3g.tarul.cn/Article/details/guaovzayv.sHtML

SELECT * FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gytnftphk.sHtML

[Q16] 查询指定列
来源：http://www.blog.yfazqb.com/Article/details/gbljwuiyq.sHtML

SELECT id, name FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gyqgrgpqk.sHtML

[Q17] 条件查询
来源：http://m.share.bbcook.cn/Article/details/gsludsgmn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gzixaezcu.sHtML

[Q18] 模糊匹配
来源：http://read.share.tarul.cn/Article/details/gzhsqshmo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.bbcook.cn/Article/details/gowbzdhlb.sHtML

[Q19] 范围查询
来源：http://3g.epnwcf.com/Article/details/gfmbzxcws.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.vehdjk.com/Article/details/glhtfjeiv.sHtML

[Q20] IN 列表
来源：http://3g.fktsv.cn/Article/details/gosznbygj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.epnwcf.com/Article/details/gwrenffgv.sHtML

[Q21] 空值判断
来源：http://www.share.fktsv.cn/Article/details/gukvqrisr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.yfazqb.com/Article/details/gsuiskunq.sHtML

[Q22] 排序
来源：http://www.m.share.vehdjk.com/Article/details/gzombixrx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.vehdjk.com/Article/details/ghkdxgzsq.sHtML

[Q23] 分页
来源：http://m.share.epnwcf.com/Article/details/gndnqjusl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.yfazqb.com/Article/details/ghwziayul.sHtML

[Q24] 去重
来源：http://baike.vehdjk.com/Article/details/gvvingsra.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/grgbodgfd.sHtML

[Q25] 只取前 N 条
来源：http://read.share.vehdjk.com/Article/details/grmncmdnp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.yfazqb.com/Article/details/gtujeeakp.sHtML

[Q26] 计数
来源：http://wap.tarul.cn/Article/details/guhbrnqiz.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.vehdjk.com/Article/details/ghohhhgfi.sHtML

[Q27] 条件计数
来源：http://www.share.vehdjk.com/Article/details/gdixpbzwf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.epnwcf.com/Article/details/gplutdjrd.sHtML

[Q28] 求和与平均
来源：http://blog.vehdjk.com/Article/details/gfuyuxstp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gvjwvemae.sHtML

[Q29] 最大最小值
来源：http://m.share.tarul.cn/Article/details/gauafxvjv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gxhwmzbni.sHtML

[Q30] 分组统计
来源：http://www.blog.sjlbkw.cn/Article/details/giqllzgtc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gaygzgqzu.sHtML

[Q31] 分组后过滤
来源：http://m.share.vehdjk.com/Article/details/guouvqpyb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.tarul.cn/Article/details/gbcnsxrdt.sHtML

[Q32] 分组拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/gttuabgyh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/gfrnnvfyf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.vehdjk.com/Article/details/gpdpklbsq.sHtML

[Q33] 多列分组
来源：http://www.share.yfazqb.com/Article/details/gjvtmbfbi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.yfazqb.com/Article/details/gbkdvkerd.sHtML

[Q34] 每组取第一条
来源：http://3g.sjlbkw.cn/Article/details/gtlxhowdv.sHtML

SELECT * FROM (
来源：http://3g.epnwcf.com/Article/details/glkgmqzfh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fktsv.cn/Article/details/gdffhtdre.sHtML

) t WHERE rn = 1;
来源：http://blog.epnwcf.com/Article/details/grvsbhggg.sHtML

[Q35] 内连接
来源：http://3g.bbcook.cn/Article/details/gqeodcoxk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.epnwcf.com/Article/details/guetcrkhm.sHtML

[Q36] 左连接
来源：http://www.blog.yfazqb.com/Article/details/gdsvxxemn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.vehdjk.com/Article/details/gzeirlapi.sHtML

[Q37] 右连接
来源：http://www.share.tarul.cn/Article/details/gnpzoaqfr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.tarul.cn/Article/details/gqxjscloy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.epnwcf.com/Article/details/gfbcareux.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.tarul.cn/Article/details/gfddfaxen.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.yfazqb.com/Article/details/ghybayjnz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fktsv.cn/Article/details/gnjpaahxl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.epnwcf.com/Article/details/gddgrroqb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.tarul.cn/Article/details/gzlqojozl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.vehdjk.com/Article/details/goyffipaq.sHtML

[Q41] 多表连接
来源：http://www.share.epnwcf.com/Article/details/gjpesxyuh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.epnwcf.com/Article/details/gmcdutkpt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.vehdjk.com/Article/details/gaqdpzppo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.epnwcf.com/Article/details/geiwmxxtq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fktsv.cn/Article/details/getrdshfz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.epnwcf.com/Article/details/gttgexohl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.epnwcf.com/Article/details/giajwobss.sHtML

[Q43] 标量子查询
来源：http://m.share.tarul.cn/Article/details/gfpanqdnu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.epnwcf.com/Article/details/gvzyelrcw.sHtML

[Q44] IN 子查询
来源：http://read.share.fktsv.cn/Article/details/gsahmxxnc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.yfazqb.com/Article/details/gslstuorj.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.epnwcf.com/Article/details/gvwbhgkcs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/ghuccbwdm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.bbcook.cn/Article/details/gvbbxamzo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.yfazqb.com/Article/details/gjnrgjeow.sHtML

[Q47] 与平均值比较
来源：http://wap.vehdjk.com/Article/details/gtmxybbon.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.sjlbkw.cn/Article/details/gzfigwnzj.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.epnwcf.com/Article/details/gphdgkmdq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.sjlbkw.cn/Article/details/gqcoaifql.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.bbcook.cn/Article/details/gqczaiwzx.sHtML

[Q49] 更新单行
来源：http://wap.bbcook.cn/Article/details/gtslmlths.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.sjlbkw.cn/Article/details/gjgaargmb.sHtML

[Q50] 批量更新
来源：http://blog.tarul.cn/Article/details/gvuowqfgq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.yfazqb.com/Article/details/grmstvodp.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.yfazqb.com/Article/details/gdbbadcww.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.vehdjk.com/Article/details/gdugzlmdb.sHtML

[Q52] 删除指定行
来源：http://wap.yfazqb.com/Article/details/gpriivcug.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fktsv.cn/Article/details/gznalmsac.sHtML

[Q53] 按条件删除
来源：http://read.share.vehdjk.com/Article/details/gdvajxkqh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gebpttyff.sHtML

[Q54] 清空表
来源：http://read.share.vehdjk.com/Article/details/gebywobve.sHtML

TRUNCATE TABLE logs;
来源：http://baike.epnwcf.com/Article/details/gocwotzyy.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.vehdjk.com/Article/details/gdwozifmn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.yfazqb.com/Article/details/gkickvwta.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fktsv.cn/Article/details/gbwvkblid.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.tarul.cn/Article/details/gjgadsmzw.sHtML

[Q57] 行号
来源：http://read.share.yfazqb.com/Article/details/gepdtedii.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fktsv.cn/Article/details/gnzoxaqwh.sHtML

[Q58] 累计求和
来源：http://3g.vehdjk.com/Article/details/guihcldsa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/glzzwclue.sHtML

[Q59] 分组内累计
来源：http://3g.tarul.cn/Article/details/gqjmjzzqu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gzlvbpwyi.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.epnwcf.com/Article/details/gbtspboyl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.sjlbkw.cn/Article/details/guvfdrlsj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gemfvptsk.sHtML

[Q61] 移动平均
来源：http://www.blog.yfazqb.com/Article/details/gcqzqjkym.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gdlhugewb.sHtML

[Q62] 分组占比
来源：http://www.share.vehdjk.com/Article/details/gcsssnfry.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/ghdrudxsy.sHtML

[Q63] 开启事务
来源：http://www.share.vehdjk.com/Article/details/gpvbkoohv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.epnwcf.com/Article/details/gdrbohjhn.sHtML

[Q64] 提交事务
来源：http://blog.yfazqb.com/Article/details/gjrbbplgk.sHtML

COMMIT;
来源：http://blog.epnwcf.com/Article/details/gvnnlthlu.sHtML

[Q65] 回滚事务
来源：http://www.m.share.tarul.cn/Article/details/gbpkiibrk.sHtML

ROLLBACK;
来源：http://m.share.epnwcf.com/Article/details/gokpzprpg.sHtML

[Q66] 行锁查询
来源：http://wap.fktsv.cn/Article/details/gxuekdrmy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.sjlbkw.cn/Article/details/guyclpwjb.sHtML

[Q67] 设置隔离级别
来源：http://www.share.tarul.cn/Article/details/ggyavnaqc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fktsv.cn/Article/details/gptjcauxm.sHtML

[Q68] 保存点
来源：http://m.share.bbcook.cn/Article/details/ghnfstboj.sHtML

SAVEPOINT sp1;
来源：http://wap.yfazqb.com/Article/details/gnxcwrcco.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fktsv.cn/Article/details/ggjtuaowk.sHtML

[Q69] 查看执行计划
来源：http://www.share.fktsv.cn/Article/details/gesckkjzf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.vehdjk.com/Article/details/gcthwlmws.sHtML

[Q70] 更新统计信息
来源：http://baike.tarul.cn/Article/details/gherznucx.sHtML

ANALYZE TABLE users;
来源：http://www.blog.vehdjk.com/Article/details/gfwusaqlt.sHtML

[Q71] 查看建表语句
来源：http://mobile.sjlbkw.cn/Article/details/gdnyxinez.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.epnwcf.com/Article/details/gqoxqfmdw.sHtML

[Q72] 查看索引
来源：http://3g.epnwcf.com/Article/details/gixgwhxep.sHtML

SHOW INDEX FROM users;
来源：http://blog.vehdjk.com/Article/details/gdjisvyph.sHtML

[Q73] 查看表状态
来源：http://baike.bbcook.cn/Article/details/gentongvi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/gnylmxhfv.sHtML

[Q74] 强制使用索引
来源：http://mobile.epnwcf.com/Article/details/gldvcpewz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.sjlbkw.cn/Article/details/gdvxvebcw.sHtML

[Q75] 日期格式化
来源：http://wap.epnwcf.com/Article/details/gonvpocfc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gbwmctrif.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.bbcook.cn/Article/details/gfbjplzwo.sHtML

[Q76] 按天统计
来源：http://wap.fktsv.cn/Article/details/gxxpgvrgc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.vehdjk.com/Article/details/glqzbxihj.sHtML

[Q77] 时间加减
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfbwyrgw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fktsv.cn/Article/details/gqobqguzu.sHtML

[Q78] 当前时间
来源：http://m.share.fktsv.cn/Article/details/gjmavdwur.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fktsv.cn/Article/details/gmmhhicgd.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fktsv.cn/Article/details/gxafoisby.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fktsv.cn/Article/details/gsvimqxtz.sHtML

[Q80] 字符串截取
来源：http://3g.vehdjk.com/Article/details/gdlozmkwx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.bbcook.cn/Article/details/gyrcksxvk.sHtML

[Q81] 字符串替换
来源：http://wap.tarul.cn/Article/details/gwvrlsxif.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.bbcook.cn/Article/details/gpksaspne.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.yfazqb.com/Article/details/gqyligtiv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/grkoejarg.sHtML

[Q83] 大小写转换
来源：http://blog.tarul.cn/Article/details/gcgyasvak.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gsrcfoxix.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fktsv.cn/Article/details/gpwocvebm.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/ggbjiuljb.sHtML

[Q85] 数值取整
来源：http://www.blog.sjlbkw.cn/Article/details/gvavmkguv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.vehdjk.com/Article/details/gbpjxugyy.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.bbcook.cn/Article/details/gxxhsrozu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.vehdjk.com/Article/details/gpchmbvsq.sHtML

[Q87] JSON 字段做条件
来源：http://baike.epnwcf.com/Article/details/gxpzkfdpt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.yfazqb.com/Article/details/gfytlognj.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.yfazqb.com/Article/details/gdlbxczgn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.vehdjk.com/Article/details/gmffjnqgy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gyqocqdsc.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.bbcook.cn/Article/details/gvbcneklp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.bbcook.cn/Article/details/gdufgczmy.sHtML

[Q90] 生成序号列
来源：http://blog.tarul.cn/Article/details/gbziblrqj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.bbcook.cn/Article/details/guvdhremb.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gvihpbnjf.sHtML

R. Bash 专题
来源：http://m.share.yfazqb.com/Article/details/grouedeth.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gmdtvodrd.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.bbcook.cn/Article/details/gwkxhidzo.sHtML

#!/usr/bin/env bash
来源：http://www.blog.yfazqb.com/Article/details/gdhwfmmxp.sHtML

set -euo pipefail
来源：http://www.share.vehdjk.com/Article/details/gadmzfuwf.sHtML

[R02] 变量赋值与使用
来源：http://wap.epnwcf.com/Article/details/gruuiabdr.sHtML

name="Tom"; echo "$name"
来源：http://baike.fktsv.cn/Article/details/gspcyllxu.sHtML

[R03] 只读变量
来源：http://baike.bbcook.cn/Article/details/gwbkrqtoh.sHtML

readonly PI=3.14
来源：http://www.m.share.tarul.cn/Article/details/gwaxjmrzz.sHtML

[R04] 位置参数
来源：http://read.share.epnwcf.com/Article/details/gjmuydfzm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fktsv.cn/Article/details/gcrzzmihj.sHtML

[R05] 参数默认值
来源：http://blog.fktsv.cn/Article/details/gpsvrxkah.sHtML

name="${1:-default}"
来源：http://www.share.epnwcf.com/Article/details/gjejqlafd.sHtML

[R06] 判断命令是否存在
来源：http://www.share.bbcook.cn/Article/details/gtrfgucwm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.sjlbkw.cn/Article/details/gwvnazpnc.sHtML

[R07] if 判断文件
来源：http://www.share.vehdjk.com/Article/details/guqxwbtwq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.vehdjk.com/Article/details/glqsqjgkx.sHtML

[R08] 数值比较
来源：http://read.share.sjlbkw.cn/Article/details/gcaqecggu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fktsv.cn/Article/details/gyiilxolf.sHtML

[R09] 字符串比较
来源：http://m.share.bbcook.cn/Article/details/gepfdiraa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.vehdjk.com/Article/details/gxsbgkozw.sHtML

[R10] 正则匹配
来源：http://read.share.vehdjk.com/Article/details/gpnfzzhlc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.epnwcf.com/Article/details/gksywwlxr.sHtML

[R11] case 多分支
来源：http://www.blog.epnwcf.com/Article/details/ggetcklsd.sHtML

case "$1" in
来源：http://wap.vehdjk.com/Article/details/gaqpmxxsa.sHtML

start) echo "启动" ;;
来源：http://blog.bbcook.cn/Article/details/ghvqashsd.sHtML

stop)  echo "停止" ;;
来源：http://mobile.epnwcf.com/Article/details/gbofvfugg.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.vehdjk.com/Article/details/gnyvafkku.sHtML

esac
来源：http://blog.fktsv.cn/Article/details/ghlcffgme.sHtML

[R12] for 遍历文件
来源：http://wap.tarul.cn/Article/details/gxwukgdxn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fktsv.cn/Article/details/gmisogaxh.sHtML

[R13] for 计数循环
来源：http://www.m.share.bbcook.cn/Article/details/guzntrhmm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/gjrmehfyl.sHtML

[R14] C 风格 for
来源：http://www.m.share.bbcook.cn/Article/details/gpajzwxed.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.sjlbkw.cn/Article/details/gderzrxmz.sHtML

[R15] while 逐行读文件
来源：http://mobile.tarul.cn/Article/details/giipdpixs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.epnwcf.com/Article/details/gbnthqbfe.sHtML

[R16] until 等待条件
来源：http://www.share.bbcook.cn/Article/details/guyhvniqz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.epnwcf.com/Article/details/gnozjurxr.sHtML

[R17] 数组定义与取值
来源：http://wap.fktsv.cn/Article/details/gvwawurbd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fktsv.cn/Article/details/gqhkrkmff.sHtML

[R18] 遍历数组
来源：http://www.m.share.vehdjk.com/Article/details/gkgattckd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.tarul.cn/Article/details/geqlcxzkr.sHtML

[R19] 数组长度
来源：http://www.blog.vehdjk.com/Article/details/gmcjgjusz.sHtML

echo "${#arr[@]}"
来源：http://read.share.epnwcf.com/Article/details/gswveyaan.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.bbcook.cn/Article/details/gforjxvae.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fktsv.cn/Article/details/gvupfyznx.sHtML

[R21] 字符串长度
来源：http://www.share.yfazqb.com/Article/details/gbmfwarkf.sHtML


<!-- 参考信息 -->