代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.epnwcf.com/Article/details/gxcplyjop.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gxzjthvsp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.sjlbkw.cn/Article/details/gkylcxtwp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.epnwcf.com/Article/details/gsfsodxip.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.epnwcf.com/Article/details/gvoscpymz.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.sjlbkw.cn/Article/details/gvlawavxd.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fktsv.cn/Article/details/gdcwpuiwh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fktsv.cn/Article/details/gcdyoaxcc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.epnwcf.com/Article/details/gfhyywzqs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.yfazqb.com/Article/details/gqydxraow.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.bbcook.cn/Article/details/gjfvixhhv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fktsv.cn/Article/details/gypxgizer.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.yfazqb.com/Article/details/gvzmmoyxp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.vehdjk.com/Article/details/gwllmzfxm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.vehdjk.com/Article/details/gssuukwxm.sHtML

Ruby: a == b
来源：http://read.share.bbcook.cn/Article/details/gbopmsqjo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fktsv.cn/Article/details/ghpwzmnmk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.sjlbkw.cn/Article/details/gwqnfjlgj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.epnwcf.com/Article/details/gsgzpilun.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.vehdjk.com/Article/details/gqmuqvfeh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.sjlbkw.cn/Article/details/gkdfebmag.sHtML

TS:   if (x == null) {}
来源：http://mobile.yfazqb.com/Article/details/gcknyhjgd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fktsv.cn/Article/details/gptrvlwuv.sHtML

Go:   if x == nil {}
来源：http://wap.epnwcf.com/Article/details/gfjcxqbzc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.sjlbkw.cn/Article/details/gjcpcpuda.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.epnwcf.com/Article/details/gqychuhuv.sHtML

[P07] 防抖与节流
来源：http://www.share.tarul.cn/Article/details/gyerrzcet.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.vehdjk.com/Article/details/grmccxvvz.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fktsv.cn/Article/details/gwxhobbdw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gpztgklpq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gzukfkoai.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.yfazqb.com/Article/details/grwvaictw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fktsv.cn/Article/details/ghqbnzuiy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.vehdjk.com/Article/details/gwcqmnyva.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.tarul.cn/Article/details/ggaquguhc.sHtML

[P08] 处理浮点精度问题
来源：http://wap.epnwcf.com/Article/details/gvbjttxtz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.vehdjk.com/Article/details/gwwclbttd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.sjlbkw.cn/Article/details/gamthvxye.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.tarul.cn/Article/details/grigvzqvz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.tarul.cn/Article/details/gxgzsbfyi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.tarul.cn/Article/details/gfhhryckx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.epnwcf.com/Article/details/gzzxbnqxw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.tarul.cn/Article/details/gfijasjpb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.tarul.cn/Article/details/gfaguiicd.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gxdrctnch.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fktsv.cn/Article/details/gfeqqtvbg.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gvwlexxwy.sHtML

[Q01] 创建表
来源：http://wap.sjlbkw.cn/Article/details/grvqdcmct.sHtML

CREATE TABLE users (
来源：http://baike.tarul.cn/Article/details/ghhyknmpf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/goygrihwd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.vehdjk.com/Article/details/gukuxvvgg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.epnwcf.com/Article/details/gzukczgkf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.yfazqb.com/Article/details/gybjmrhou.sHtML

);
来源：http://read.share.epnwcf.com/Article/details/gaucowqna.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.epnwcf.com/Article/details/gctcycjub.sHtML

CREATE TABLE orders (
来源：http://mobile.epnwcf.com/Article/details/gmmitaobl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.epnwcf.com/Article/details/gicllzcob.sHtML

user_id INT NOT NULL,
来源：http://baike.bbcook.cn/Article/details/gfioszhfj.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.sjlbkw.cn/Article/details/gpkyfjkan.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.bbcook.cn/Article/details/gwjboqvbo.sHtML

);
来源：http://mobile.vehdjk.com/Article/details/gwrcwdkka.sHtML

