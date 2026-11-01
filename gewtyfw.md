代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fktsv.cn/Article/details/gkfpvlvoj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.vehdjk.com/Article/details/gkvkunfda.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/gkgmtnnhq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fktsv.cn/Article/details/gvffjumkv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.vehdjk.com/Article/details/gncgxtpsb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fktsv.cn/Article/details/glrpdnysx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.yfazqb.com/Article/details/gddwubzbj.sHtML

[P04] 求长度
来源：http://read.share.vehdjk.com/Article/details/gvxrlnxjh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.epnwcf.com/Article/details/gaznxxjsn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gnhemlmhr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fktsv.cn/Article/details/gtsvvfcda.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.bbcook.cn/Article/details/glcxvmpdj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.vehdjk.com/Article/details/gnmqawmmb.sHtML

Go:   len(arr);  len(m)
来源：http://3g.bbcook.cn/Article/details/ghtuzvain.sHtML

Ruby: x.length;  x.size
来源：http://blog.fktsv.cn/Article/details/gzjwfepma.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.epnwcf.com/Article/details/gfjracuel.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fktsv.cn/Article/details/geiklclxb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.bbcook.cn/Article/details/gumlbtiml.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.vehdjk.com/Article/details/gmarpdwzb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.tarul.cn/Article/details/gvhffjlut.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.yfazqb.com/Article/details/gwlcvadqn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fktsv.cn/Article/details/gvkmfhtzy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.vehdjk.com/Article/details/gwirkdtif.sHtML

Ruby: a == b
来源：http://3g.sjlbkw.cn/Article/details/gvxhxcris.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fktsv.cn/Article/details/gsovmcgkn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.yfazqb.com/Article/details/gwxgislcl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.sjlbkw.cn/Article/details/gjunzezgm.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.vehdjk.com/Article/details/gzcopmdbf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.yfazqb.com/Article/details/gxdcqegza.sHtML

TS:   if (x == null) {}
来源：http://baike.vehdjk.com/Article/details/gwvygpcri.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.sjlbkw.cn/Article/details/giuwtkkai.sHtML

Go:   if x == nil {}
来源：http://blog.sjlbkw.cn/Article/details/gaobaxepb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.tarul.cn/Article/details/grsbbfbff.sHtML

C#:   if (x is null) {}
来源：http://mobile.bbcook.cn/Article/details/ggactsblr.sHtML

[P07] 防抖与节流
来源：http://m.share.sjlbkw.cn/Article/details/grfxphgqa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.sjlbkw.cn/Article/details/gzdncasii.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.vehdjk.com/Article/details/gvaniijrf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/gpwykysmf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.yfazqb.com/Article/details/grwpnedgc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.yfazqb.com/Article/details/gaiwvlvxi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.vehdjk.com/Article/details/gvbqujgeh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.yfazqb.com/Article/details/gerqgxmtx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.bbcook.cn/Article/details/gahfwryup.sHtML

[P08] 处理浮点精度问题
来源：http://wap.yfazqb.com/Article/details/gpjdyzksr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.yfazqb.com/Article/details/gdxlqbefi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.bbcook.cn/Article/details/ggptolbmn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.tarul.cn/Article/details/gpkemktpy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.epnwcf.com/Article/details/gnhddzsgz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.bbcook.cn/Article/details/gemcjxwds.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.vehdjk.com/Article/details/ghayffyiz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.vehdjk.com/Article/details/gftxwcgoh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.vehdjk.com/Article/details/gfyjwqivv.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gedfmsjlw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.vehdjk.com/Article/details/gzjwvzyso.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ggrpomtws.sHtML

[Q01] 创建表
来源：http://baike.vehdjk.com/Article/details/gpfjtupbx.sHtML

