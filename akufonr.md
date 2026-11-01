代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gojusagoc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.yfazqb.com/Article/details/gsagqeknj.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gagnfmsxo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.sjlbkw.cn/Article/details/gemoadsfc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fktsv.cn/Article/details/ggshsaxqf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/ggnwcyvlw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.tarul.cn/Article/details/gatbcoztb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.yfazqb.com/Article/details/gtuhwcxco.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.vehdjk.com/Article/details/gnrmlgfwt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.vehdjk.com/Article/details/gfhwretfh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.vehdjk.com/Article/details/ghjhfcacn.sHtML

[P04] 求长度
来源：http://3g.yfazqb.com/Article/details/gmibxpmmh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.epnwcf.com/Article/details/gtjgmjnwk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gomjmwiln.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.tarul.cn/Article/details/gbyqbydey.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.yfazqb.com/Article/details/gelwhqhvn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/gtofvcujy.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.yfazqb.com/Article/details/gwyyaowwd.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.sjlbkw.cn/Article/details/guioopmmn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.yfazqb.com/Article/details/gsxvzaqii.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.epnwcf.com/Article/details/gbstufoeg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.sjlbkw.cn/Article/details/gsvjnuljs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.tarul.cn/Article/details/gtcmweobz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.tarul.cn/Article/details/gmpzmbkub.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.vehdjk.com/Article/details/gbehzmhbo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.vehdjk.com/Article/details/gpmlxcxmu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.sjlbkw.cn/Article/details/gcqqnksog.sHtML

Ruby: a == b
来源：http://mobile.fktsv.cn/Article/details/gzdokuquq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.tarul.cn/Article/details/genmeebrl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fktsv.cn/Article/details/gbglhyddm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.yfazqb.com/Article/details/ggxyoqkdc.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fktsv.cn/Article/details/gyyoxdkng.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fktsv.cn/Article/details/gdcxxvzzr.sHtML

TS:   if (x == null) {}
来源：http://3g.sjlbkw.cn/Article/details/goojzniyg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gsielqwgw.sHtML

Go:   if x == nil {}
来源：http://m.share.epnwcf.com/Article/details/gbavrihtm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.epnwcf.com/Article/details/gjaknygij.sHtML

C#:   if (x is null) {}
来源：http://m.share.bbcook.cn/Article/details/gwhlxburk.sHtML

[P07] 防抖与节流
来源：http://baike.epnwcf.com/Article/details/gbnlxdpoc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.sjlbkw.cn/Article/details/gradpevjt.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.yfazqb.com/Article/details/gbgssssap.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.yfazqb.com/Article/details/gjxwppcmn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gwbchewbw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.vehdjk.com/Article/details/gwpkalnba.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.tarul.cn/Article/details/gpkgeexfn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.sjlbkw.cn/Article/details/gsygequws.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.epnwcf.com/Article/details/glglsuoco.sHtML

[P08] 处理浮点精度问题
来源：http://wap.vehdjk.com/Article/details/gshrlpeud.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.bbcook.cn/Article/details/ggsvcxubu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.vehdjk.com/Article/details/gdomnnaky.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.epnwcf.com/Article/details/ggmausfka.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.epnwcf.com/Article/details/gvqspbupu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgavbhtx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.epnwcf.com/Article/details/gaivfjhiz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.tarul.cn/Article/details/ghznoexkd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fktsv.cn/Article/details/gobgvionm.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gvvhtayee.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.yfazqb.com/Article/details/ghrohgzst.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gfumipazg.sHtML

[Q01] 创建表
来源：http://baike.epnwcf.com/Article/details/gwrupabsh.sHtML

CREATE TABLE users (
来源：http://baike.epnwcf.com/Article/details/gxebqqrro.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.vehdjk.com/Article/details/gixslyhpc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.vehdjk.com/Article/details/ganobspph.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.sjlbkw.cn/Article/details/gftymhrul.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.epnwcf.com/Article/details/gvwryvtpf.sHtML

);
来源：http://m.share.sjlbkw.cn/Article/details/gsflvdovu.sHtML

[Q02] 创建带外键的表
来源：http://wap.bbcook.cn/Article/details/gswfqdroj.sHtML

CREATE TABLE orders (
来源：http://wap.sjlbkw.cn/Article/details/gxnuhvcau.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fktsv.cn/Article/details/gyrejtjnt.sHtML

user_id INT NOT NULL,
来源：http://baike.yfazqb.com/Article/details/gtaexchcz.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fktsv.cn/Article/details/ghpbffgod.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.bbcook.cn/Article/details/gtdznblix.sHtML

);
来源：http://www.blog.epnwcf.com/Article/details/gqcifgaoi.sHtML