[Q03] 增加列
来源：http://mobile.sjlbkw.cn/Article/details/gcavvbuok.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.tarul.cn/Article/details/gcwfdhnty.sHtML

[Q04] 修改列类型
来源：http://mobile.epnwcf.com/Article/details/gezanohgp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.tarul.cn/Article/details/gnmbnftaf.sHtML

[Q05] 重命名列
来源：http://read.share.bbcook.cn/Article/details/gxyhowtka.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.sjlbkw.cn/Article/details/gsovqdvvh.sHtML

[Q06] 删除列
来源：http://m.share.vehdjk.com/Article/details/gwqzueadk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.yfazqb.com/Article/details/gggphqsxt.sHtML

[Q07] 删除表
来源：http://blog.epnwcf.com/Article/details/ginjlqnzf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.yfazqb.com/Article/details/gzdphgrjk.sHtML

[Q08] 创建普通索引
来源：http://www.blog.epnwcf.com/Article/details/gftsoqipj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.vehdjk.com/Article/details/gedxykjwo.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.yfazqb.com/Article/details/gxtdihsct.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.yfazqb.com/Article/details/gfwohskqr.sHtML

[Q10] 插入单行
来源：http://wap.yfazqb.com/Article/details/gbyjacwsn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fktsv.cn/Article/details/gvisuctpy.sHtML

[Q11] 一次插入多行
来源：http://read.share.epnwcf.com/Article/details/glcsjswdm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.tarul.cn/Article/details/gzrfwxkcl.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.bbcook.cn/Article/details/gsxmlraxu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.tarul.cn/Article/details/gslilxqdf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.vehdjk.com/Article/details/gwhzbzmfk.sHtML

[Q13] 忽略重复插入
来源：http://wap.sjlbkw.cn/Article/details/glmohrqib.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gngfwwcex.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.yfazqb.com/Article/details/gblfpqwrf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.epnwcf.com/Article/details/gfamomhhf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.bbcook.cn/Article/details/gmxnfzxbg.sHtML

[Q15] 查询全部
来源：http://mobile.vehdjk.com/Article/details/grtxslehv.sHtML

SELECT * FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/golpewsum.sHtML

[Q16] 查询指定列
来源：http://wap.bbcook.cn/Article/details/gwhhlwpjd.sHtML

SELECT id, name FROM users;
来源：http://read.share.yfazqb.com/Article/details/gsgnlgqda.sHtML

[Q17] 条件查询
来源：http://www.blog.epnwcf.com/Article/details/ggaznicaw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fktsv.cn/Article/details/gtjxymxll.sHtML

[Q18] 模糊匹配
来源：http://m.share.epnwcf.com/Article/details/gkdeahxkp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.yfazqb.com/Article/details/gjikbifra.sHtML

[Q19] 范围查询
来源：http://blog.bbcook.cn/Article/details/gynumzngh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fktsv.cn/Article/details/gspztkeyf.sHtML

[Q20] IN 列表
来源：http://m.share.bbcook.cn/Article/details/ggafivtki.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.vehdjk.com/Article/details/guuoviyux.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/guygjucwi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.yfazqb.com/Article/details/ginnugmbq.sHtML

[Q22] 排序
来源：http://m.share.sjlbkw.cn/Article/details/ggdakztcj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fktsv.cn/Article/details/guafamrxf.sHtML

[Q23] 分页
来源：http://www.m.share.fktsv.cn/Article/details/gycgcpoip.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.epnwcf.com/Article/details/gjyjiizsl.sHtML

[Q24] 去重
来源：http://mobile.epnwcf.com/Article/details/gbzfyblsw.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.yfazqb.com/Article/details/gixvtyafx.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.tarul.cn/Article/details/glcvgfsyr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.bbcook.cn/Article/details/gddoxzhvj.sHtML