CREATE TABLE users (
来源：http://www.blog.epnwcf.com/Article/details/gwkuzkuxu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.epnwcf.com/Article/details/godapcaxf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.sjlbkw.cn/Article/details/geestwbkm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.bbcook.cn/Article/details/gjtarxiis.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fktsv.cn/Article/details/ggxpqhmsn.sHtML

);
来源：http://3g.tarul.cn/Article/details/gffyoebio.sHtML

[Q02] 创建带外键的表
来源：http://www.share.vehdjk.com/Article/details/gbzjoeqox.sHtML

CREATE TABLE orders (
来源：http://wap.vehdjk.com/Article/details/gyctxtmmd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.sjlbkw.cn/Article/details/gussfpdlf.sHtML

user_id INT NOT NULL,
来源：http://m.share.sjlbkw.cn/Article/details/gnpsdfdqn.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.epnwcf.com/Article/details/gzmgulqan.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.epnwcf.com/Article/details/gukfwiwkq.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/gylyobbei.sHtML

[Q03] 增加列
来源：http://m.share.fktsv.cn/Article/details/guzvyafql.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fktsv.cn/Article/details/gnepugymi.sHtML

[Q04] 修改列类型
来源：http://mobile.sjlbkw.cn/Article/details/gysbjskdv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.vehdjk.com/Article/details/gwbpnabkb.sHtML

[Q05] 重命名列
来源：http://m.share.sjlbkw.cn/Article/details/gjhbpeczv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.tarul.cn/Article/details/gqvqwgzfq.sHtML

[Q06] 删除列
来源：http://wap.tarul.cn/Article/details/gdzrzozpw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.epnwcf.com/Article/details/gdzmonplu.sHtML

[Q07] 删除表
来源：http://wap.fktsv.cn/Article/details/gbovolccz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.tarul.cn/Article/details/gcquzjdlq.sHtML

[Q08] 创建普通索引
来源：http://www.share.sjlbkw.cn/Article/details/gsxbgyggn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/gqjqslzus.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fktsv.cn/Article/details/gbcvhsyzz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.yfazqb.com/Article/details/gpkgvmwjx.sHtML

[Q10] 插入单行
来源：http://baike.vehdjk.com/Article/details/gqnlszqjv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.bbcook.cn/Article/details/gowsodpjy.sHtML

[Q11] 一次插入多行
来源：http://blog.vehdjk.com/Article/details/gekkwoshe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.sjlbkw.cn/Article/details/gfwgotvjz.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.epnwcf.com/Article/details/gghfjlzvm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.sjlbkw.cn/Article/details/gcxeljcgk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fktsv.cn/Article/details/gkqftphtg.sHtML

[Q13] 忽略重复插入
来源：http://mobile.vehdjk.com/Article/details/geuszkeho.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gahebdepm.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.epnwcf.com/Article/details/gqvjwvaqe.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.vehdjk.com/Article/details/gwjtbxejq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fktsv.cn/Article/details/gqupnozik.sHtML

[Q15] 查询全部
来源：http://read.share.tarul.cn/Article/details/gkhduatfy.sHtML

SELECT * FROM users;
来源：http://3g.fktsv.cn/Article/details/gveahwyun.sHtML

[Q16] 查询指定列
来源：http://3g.tarul.cn/Article/details/geazjqvvs.sHtML

SELECT id, name FROM users;
来源：http://baike.bbcook.cn/Article/details/glpzxczci.sHtML

[Q17] 条件查询
来源：http://baike.tarul.cn/Article/details/gfmkxptwu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.sjlbkw.cn/Article/details/gqaiwflny.sHtML

[Q18] 模糊匹配
来源：http://www.blog.bbcook.cn/Article/details/gvbiicjvf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.yfazqb.com/Article/details/gslgimihk.sHtML

[Q19] 范围查询
来源：http://m.share.sjlbkw.cn/Article/details/gxnxcpxai.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.tarul.cn/Article/details/gsualunev.sHtML

[Q20] IN 列表
来源：http://3g.yfazqb.com/Article/details/gkeaufjyr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.epnwcf.com/Article/details/gkairnnrr.sHtML

[Q21] 空值判断
来源：http://www.share.epnwcf.com/Article/details/geifgdxvp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.sjlbkw.cn/Article/details/gwxmhjpei.sHtML

[Q22] 排序
来源：http://read.share.tarul.cn/Article/details/gsyznqukg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.sjlbkw.cn/Article/details/gcajwciys.sHtML

[Q23] 分页
来源：http://read.share.tarul.cn/Article/details/gkkkvyyww.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.epnwcf.com/Article/details/gldaehhia.sHtML

[Q24] 去重
来源：http://mobile.yfazqb.com/Article/details/gafnzjrik.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.vehdjk.com/Article/details/glmfcnjxm.sHtML

[Q25] 只取前 N 条
来源：http://read.share.yfazqb.com/Article/details/glpamqcxi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fktsv.cn/Article/details/giettmmmw.sHtML

[Q26] 计数
来源：http://wap.vehdjk.com/Article/details/gypovaczh.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fktsv.cn/Article/details/gezklufhw.sHtML

[Q27] 条件计数
来源：http://www.share.bbcook.cn/Article/details/grszxxicd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.epnwcf.com/Article/details/ghmtxqvuq.sHtML

[Q28] 求和与平均
来源：http://baike.vehdjk.com/Article/details/givmubpkh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.tarul.cn/Article/details/gdgsqhjnh.sHtML

[Q29] 最大最小值
来源：http://mobile.epnwcf.com/Article/details/gcfsrupgk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gugkuwkyf.sHtML

[Q30] 分组统计
来源：http://m.share.yfazqb.com/Article/details/gtpoomvta.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gqsrjkvmi.sHtML

[Q31] 分组后过滤
来源：http://baike.fktsv.cn/Article/details/ganxmfdte.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.vehdjk.com/Article/details/gepnsovgj.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.yfazqb.com/Article/details/gccpxkdxq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gyafxbuox.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.bbcook.cn/Article/details/gdyijatro.sHtML

[Q33] 多列分组
来源：http://mobile.sjlbkw.cn/Article/details/gpplowppi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.tarul.cn/Article/details/gffkmxlkl.sHtML

[Q34] 每组取第一条
来源：http://m.share.sjlbkw.cn/Article/details/gaighlzer.sHtML

SELECT * FROM (
来源：http://www.blog.yfazqb.com/Article/details/ggbzomney.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.tarul.cn/Article/details/gnjhaquty.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gfmtvynwl.sHtML

[Q35] 内连接
来源：http://m.share.vehdjk.com/Article/details/gkhjxlwea.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.sjlbkw.cn/Article/details/gcoazqeop.sHtML

[Q36] 左连接
来源：http://3g.vehdjk.com/Article/details/gctczqxdv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fktsv.cn/Article/details/gwgspjrvz.sHtML

[Q37] 右连接
来源：http://www.share.fktsv.cn/Article/details/gmmencqyh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.yfazqb.com/Article/details/gtyxszcyn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.yfazqb.com/Article/details/gqvkardpl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.vehdjk.com/Article/details/gtanpdned.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fktsv.cn/Article/details/gnulbkydv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.bbcook.cn/Article/details/gkjwtvppj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.sjlbkw.cn/Article/details/gbenxrpqd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fktsv.cn/Article/details/gifrzqgzt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.tarul.cn/Article/details/gtbhpbahm.sHtML

[Q41] 多表连接
来源：http://www.m.share.sjlbkw.cn/Article/details/guevwsbew.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.yfazqb.com/Article/details/gawnxoqnz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.epnwcf.com/Article/details/gafuvxkvm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.vehdjk.com/Article/details/gaoqixcry.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.tarul.cn/Article/details/gvyvazzvf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.epnwcf.com/Article/details/ghiqjxtxz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fktsv.cn/Article/details/gfkkiswyq.sHtML

[Q43] 标量子查询
来源：http://www.blog.sjlbkw.cn/Article/details/gynfkmuzu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.epnwcf.com/Article/details/gliaaqsor.sHtML

[Q44] IN 子查询
来源：http://mobile.epnwcf.com/Article/details/gqttbkkya.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.epnwcf.com/Article/details/grluikjsw.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fktsv.cn/Article/details/gjndvqvvr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.tarul.cn/Article/details/ghpuguiac.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.epnwcf.com/Article/details/glaizqset.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.epnwcf.com/Article/details/gtnhgeccc.sHtML

[Q47] 与平均值比较
来源：http://baike.sjlbkw.cn/Article/details/gpqjkjxhe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fktsv.cn/Article/details/ggxaobqhl.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.vehdjk.com/Article/details/ggmbyhtqm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.epnwcf.com/Article/details/gzdyftloe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.epnwcf.com/Article/details/gltzposxf.sHtML

[Q49] 更新单行
来源：http://m.share.bbcook.cn/Article/details/gkcqrvijd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.tarul.cn/Article/details/gwqacguuz.sHtML

[Q50] 批量更新
来源：http://www.m.share.tarul.cn/Article/details/gdeaaahtu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fktsv.cn/Article/details/ghceoptyi.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvzslpwt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.bbcook.cn/Article/details/gkftxgkga.sHtML

[Q52] 删除指定行
来源：http://blog.yfazqb.com/Article/details/ghelfyqne.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/gdxfekumi.sHtML

[Q53] 按条件删除
来源：http://blog.vehdjk.com/Article/details/gueyxsets.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.tarul.cn/Article/details/gtpwhgdvj.sHtML

[Q54] 清空表
来源：http://baike.vehdjk.com/Article/details/gzkunvdod.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.tarul.cn/Article/details/gvqjaomeu.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.vehdjk.com/Article/details/gbjqbsbct.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fktsv.cn/Article/details/gqgrzljkj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fktsv.cn/Article/details/ggylvoloy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.tarul.cn/Article/details/gjpfdqicg.sHtML

[Q57] 行号
来源：http://3g.sjlbkw.cn/Article/details/glkwpzxok.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gdmvkvngg.sHtML

[Q58] 累计求和
来源：http://www.m.share.yfazqb.com/Article/details/gwcieqmtm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.epnwcf.com/Article/details/gfmlbokgd.sHtML

[Q59] 分组内累计
来源：http://blog.bbcook.cn/Article/details/gmmiozvld.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fktsv.cn/Article/details/gqysqmvfb.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.yfazqb.com/Article/details/giidnimyk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fktsv.cn/Article/details/gjwveypxr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gfypjsezj.sHtML

[Q61] 移动平均
来源：http://m.share.yfazqb.com/Article/details/gezzehfhq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.bbcook.cn/Article/details/giuzzdvqm.sHtML

[Q62] 分组占比
来源：http://read.share.epnwcf.com/Article/details/gkmesyjpl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gioktlbdr.sHtML

[Q63] 开启事务
来源：http://www.m.share.epnwcf.com/Article/details/gkhrzbovs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.bbcook.cn/Article/details/gsspocaex.sHtML

[Q64] 提交事务
来源：http://m.share.epnwcf.com/Article/details/grhpkrzct.sHtML

COMMIT;
来源：http://m.share.vehdjk.com/Article/details/gxjbjkfyq.sHtML

[Q65] 回滚事务
来源：http://www.share.yfazqb.com/Article/details/gtegvobdc.sHtML

ROLLBACK;
来源：http://3g.bbcook.cn/Article/details/gpxgyqpdn.sHtML

[Q66] 行锁查询
来源：http://3g.fktsv.cn/Article/details/gdducmack.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.epnwcf.com/Article/details/gljzqedys.sHtML

[Q67] 设置隔离级别
来源：http://read.share.tarul.cn/Article/details/gglobpfho.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.epnwcf.com/Article/details/ghilzeyhs.sHtML

[Q68] 保存点
来源：http://mobile.fktsv.cn/Article/details/gxmhpaang.sHtML

SAVEPOINT sp1;
来源：http://blog.epnwcf.com/Article/details/gmuwqtdul.sHtML

ROLLBACK TO sp1;
来源：http://www.share.bbcook.cn/Article/details/ghdthkbtj.sHtML

[Q69] 查看执行计划
来源：http://m.share.epnwcf.com/Article/details/gsiqrzuca.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.bbcook.cn/Article/details/gbpwnawbm.sHtML

[Q70] 更新统计信息
来源：http://www.blog.yfazqb.com/Article/details/gbbgcdfpj.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.tarul.cn/Article/details/gxragevws.sHtML

[Q71] 查看建表语句
来源：http://www.blog.epnwcf.com/Article/details/gomjnulyw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.tarul.cn/Article/details/gzujwjocs.sHtML

[Q72] 查看索引
来源：http://www.blog.fktsv.cn/Article/details/gpmraiyoc.sHtML

SHOW INDEX FROM users;
来源：http://www.share.epnwcf.com/Article/details/gqnhwyhqi.sHtML

[Q73] 查看表状态
来源：http://www.m.share.bbcook.cn/Article/details/gonnlsxcv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.bbcook.cn/Article/details/gnchhkrte.sHtML

[Q74] 强制使用索引
来源：http://mobile.yfazqb.com/Article/details/grkabdjfx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.tarul.cn/Article/details/gmnegumuz.sHtML

[Q75] 日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gcxvtsoxx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.vehdjk.com/Article/details/guooeykjk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.epnwcf.com/Article/details/goasskhxo.sHtML

[Q76] 按天统计
来源：http://www.m.share.bbcook.cn/Article/details/gvwbpshrf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.yfazqb.com/Article/details/ghssgzzzr.sHtML

[Q77] 时间加减
来源：http://m.share.fktsv.cn/Article/details/gujflpgla.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.bbcook.cn/Article/details/ggxleyreu.sHtML

[Q78] 当前时间
来源：http://wap.sjlbkw.cn/Article/details/gtmsvsstn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.sjlbkw.cn/Article/details/gelentwpk.sHtML

[Q79] 字符串拼接
来源：http://read.share.fktsv.cn/Article/details/gttqhctig.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.sjlbkw.cn/Article/details/gqfidjttx.sHtML

[Q80] 字符串截取
来源：http://read.share.vehdjk.com/Article/details/gurtnbweo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.bbcook.cn/Article/details/gncfjskdf.sHtML

[Q81] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/gcqaapgdh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fktsv.cn/Article/details/gaewetqox.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.yfazqb.com/Article/details/gdevotunw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gtdhbpgcp.sHtML

[Q83] 大小写转换
来源：http://wap.sjlbkw.cn/Article/details/gwjxzbikh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/graadribg.sHtML

[Q84] 去除首尾空格
来源：http://baike.tarul.cn/Article/details/giqpdlohr.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gbjnethkf.sHtML

[Q85] 数值取整
来源：http://mobile.fktsv.cn/Article/details/gdehtxxis.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.bbcook.cn/Article/details/gouclbxql.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fktsv.cn/Article/details/gedysrohg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.yfazqb.com/Article/details/gykfeqwev.sHtML

[Q87] JSON 字段做条件
来源：http://baike.epnwcf.com/Article/details/gahsasogn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.vehdjk.com/Article/details/gwmgvtdiz.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.yfazqb.com/Article/details/ggzzruqem.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.vehdjk.com/Article/details/gnpcytuwx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fktsv.cn/Article/details/gswnnkjde.sHtML

[Q89] 判断表是否存在
来源：http://m.share.bbcook.cn/Article/details/gwdqpecrx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fktsv.cn/Article/details/gxrtodgob.sHtML

[Q90] 生成序号列
来源：http://m.share.bbcook.cn/Article/details/gasatcspv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.yfazqb.com/Article/details/gpxddmvgk.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gfqfpiuty.sHtML

R. Bash 专题
来源：http://www.blog.vehdjk.com/Article/details/gemxpvzdn.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gbspcswsa.sHtML

[R01] shebang 与严格模式
来源：http://read.share.sjlbkw.cn/Article/details/gkvrvycjp.sHtML

#!/usr/bin/env bash
来源：http://3g.epnwcf.com/Article/details/grljzgslr.sHtML

set -euo pipefail
来源：http://blog.fktsv.cn/Article/details/gbfwejcdx.sHtML

[R02] 变量赋值与使用
来源：http://blog.vehdjk.com/Article/details/gfsrxlgzu.sHtML

name="Tom"; echo "$name"
来源：http://m.share.vehdjk.com/Article/details/grahyrojz.sHtML

[R03] 只读变量
来源：http://www.blog.vehdjk.com/Article/details/gfpyrkxdq.sHtML

readonly PI=3.14
来源：http://www.share.tarul.cn/Article/details/ghqlygwsl.sHtML

[R04] 位置参数
来源：http://blog.sjlbkw.cn/Article/details/gwhepngxz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.epnwcf.com/Article/details/gcrqtyxec.sHtML

[R05] 参数默认值
来源：http://read.share.yfazqb.com/Article/details/gzlpygjcb.sHtML

name="${1:-default}"
来源：http://read.share.epnwcf.com/Article/details/gubuzwfkk.sHtML

[R06] 判断命令是否存在
来源：http://3g.yfazqb.com/Article/details/gdwvrsmua.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.vehdjk.com/Article/details/gkgrcsaoo.sHtML

[R07] if 判断文件
来源：http://baike.bbcook.cn/Article/details/gfpvxwrfj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.yfazqb.com/Article/details/gvxgilxxm.sHtML

[R08] 数值比较
来源：http://mobile.bbcook.cn/Article/details/grdxzcunc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.yfazqb.com/Article/details/gbeumbjqj.sHtML

[R09] 字符串比较
来源：http://www.blog.yfazqb.com/Article/details/ggaxonrww.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.epnwcf.com/Article/details/gymdimnrx.sHtML

[R10] 正则匹配
来源：http://www.share.sjlbkw.cn/Article/details/gizmamwqf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.sjlbkw.cn/Article/details/gjiduwuqs.sHtML

[R11] case 多分支
来源：http://m.share.tarul.cn/Article/details/gplbqpdkw.sHtML

case "$1" in
来源：http://www.blog.yfazqb.com/Article/details/gdanzuadc.sHtML

start) echo "启动" ;;
来源：http://www.blog.tarul.cn/Article/details/gkpvuhifa.sHtML

stop)  echo "停止" ;;
来源：http://baike.fktsv.cn/Article/details/gghiskrku.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fktsv.cn/Article/details/gaapirhoz.sHtML

esac
来源：http://www.blog.sjlbkw.cn/Article/details/gimqghkpd.sHtML

[R12] for 遍历文件
来源：http://www.blog.yfazqb.com/Article/details/gzjvyzozg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.bbcook.cn/Article/details/gpifomjus.sHtML

[R13] for 计数循环
来源：http://blog.bbcook.cn/Article/details/gheiyocqk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.vehdjk.com/Article/details/gwyejmtyq.sHtML

[R14] C 风格 for
来源：http://www.m.share.yfazqb.com/Article/details/ghzhhucry.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.epnwcf.com/Article/details/gxhgxoyhv.sHtML

[R15] while 逐行读文件
来源：http://baike.epnwcf.com/Article/details/gxrwjpcol.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.epnwcf.com/Article/details/gqeoqoadz.sHtML

[R16] until 等待条件
来源：http://www.share.yfazqb.com/Article/details/ghabymypn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.yfazqb.com/Article/details/gdirouekp.sHtML

[R17] 数组定义与取值
来源：http://www.share.vehdjk.com/Article/details/gucxujsxf.sHtML


<!-- 参考信息 -->