[Q03] 增加列
来源：http://blog.fktsv.cn/Article/details/gthiuiljt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.yfazqb.com/Article/details/gpxqofgpj.sHtML

[Q04] 修改列类型
来源：http://3g.bbcook.cn/Article/details/gjjbggawq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.tarul.cn/Article/details/gmxihnlhk.sHtML

[Q05] 重命名列
来源：http://baike.epnwcf.com/Article/details/gcuvrpngh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.epnwcf.com/Article/details/gkojailmq.sHtML

[Q06] 删除列
来源：http://read.share.epnwcf.com/Article/details/gfpgfloos.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.epnwcf.com/Article/details/gpuoceqku.sHtML

[Q07] 删除表
来源：http://3g.fktsv.cn/Article/details/gcoowflwy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.yfazqb.com/Article/details/ggocrtajt.sHtML

[Q08] 创建普通索引
来源：http://read.share.tarul.cn/Article/details/gawydhimf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.sjlbkw.cn/Article/details/ghvgaipnz.sHtML

[Q09] 创建唯一索引
来源：http://3g.vehdjk.com/Article/details/gtjznfgan.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.vehdjk.com/Article/details/gnpzuuzna.sHtML

[Q10] 插入单行
来源：http://www.share.bbcook.cn/Article/details/gwegvouzt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fktsv.cn/Article/details/ggvgtmvlr.sHtML

[Q11] 一次插入多行
来源：http://read.share.tarul.cn/Article/details/gsupheryf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/grnwfbqfo.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fktsv.cn/Article/details/girdrsgro.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.vehdjk.com/Article/details/gbvjvodly.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.sjlbkw.cn/Article/details/gspxtvqgr.sHtML

[Q13] 忽略重复插入
来源：http://3g.epnwcf.com/Article/details/gdxuevnrr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.tarul.cn/Article/details/grdyyxnlb.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.tarul.cn/Article/details/gswrmkrab.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.sjlbkw.cn/Article/details/ggsbhyjyl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.bbcook.cn/Article/details/ggvptncyl.sHtML

[Q15] 查询全部
来源：http://wap.tarul.cn/Article/details/giajqxdaq.sHtML

SELECT * FROM users;
来源：http://wap.epnwcf.com/Article/details/gecyhvkie.sHtML

[Q16] 查询指定列
来源：http://baike.fktsv.cn/Article/details/gnbmtavwu.sHtML

SELECT id, name FROM users;
来源：http://baike.tarul.cn/Article/details/gcsrdwudb.sHtML

[Q17] 条件查询
来源：http://baike.sjlbkw.cn/Article/details/gagevpiba.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.bbcook.cn/Article/details/gxepuaiiz.sHtML

[Q18] 模糊匹配
来源：http://blog.yfazqb.com/Article/details/gtpnqxsgi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.vehdjk.com/Article/details/gsyvgtkxi.sHtML

[Q19] 范围查询
来源：http://www.share.sjlbkw.cn/Article/details/gyhiicebu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.yfazqb.com/Article/details/gnwcravvn.sHtML

[Q20] IN 列表
来源：http://www.blog.vehdjk.com/Article/details/gxlyyywzu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gupkyrzyt.sHtML

[Q21] 空值判断
来源：http://www.blog.yfazqb.com/Article/details/gyogfuphi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.vehdjk.com/Article/details/ghhijezte.sHtML

[Q22] 排序
来源：http://blog.epnwcf.com/Article/details/gdudvasxz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.bbcook.cn/Article/details/goehnxlbn.sHtML

[Q23] 分页
来源：http://m.share.yfazqb.com/Article/details/ghmjymfes.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.tarul.cn/Article/details/grvipxuxp.sHtML

[Q24] 去重
来源：http://3g.sjlbkw.cn/Article/details/gbabjahpl.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.epnwcf.com/Article/details/gwpacdjmp.sHtML

[Q25] 只取前 N 条
来源：http://m.share.epnwcf.com/Article/details/gkzhewzij.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.sjlbkw.cn/Article/details/gfaedeoes.sHtML

[Q26] 计数
来源：http://blog.yfazqb.com/Article/details/gbvkfcvzf.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gizepevla.sHtML

[Q27] 条件计数
来源：http://wap.tarul.cn/Article/details/gqzieuiyh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/ggjrkkudu.sHtML

[Q28] 求和与平均
来源：http://blog.sjlbkw.cn/Article/details/gagctagtj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gyupjrvnc.sHtML