[Q26] 计数
来源：http://read.share.bbcook.cn/Article/details/gpqetwwzc.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.yfazqb.com/Article/details/gsfibipng.sHtML

[Q27] 条件计数
来源：http://mobile.tarul.cn/Article/details/gukbcxoir.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.yfazqb.com/Article/details/gncgooaue.sHtML

[Q28] 求和与平均
来源：http://www.blog.sjlbkw.cn/Article/details/gbipqgitd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.tarul.cn/Article/details/gelzdespi.sHtML

[Q29] 最大最小值
来源：http://www.share.sjlbkw.cn/Article/details/gngjyyfpn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gzpxkmslj.sHtML

[Q30] 分组统计
来源：http://blog.epnwcf.com/Article/details/gezrlajfd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gnqfsveck.sHtML

[Q31] 分组后过滤
来源：http://mobile.vehdjk.com/Article/details/gfbvbcovw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.tarul.cn/Article/details/gwuafktje.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.epnwcf.com/Article/details/gcwmpwjnf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/gujtjhdzh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.vehdjk.com/Article/details/gmulvpmnm.sHtML

[Q33] 多列分组
来源：http://www.share.bbcook.cn/Article/details/gdvplleqi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.yfazqb.com/Article/details/ggfbiaglj.sHtML

[Q34] 每组取第一条
来源：http://read.share.yfazqb.com/Article/details/gpyxeqpmc.sHtML

SELECT * FROM (
来源：http://www.share.tarul.cn/Article/details/gklbltcns.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.vehdjk.com/Article/details/gpdbcbspv.sHtML

) t WHERE rn = 1;
来源：http://wap.fktsv.cn/Article/details/gamxlkxzy.sHtML

[Q35] 内连接
来源：http://read.share.sjlbkw.cn/Article/details/gkurpnpwv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.yfazqb.com/Article/details/gxnmywbgv.sHtML

[Q36] 左连接
来源：http://m.share.tarul.cn/Article/details/gibxpcumo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.sjlbkw.cn/Article/details/gwrfxuztd.sHtML

[Q37] 右连接
来源：http://mobile.yfazqb.com/Article/details/gnzpnlqzd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.vehdjk.com/Article/details/gwxlrhnhk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fktsv.cn/Article/details/gzjclfwgj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.vehdjk.com/Article/details/gohmddmwo.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fktsv.cn/Article/details/gtrposxnk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.tarul.cn/Article/details/gcxyqwpid.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.vehdjk.com/Article/details/gddwqqrxx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.sjlbkw.cn/Article/details/gplvqdwov.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.yfazqb.com/Article/details/ggpuatvie.sHtML

[Q41] 多表连接
来源：http://blog.fktsv.cn/Article/details/gugpqpefy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.epnwcf.com/Article/details/gruqqljwk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.yfazqb.com/Article/details/gegladkpd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.sjlbkw.cn/Article/details/gbvxlqggw.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.tarul.cn/Article/details/gsoeitbyb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.yfazqb.com/Article/details/gztpnxddr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.bbcook.cn/Article/details/giyxwroyo.sHtML

[Q43] 标量子查询
来源：http://www.blog.fktsv.cn/Article/details/gyjbbhsqd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.tarul.cn/Article/details/gedeeawjq.sHtML

[Q44] IN 子查询
来源：http://www.blog.bbcook.cn/Article/details/gdwjopodv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.sjlbkw.cn/Article/details/gtxmqvhgs.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.sjlbkw.cn/Article/details/geryslikj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/gehuexekq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.epnwcf.com/Article/details/gaspmxsix.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fktsv.cn/Article/details/guwubebat.sHtML

[Q47] 与平均值比较
来源：http://mobile.fktsv.cn/Article/details/gofbdacjz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.yfazqb.com/Article/details/ghufmkaci.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.yfazqb.com/Article/details/gkrzggbat.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.sjlbkw.cn/Article/details/gsviaaopt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.sjlbkw.cn/Article/details/gnakfhivi.sHtML

[Q49] 更新单行
来源：http://baike.epnwcf.com/Article/details/gudcbvcco.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.bbcook.cn/Article/details/gtwuzqrjh.sHtML

[Q50] 批量更新
来源：http://www.share.bbcook.cn/Article/details/gbsosqxkt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.epnwcf.com/Article/details/gfjtqnayp.sHtML

[Q51] 用子查询更新
来源：http://baike.epnwcf.com/Article/details/gxqincuom.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.sjlbkw.cn/Article/details/gowoefzoz.sHtML

[Q52] 删除指定行
来源：http://www.blog.vehdjk.com/Article/details/gufwlqtpt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.sjlbkw.cn/Article/details/gmuxlfecd.sHtML

[Q53] 按条件删除
来源：http://baike.yfazqb.com/Article/details/ghosknmea.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.vehdjk.com/Article/details/goybccgrf.sHtML

[Q54] 清空表
来源：http://www.m.share.fktsv.cn/Article/details/gqervjlll.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.tarul.cn/Article/details/gyvgqlakr.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.tarul.cn/Article/details/giiiarrix.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.vehdjk.com/Article/details/gwkdrqert.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.yfazqb.com/Article/details/gprnscqjd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.bbcook.cn/Article/details/gdmmvmcvr.sHtML

[Q57] 行号
来源：http://baike.bbcook.cn/Article/details/gsvjmvgfl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gwsuwzqra.sHtML

[Q58] 累计求和
来源：http://www.m.share.vehdjk.com/Article/details/ggqiecqqv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.yfazqb.com/Article/details/gzueqtjqt.sHtML

[Q59] 分组内累计
来源：http://blog.epnwcf.com/Article/details/gitqazspi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gmvqtsgue.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.bbcook.cn/Article/details/gkupfocjh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.sjlbkw.cn/Article/details/gnifapsfl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.yfazqb.com/Article/details/gkhfmqyfu.sHtML

[Q61] 移动平均
来源：http://wap.fktsv.cn/Article/details/gzruxxnvp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gwsyogojc.sHtML

[Q62] 分组占比
来源：http://blog.vehdjk.com/Article/details/goxnmhzfz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/gypsfjmgd.sHtML

[Q63] 开启事务
来源：http://wap.bbcook.cn/Article/details/gmhpapmmf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.bbcook.cn/Article/details/goyibontf.sHtML

[Q64] 提交事务
来源：http://www.share.vehdjk.com/Article/details/goxcgjvgn.sHtML

COMMIT;
来源：http://read.share.sjlbkw.cn/Article/details/gwrkvthbg.sHtML

[Q65] 回滚事务
来源：http://baike.bbcook.cn/Article/details/gyrumnbfx.sHtML

ROLLBACK;
来源：http://mobile.sjlbkw.cn/Article/details/gonhasswx.sHtML

[Q66] 行锁查询
来源：http://3g.bbcook.cn/Article/details/gfgwsvwos.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.vehdjk.com/Article/details/giwgyckvs.sHtML

[Q67] 设置隔离级别
来源：http://read.share.bbcook.cn/Article/details/gfunwyrwe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.epnwcf.com/Article/details/gqrroyilu.sHtML

[Q68] 保存点
来源：http://3g.fktsv.cn/Article/details/grbwarbcn.sHtML

SAVEPOINT sp1;
来源：http://mobile.yfazqb.com/Article/details/gxlfatvpw.sHtML

ROLLBACK TO sp1;
来源：http://mobile.bbcook.cn/Article/details/gesuwbbho.sHtML

[Q69] 查看执行计划
来源：http://baike.fktsv.cn/Article/details/guniondqr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.epnwcf.com/Article/details/gstikwobc.sHtML

[Q70] 更新统计信息
来源：http://m.share.bbcook.cn/Article/details/gcitwfkci.sHtML