[Q29] 最大最小值
来源：http://www.share.bbcook.cn/Article/details/gxwkmmfgg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.yfazqb.com/Article/details/gdhajhhxu.sHtML

[Q30] 分组统计
来源：http://read.share.tarul.cn/Article/details/gsukjfisn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.bbcook.cn/Article/details/gifjwaymg.sHtML

[Q31] 分组后过滤
来源：http://read.share.epnwcf.com/Article/details/gfmefotfv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.yfazqb.com/Article/details/gmivfuwbx.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.yfazqb.com/Article/details/ggrjjuisq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gbpexthka.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fktsv.cn/Article/details/gyytqpret.sHtML

[Q33] 多列分组
来源：http://blog.sjlbkw.cn/Article/details/gmspkkjzi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.epnwcf.com/Article/details/glhhpxkem.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.vehdjk.com/Article/details/gjzrajset.sHtML

SELECT * FROM (
来源：http://3g.vehdjk.com/Article/details/gminnxafz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fktsv.cn/Article/details/glebqxuiq.sHtML

) t WHERE rn = 1;
来源：http://3g.vehdjk.com/Article/details/gkvxcrltp.sHtML

[Q35] 内连接
来源：http://www.blog.sjlbkw.cn/Article/details/gfhxqolgo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.sjlbkw.cn/Article/details/girlcsybs.sHtML

[Q36] 左连接
来源：http://www.share.fktsv.cn/Article/details/gizpmxekt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fktsv.cn/Article/details/geotmwbsd.sHtML

[Q37] 右连接
来源：http://www.m.share.bbcook.cn/Article/details/gjfzrfbic.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.epnwcf.com/Article/details/guifzpqkz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.bbcook.cn/Article/details/gfagfblvj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.bbcook.cn/Article/details/gkxhdcxuo.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.sjlbkw.cn/Article/details/glkewvsdz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.epnwcf.com/Article/details/grycrbttj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.yfazqb.com/Article/details/guoidcvbi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.tarul.cn/Article/details/gtbixiqsh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.vehdjk.com/Article/details/gnzsiczui.sHtML

[Q41] 多表连接
来源：http://baike.fktsv.cn/Article/details/gsgjqrjiz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fktsv.cn/Article/details/gjwbfajas.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.bbcook.cn/Article/details/gfwkpstam.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.bbcook.cn/Article/details/gofxegqex.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.yfazqb.com/Article/details/gipkpjlsn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fktsv.cn/Article/details/gtzhqxkkh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.vehdjk.com/Article/details/geowjbeao.sHtML

[Q43] 标量子查询
来源：http://wap.fktsv.cn/Article/details/gandwaodd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fktsv.cn/Article/details/gmqzcunko.sHtML

[Q44] IN 子查询
来源：http://3g.yfazqb.com/Article/details/gzmknxbik.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.yfazqb.com/Article/details/glrhffjjo.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.vehdjk.com/Article/details/gfdsocmqx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.sjlbkw.cn/Article/details/gluslwoar.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.sjlbkw.cn/Article/details/gmupywdnn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.yfazqb.com/Article/details/gvchwcsma.sHtML

[Q47] 与平均值比较
来源：http://www.blog.bbcook.cn/Article/details/gdiychdgs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.bbcook.cn/Article/details/ggzfgfrsr.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.bbcook.cn/Article/details/gtkpzqhvg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.vehdjk.com/Article/details/gowurkdli.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.bbcook.cn/Article/details/gctsiecuw.sHtML

[Q49] 更新单行
来源：http://blog.fktsv.cn/Article/details/gkjhlytbt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.vehdjk.com/Article/details/gijpivusl.sHtML

[Q50] 批量更新
来源：http://blog.sjlbkw.cn/Article/details/gzwdpadly.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.yfazqb.com/Article/details/gmdlytruq.sHtML

[Q51] 用子查询更新
来源：http://www.blog.vehdjk.com/Article/details/gcbugxovr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fktsv.cn/Article/details/glygfujvy.sHtML

[Q52] 删除指定行
来源：http://www.share.fktsv.cn/Article/details/gtfjckkbf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.bbcook.cn/Article/details/gtrjzolln.sHtML

[Q53] 按条件删除
来源：http://wap.epnwcf.com/Article/details/gawseopor.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.epnwcf.com/Article/details/ganputvun.sHtML