ANALYZE TABLE users;
来源：http://m.share.epnwcf.com/Article/details/gshfpwpco.sHtML

[Q71] 查看建表语句
来源：http://wap.epnwcf.com/Article/details/gkkghdhmx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.vehdjk.com/Article/details/guekfhewl.sHtML

[Q72] 查看索引
来源：http://www.m.share.tarul.cn/Article/details/gxunfecwo.sHtML

SHOW INDEX FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gwuitisws.sHtML

[Q73] 查看表状态
来源：http://blog.yfazqb.com/Article/details/gyfkbepug.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.tarul.cn/Article/details/gjusyyeky.sHtML

[Q74] 强制使用索引
来源：http://www.share.epnwcf.com/Article/details/gvnlmuoca.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.bbcook.cn/Article/details/gdvbnwufp.sHtML

[Q75] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gahwtsljo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gmohelijq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.bbcook.cn/Article/details/gzzqvhnge.sHtML

[Q76] 按天统计
来源：http://www.m.share.bbcook.cn/Article/details/gbszivmab.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.vehdjk.com/Article/details/gxkysrqyo.sHtML

[Q77] 时间加减
来源：http://read.share.vehdjk.com/Article/details/gcqkmcxyo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.vehdjk.com/Article/details/gkuehgihh.sHtML

[Q78] 当前时间
来源：http://www.m.share.epnwcf.com/Article/details/gfzqsvjrp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.epnwcf.com/Article/details/gukqpnohe.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/gkjhemitc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.tarul.cn/Article/details/gbkzwlbqo.sHtML

[Q80] 字符串截取
来源：http://wap.epnwcf.com/Article/details/ggwmfdyde.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gyqdyekxd.sHtML

[Q81] 字符串替换
来源：http://mobile.epnwcf.com/Article/details/gerswldds.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.yfazqb.com/Article/details/gdcughfut.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.epnwcf.com/Article/details/gvdlnwmmk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/gxltzhtls.sHtML

[Q83] 大小写转换
来源：http://3g.vehdjk.com/Article/details/gzaobrgcy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gdbxsgdvs.sHtML

[Q84] 去除首尾空格
来源：http://www.share.vehdjk.com/Article/details/gwkwvtzlm.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/glbibsltl.sHtML

[Q85] 数值取整
来源：http://www.blog.vehdjk.com/Article/details/gbcwvgkdh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.sjlbkw.cn/Article/details/gtkjplcjx.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.yfazqb.com/Article/details/gfndinhpu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.vehdjk.com/Article/details/gtfyltwkl.sHtML

[Q87] JSON 字段做条件
来源：http://wap.yfazqb.com/Article/details/gilajdzwp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fktsv.cn/Article/details/gzedreocc.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fktsv.cn/Article/details/gosuytzol.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.epnwcf.com/Article/details/gxolfvqhi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gthwuuuwa.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/grihorjlw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.epnwcf.com/Article/details/gfuyhhyyc.sHtML

[Q90] 生成序号列
来源：http://3g.yfazqb.com/Article/details/glemecvrl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.vehdjk.com/Article/details/gfgehtawj.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gxcpdeuvo.sHtML

R. Bash 专题
来源：http://www.m.share.vehdjk.com/Article/details/gqnoktzpm.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gofoguwym.sHtML

[R01] shebang 与严格模式
来源：http://mobile.bbcook.cn/Article/details/gcdkezayp.sHtML

#!/usr/bin/env bash
来源：http://3g.fktsv.cn/Article/details/gwhqzsezv.sHtML

set -euo pipefail
来源：http://www.m.share.tarul.cn/Article/details/gqipfzhzj.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.yfazqb.com/Article/details/gwkfajpwb.sHtML

name="Tom"; echo "$name"
来源：http://m.share.sjlbkw.cn/Article/details/goebegkbr.sHtML