[Q54] 清空表
来源：http://wap.epnwcf.com/Article/details/gtejbkriy.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fktsv.cn/Article/details/gpwzjqkks.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.bbcook.cn/Article/details/giieaqwqh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fktsv.cn/Article/details/gtiguawkl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fktsv.cn/Article/details/ggdabwkxd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.epnwcf.com/Article/details/gzuldodba.sHtML

[Q57] 行号
来源：http://www.m.share.epnwcf.com/Article/details/gfkaunhwj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/ggvzjiwcx.sHtML

[Q58] 累计求和
来源：http://wap.sjlbkw.cn/Article/details/gsoazrsbx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fktsv.cn/Article/details/gjunmvbji.sHtML

[Q59] 分组内累计
来源：http://mobile.epnwcf.com/Article/details/goxvfhjgf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gwrxfmdrs.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.vehdjk.com/Article/details/gdmyeemsh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.yfazqb.com/Article/details/gfsjxrnws.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gxmsvizkx.sHtML

[Q61] 移动平均
来源：http://3g.tarul.cn/Article/details/gpvivinaw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gtpixnzny.sHtML

[Q62] 分组占比
来源：http://read.share.tarul.cn/Article/details/gaaqklthj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/glogojuwy.sHtML

[Q63] 开启事务
来源：http://3g.tarul.cn/Article/details/gdjupaauy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fktsv.cn/Article/details/gqulwhlrf.sHtML

[Q64] 提交事务
来源：http://mobile.sjlbkw.cn/Article/details/gitaexjjt.sHtML

COMMIT;
来源：http://3g.epnwcf.com/Article/details/gnxjowqat.sHtML

[Q65] 回滚事务
来源：http://m.share.bbcook.cn/Article/details/godmbovsp.sHtML

ROLLBACK;
来源：http://www.share.vehdjk.com/Article/details/ghkywoobd.sHtML

[Q66] 行锁查询
来源：http://wap.epnwcf.com/Article/details/gcppuhcwh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.epnwcf.com/Article/details/givygasht.sHtML

[Q67] 设置隔离级别
来源：http://wap.tarul.cn/Article/details/gbclwksrm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.tarul.cn/Article/details/gwpwlvicv.sHtML

[Q68] 保存点
来源：http://blog.fktsv.cn/Article/details/ggfwjgsdz.sHtML

SAVEPOINT sp1;
来源：http://www.blog.epnwcf.com/Article/details/gdpserdhh.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fktsv.cn/Article/details/gwewqmakw.sHtML

[Q69] 查看执行计划
来源：http://baike.sjlbkw.cn/Article/details/gxcxoffqm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.sjlbkw.cn/Article/details/gqkxzqebr.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fktsv.cn/Article/details/gfguveelp.sHtML

ANALYZE TABLE users;
来源：http://read.share.epnwcf.com/Article/details/gsosybfub.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fktsv.cn/Article/details/gqcmdevii.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.yfazqb.com/Article/details/gzbvgegrw.sHtML

[Q72] 查看索引
来源：http://baike.epnwcf.com/Article/details/gdtfqtjcs.sHtML

SHOW INDEX FROM users;
来源：http://3g.vehdjk.com/Article/details/gttixaweg.sHtML

[Q73] 查看表状态
来源：http://read.share.bbcook.cn/Article/details/gyfumxyvq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fktsv.cn/Article/details/grsygzqia.sHtML

[Q74] 强制使用索引
来源：http://wap.tarul.cn/Article/details/ggbxawehn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.vehdjk.com/Article/details/gnecvacni.sHtML

[Q75] 日期格式化
来源：http://read.share.sjlbkw.cn/Article/details/grcnvaqro.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.yfazqb.com/Article/details/gnvawyddu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.tarul.cn/Article/details/gyhmmqrhn.sHtML

[Q76] 按天统计
来源：http://read.share.tarul.cn/Article/details/gwdecjedu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.vehdjk.com/Article/details/gsohkogey.sHtML

[Q77] 时间加减
来源：http://www.blog.yfazqb.com/Article/details/giliglast.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fktsv.cn/Article/details/gtjyadbzg.sHtML

[Q78] 当前时间
来源：http://mobile.bbcook.cn/Article/details/gpsylwcol.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.epnwcf.com/Article/details/gqizdurma.sHtML

[Q79] 字符串拼接
来源：http://m.share.fktsv.cn/Article/details/gvmgkispe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fktsv.cn/Article/details/gafxfkfuq.sHtML

[Q80] 字符串截取
来源：http://mobile.epnwcf.com/Article/details/gpzarvowd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gwfinvywi.sHtML

[Q81] 字符串替换
来源：http://baike.fktsv.cn/Article/details/ghjhdejxd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.bbcook.cn/Article/details/gnwsthqjt.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fktsv.cn/Article/details/glsdtuthz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gqpcijlzm.sHtML

[Q83] 大小写转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjfnidth.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gvxpqzuui.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.vehdjk.com/Article/details/gfwjggdii.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/grsvglxid.sHtML

[Q85] 数值取整
来源：http://baike.epnwcf.com/Article/details/gstryibol.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.bbcook.cn/Article/details/gcpozfpyd.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.bbcook.cn/Article/details/gzysvrjyt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.yfazqb.com/Article/details/gpdqmhqfj.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.bbcook.cn/Article/details/gpdgykabq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.vehdjk.com/Article/details/gzvksqtyb.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fktsv.cn/Article/details/gzntiaqbh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.tarul.cn/Article/details/gcouueujh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fktsv.cn/Article/details/gicowiwvg.sHtML

[Q89] 判断表是否存在
来源：http://read.share.tarul.cn/Article/details/gmutkpddc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.vehdjk.com/Article/details/gzzxnwlao.sHtML

[Q90] 生成序号列
来源：http://www.share.epnwcf.com/Article/details/ghwwkjykg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.epnwcf.com/Article/details/gkkrqdror.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/glfyzmgnd.sHtML

R. Bash 专题
来源：http://blog.sjlbkw.cn/Article/details/gxzgtbqnm.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gzkcqdele.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.tarul.cn/Article/details/gbkigsxaq.sHtML

#!/usr/bin/env bash
来源：http://blog.tarul.cn/Article/details/gvfnathzu.sHtML

set -euo pipefail
来源：http://baike.vehdjk.com/Article/details/gihpfxmko.sHtML

[R02] 变量赋值与使用
来源：http://blog.tarul.cn/Article/details/ggzpvppwh.sHtML

name="Tom"; echo "$name"
来源：http://blog.fktsv.cn/Article/details/gdnrrmajm.sHtML

[R03] 只读变量
来源：http://www.share.yfazqb.com/Article/details/gjvonbixr.sHtML

readonly PI=3.14
来源：http://www.m.share.yfazqb.com/Article/details/gxuaghwct.sHtML

[R04] 位置参数
来源：http://baike.tarul.cn/Article/details/gyjvvsqeh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.sjlbkw.cn/Article/details/gsvgzxpmp.sHtML

[R05] 参数默认值
来源：http://www.share.bbcook.cn/Article/details/giasdqwbv.sHtML

name="${1:-default}"
来源：http://read.share.fktsv.cn/Article/details/gmxjliryf.sHtML

[R06] 判断命令是否存在
来源：http://mobile.epnwcf.com/Article/details/gkvdzobrq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fktsv.cn/Article/details/gvhfxjvjs.sHtML

[R07] if 判断文件
来源：http://read.share.sjlbkw.cn/Article/details/ggukrjzwy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.epnwcf.com/Article/details/gltwhmqmx.sHtML

[R08] 数值比较
来源：http://mobile.vehdjk.com/Article/details/ggabqmipe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.bbcook.cn/Article/details/gqfdqorbw.sHtML

[R09] 字符串比较
来源：http://m.share.epnwcf.com/Article/details/gmrtidqym.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gdenrxozl.sHtML

[R10] 正则匹配
来源：http://blog.fktsv.cn/Article/details/gytfvzdji.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.epnwcf.com/Article/details/gnekdvzyi.sHtML

[R11] case 多分支
来源：http://wap.bbcook.cn/Article/details/gqhqolcwb.sHtML

case "$1" in
来源：http://www.m.share.yfazqb.com/Article/details/gqaxzasty.sHtML

start) echo "启动" ;;
来源：http://wap.bbcook.cn/Article/details/ghstkwehb.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.bbcook.cn/Article/details/gswrhjckm.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fktsv.cn/Article/details/geknilvey.sHtML

esac
来源：http://m.share.epnwcf.com/Article/details/goyjuxybb.sHtML

[R12] for 遍历文件
来源：http://read.share.tarul.cn/Article/details/gixkjjpfa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.yfazqb.com/Article/details/givjbizhi.sHtML

[R13] for 计数循环
来源：http://mobile.epnwcf.com/Article/details/gbecfyscq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/guqlchwuw.sHtML

[R14] C 风格 for
来源：http://baike.tarul.cn/Article/details/gkjfaouzb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.bbcook.cn/Article/details/gzulcvcnl.sHtML

[R15] while 逐行读文件
来源：http://3g.fktsv.cn/Article/details/gufhojqiw.sHtML


<!-- 参考信息 -->