[R03] 只读变量
来源：http://3g.bbcook.cn/Article/details/gqjnehkwa.sHtML

readonly PI=3.14
来源：http://www.m.share.bbcook.cn/Article/details/gryazipeo.sHtML

[R04] 位置参数
来源：http://read.share.vehdjk.com/Article/details/gddxupypd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.sjlbkw.cn/Article/details/gmhqainnm.sHtML

[R05] 参数默认值
来源：http://read.share.vehdjk.com/Article/details/gccdrsvky.sHtML

name="${1:-default}"
来源：http://www.m.share.fktsv.cn/Article/details/gpnyaivkq.sHtML

[R06] 判断命令是否存在
来源：http://www.share.vehdjk.com/Article/details/gbrbvcmpx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.bbcook.cn/Article/details/ggmihpblr.sHtML

[R07] if 判断文件
来源：http://www.m.share.vehdjk.com/Article/details/gvfdnzngj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fktsv.cn/Article/details/ghrvppokq.sHtML

[R08] 数值比较
来源：http://blog.epnwcf.com/Article/details/glvtprhoh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.tarul.cn/Article/details/gbfhkdxks.sHtML

[R09] 字符串比较
来源：http://wap.bbcook.cn/Article/details/gktqxlebm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.sjlbkw.cn/Article/details/goihfgghi.sHtML

[R10] 正则匹配
来源：http://read.share.vehdjk.com/Article/details/gpldauemw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.sjlbkw.cn/Article/details/gcsfxriio.sHtML

[R11] case 多分支
来源：http://blog.epnwcf.com/Article/details/gukomrurh.sHtML

case "$1" in
来源：http://blog.fktsv.cn/Article/details/giqumfivp.sHtML

start) echo "启动" ;;
来源：http://3g.bbcook.cn/Article/details/glxldeyiv.sHtML

stop)  echo "停止" ;;
来源：http://wap.vehdjk.com/Article/details/grjrqysxe.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.epnwcf.com/Article/details/glpwcvlvv.sHtML

esac
来源：http://mobile.epnwcf.com/Article/details/gyodgeroy.sHtML

[R12] for 遍历文件
来源：http://www.m.share.vehdjk.com/Article/details/gpaqccrts.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.yfazqb.com/Article/details/gpmoddnvx.sHtML

[R13] for 计数循环
来源：http://m.share.epnwcf.com/Article/details/gavwylqej.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gdisdzhpg.sHtML

[R14] C 风格 for
来源：http://3g.epnwcf.com/Article/details/gwnkovwyj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.sjlbkw.cn/Article/details/gxbezfjoc.sHtML

[R15] while 逐行读文件
来源：http://blog.bbcook.cn/Article/details/ggbiqcjvt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.vehdjk.com/Article/details/gljnrpiuy.sHtML

[R16] until 等待条件
来源：http://wap.epnwcf.com/Article/details/gweyhkjjn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.vehdjk.com/Article/details/ggnremeqy.sHtML

[R17] 数组定义与取值
来源：http://baike.yfazqb.com/Article/details/gywzbyonz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.bbcook.cn/Article/details/gwtexoahc.sHtML

[R18] 遍历数组
来源：http://mobile.yfazqb.com/Article/details/gsycekdcb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.epnwcf.com/Article/details/guqerdewi.sHtML

[R19] 数组长度
来源：http://baike.yfazqb.com/Article/details/ghnlnudgn.sHtML

echo "${#arr[@]}"
来源：http://wap.epnwcf.com/Article/details/girlzmfhr.sHtML

[R20] 关联数组（字典）
来源：http://wap.epnwcf.com/Article/details/gitzlrnad.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.vehdjk.com/Article/details/gmmiizhht.sHtML

[R21] 字符串长度
来源：http://mobile.bbcook.cn/Article/details/ggcaxdpwr.sHtML


<!-- 参考信息 -->