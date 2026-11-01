代发 wailian999

C#:   Parallel.For
来源：http://www.blog.yfazqb.com/Article/details/gazjcmdgr.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gzougusra.sHtML

P. 常用工具函数
来源：http://baike.tarul.cn/Article/details/guvlvgmmv.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gfyeycdwp.sHtML

[P01] 生成 UUID
来源：http://www.m.share.vehdjk.com/Article/details/ghychaacx.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.epnwcf.com/Article/details/gkkqdnxjv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fktsv.cn/Article/details/gpshmmxap.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/gtyvtywzf.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gwddybctn.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.yfazqb.com/Article/details/gvvkmpjlk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.tarul.cn/Article/details/gidutbjzh.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.yfazqb.com/Article/details/gzszcwlzb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fktsv.cn/Article/details/gqeliviko.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.vehdjk.com/Article/details/gagauambh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fktsv.cn/Article/details/gfmrzvhdh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.vehdjk.com/Article/details/gxwaohdzt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.bbcook.cn/Article/details/gohhhpfmn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.epnwcf.com/Article/details/gwzzavlai.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.vehdjk.com/Article/details/gwkcffcfi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.epnwcf.com/Article/details/gksvwtqsi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.yfazqb.com/Article/details/ggldfwjpz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.tarul.cn/Article/details/grdghidpw.sHtML

[P03] 生成短随机字符串
来源：http://blog.bbcook.cn/Article/details/gyvtyqomq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.yfazqb.com/Article/details/gbpzzanxl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.yfazqb.com/Article/details/ggounajnp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.sjlbkw.cn/Article/details/gbgmjdgxa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/guqvophyo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fktsv.cn/Article/details/gjgpbgnhd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.bbcook.cn/Article/details/gwsoehqel.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.vehdjk.com/Article/details/grmcpegxe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.sjlbkw.cn/Article/details/ghqbsktpa.sHtML

[P04] 求长度
来源：http://3g.vehdjk.com/Article/details/gnkaloaus.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.tarul.cn/Article/details/gtolcczjr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gsqnvttaw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gnudedckf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.vehdjk.com/Article/details/gxdhyfbtp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.tarul.cn/Article/details/gfsjjcumg.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.yfazqb.com/Article/details/gugbnwoiy.sHtML

Ruby: x.length;  x.size
来源：http://wap.bbcook.cn/Article/details/gwstxcogg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.tarul.cn/Article/details/gncuufjdw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.vehdjk.com/Article/details/gdngxjjdp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.tarul.cn/Article/details/glisydfvp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.sjlbkw.cn/Article/details/gsiobuzgq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.sjlbkw.cn/Article/details/gludfwxyb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.vehdjk.com/Article/details/gtprrrafp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fktsv.cn/Article/details/gjqjavltv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.sjlbkw.cn/Article/details/grfannwky.sHtML

Ruby: a == b
来源：http://blog.epnwcf.com/Article/details/gbukkvpew.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.sjlbkw.cn/Article/details/grizivdsy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.yfazqb.com/Article/details/gacwsuled.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.tarul.cn/Article/details/ginovrcfq.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.sjlbkw.cn/Article/details/gzdbteadq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.vehdjk.com/Article/details/gkxhkyvxi.sHtML

TS:   if (x == null) {}
来源：http://mobile.yfazqb.com/Article/details/geyymorwo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/gemujirft.sHtML

Go:   if x == nil {}
来源：http://read.share.bbcook.cn/Article/details/grwzbppex.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fktsv.cn/Article/details/gudzrvgyt.sHtML

C#:   if (x is null) {}
来源：http://wap.sjlbkw.cn/Article/details/gfgguthym.sHtML

[P07] 防抖与节流
来源：http://3g.sjlbkw.cn/Article/details/gxdjmtkfq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.bbcook.cn/Article/details/gsbffcoch.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.sjlbkw.cn/Article/details/gqrmgedxs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gordizyot.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gcanbzhzj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.yfazqb.com/Article/details/gtzjtjvhc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.vehdjk.com/Article/details/geczelvcp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.epnwcf.com/Article/details/gvuicqldg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.yfazqb.com/Article/details/gsuslpuyj.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.yfazqb.com/Article/details/gadjumpbh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.sjlbkw.cn/Article/details/gcryxnywm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.epnwcf.com/Article/details/gzelmhoci.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fktsv.cn/Article/details/gbhyjddmo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.bbcook.cn/Article/details/ggrwkovzd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.sjlbkw.cn/Article/details/gapsnfvtm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.yfazqb.com/Article/details/gjumrvahv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.vehdjk.com/Article/details/grujznmum.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.vehdjk.com/Article/details/gdxjmoxme.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gxpxzettc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.epnwcf.com/Article/details/gcjwlisrr.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gzwaiifve.sHtML

[Q01] 创建表
来源：http://read.share.epnwcf.com/Article/details/gdtgpzdkj.sHtML

CREATE TABLE users (
来源：http://blog.bbcook.cn/Article/details/gjqiayfdx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gkiuzygvz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/gbxfzrwja.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fktsv.cn/Article/details/gynkmeafn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.yfazqb.com/Article/details/gucnhzkyg.sHtML

);
来源：http://wap.yfazqb.com/Article/details/guiearbvd.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.epnwcf.com/Article/details/ganlzzdlm.sHtML

CREATE TABLE orders (
来源：http://3g.yfazqb.com/Article/details/gbkksrflc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fktsv.cn/Article/details/gqcnhvxzo.sHtML

user_id INT NOT NULL,
来源：http://www.share.fktsv.cn/Article/details/gqbwmziqo.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.sjlbkw.cn/Article/details/gfydwkwyu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.vehdjk.com/Article/details/gopaspccw.sHtML

);
来源：http://www.blog.bbcook.cn/Article/details/gtpmgznwq.sHtML

[Q03] 增加列
来源：http://m.share.tarul.cn/Article/details/gwegimnor.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.yfazqb.com/Article/details/gikahtfux.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fktsv.cn/Article/details/gpwrbwuww.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmesanohh.sHtML

[Q05] 重命名列
来源：http://read.share.epnwcf.com/Article/details/gpnokwfwz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.vehdjk.com/Article/details/gzwmseupm.sHtML

[Q06] 删除列
来源：http://www.m.share.sjlbkw.cn/Article/details/godtmimpm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.bbcook.cn/Article/details/gileleukj.sHtML

[Q07] 删除表
来源：http://mobile.bbcook.cn/Article/details/gjgoyslwc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.vehdjk.com/Article/details/ggummqcqt.sHtML

[Q08] 创建普通索引
来源：http://mobile.sjlbkw.cn/Article/details/gcaafthca.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.epnwcf.com/Article/details/gsosnsxea.sHtML

[Q09] 创建唯一索引
来源：http://3g.sjlbkw.cn/Article/details/gvinwncud.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.tarul.cn/Article/details/gjxftuuos.sHtML

[Q10] 插入单行
来源：http://m.share.tarul.cn/Article/details/gglybiahf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.bbcook.cn/Article/details/gmaouxwuk.sHtML

[Q11] 一次插入多行
来源：http://www.blog.yfazqb.com/Article/details/glxwjlgbo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.vehdjk.com/Article/details/gpkqzncls.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.sjlbkw.cn/Article/details/gwweznffo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.yfazqb.com/Article/details/gehyvtsze.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.epnwcf.com/Article/details/gmkmwferu.sHtML

[Q13] 忽略重复插入
来源：http://wap.tarul.cn/Article/details/gyrxtgalz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.tarul.cn/Article/details/gvajbmxdq.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.yfazqb.com/Article/details/gzpvshnba.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.yfazqb.com/Article/details/gpghxkoed.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.sjlbkw.cn/Article/details/grunddqse.sHtML

[Q15] 查询全部
来源：http://mobile.fktsv.cn/Article/details/ghcvadetz.sHtML

SELECT * FROM users;
来源：http://wap.bbcook.cn/Article/details/guqcpjcxd.sHtML

[Q16] 查询指定列
来源：http://www.share.yfazqb.com/Article/details/gmrunlwky.sHtML

SELECT id, name FROM users;
来源：http://baike.bbcook.cn/Article/details/gjmbgjvic.sHtML

[Q17] 条件查询
来源：http://read.share.sjlbkw.cn/Article/details/gtzgejndt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gbersgrqn.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwmxprmn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fktsv.cn/Article/details/glgycrlks.sHtML

[Q19] 范围查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzxrpvla.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.bbcook.cn/Article/details/gqclacpar.sHtML

[Q20] IN 列表
来源：http://3g.vehdjk.com/Article/details/gcnxslhob.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.vehdjk.com/Article/details/gybffxhwf.sHtML

[Q21] 空值判断
来源：http://www.blog.sjlbkw.cn/Article/details/gcrcfzlae.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.vehdjk.com/Article/details/gewfmboqk.sHtML

[Q22] 排序
来源：http://3g.fktsv.cn/Article/details/gwjhkkfuk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.tarul.cn/Article/details/gxsspazkj.sHtML

[Q23] 分页
来源：http://mobile.bbcook.cn/Article/details/gfiuwylzj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.vehdjk.com/Article/details/gsteaimit.sHtML

[Q24] 去重
来源：http://www.share.bbcook.cn/Article/details/gucnfcmpl.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fktsv.cn/Article/details/guizwrjfg.sHtML

[Q25] 只取前 N 条
来源：http://3g.sjlbkw.cn/Article/details/gzzekoszy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.vehdjk.com/Article/details/gfwmppvlj.sHtML

[Q26] 计数
来源：http://baike.tarul.cn/Article/details/gvbvmhiyv.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.bbcook.cn/Article/details/grbztuvbh.sHtML

[Q27] 条件计数
来源：http://mobile.fktsv.cn/Article/details/giqnvzoxf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.epnwcf.com/Article/details/gxmhclvyh.sHtML

[Q28] 求和与平均
来源：http://blog.yfazqb.com/Article/details/gxlfkdcxo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gzrpwzxyq.sHtML

[Q29] 最大最小值
来源：http://wap.vehdjk.com/Article/details/ggdrkiqzq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gmixghzms.sHtML

[Q30] 分组统计
来源：http://www.m.share.fktsv.cn/Article/details/gcdgxpmta.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/grjijxgsh.sHtML

[Q31] 分组后过滤
来源：http://www.share.vehdjk.com/Article/details/gmjewglwl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.bbcook.cn/Article/details/gtdmbcagx.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.tarul.cn/Article/details/gripapzvc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gksskgszv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fktsv.cn/Article/details/gjkpkbscz.sHtML

[Q33] 多列分组
来源：http://mobile.yfazqb.com/Article/details/gzkoxborp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.vehdjk.com/Article/details/gilvfflvl.sHtML

[Q34] 每组取第一条
来源：http://baike.epnwcf.com/Article/details/gmdrbrmnu.sHtML

SELECT * FROM (
来源：http://www.m.share.tarul.cn/Article/details/gsppyhwid.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.bbcook.cn/Article/details/gcuwkdmaq.sHtML

) t WHERE rn = 1;
来源：http://read.share.epnwcf.com/Article/details/gejpjgcyj.sHtML

[Q35] 内连接
来源：http://baike.yfazqb.com/Article/details/gaqnrmbvt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.tarul.cn/Article/details/gygwxtoxw.sHtML

[Q36] 左连接
来源：http://3g.bbcook.cn/Article/details/gzxdighjz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.sjlbkw.cn/Article/details/gctazckzo.sHtML

[Q37] 右连接
来源：http://baike.fktsv.cn/Article/details/gqdkbrysz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.epnwcf.com/Article/details/ghcososrr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.yfazqb.com/Article/details/gznlhwpve.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.tarul.cn/Article/details/gbyeidhnv.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.vehdjk.com/Article/details/gqkxbhoxb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.yfazqb.com/Article/details/gznptmeve.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.epnwcf.com/Article/details/gvchdzezp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.bbcook.cn/Article/details/glhjmnbjt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.epnwcf.com/Article/details/gftmpqdjj.sHtML

[Q41] 多表连接
来源：http://blog.vehdjk.com/Article/details/gfyssyrxl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.vehdjk.com/Article/details/gbhxorqgx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.bbcook.cn/Article/details/gcdiaifbh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.sjlbkw.cn/Article/details/gapfvcacs.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.tarul.cn/Article/details/gojjrxgoc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.yfazqb.com/Article/details/graowrpmr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.sjlbkw.cn/Article/details/govvzazoq.sHtML

[Q43] 标量子查询
来源：http://mobile.yfazqb.com/Article/details/gxhzgsefm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.vehdjk.com/Article/details/gtngprvth.sHtML

[Q44] IN 子查询
来源：http://wap.yfazqb.com/Article/details/gtvvackrb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.epnwcf.com/Article/details/gbqwufpzf.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.yfazqb.com/Article/details/gsbmfvrly.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.sjlbkw.cn/Article/details/ggjxpduff.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.epnwcf.com/Article/details/gjvvxnthp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.bbcook.cn/Article/details/gvlsuhmqb.sHtML

[Q47] 与平均值比较
来源：http://read.share.sjlbkw.cn/Article/details/gnacllmyf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.tarul.cn/Article/details/glrvegpte.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fktsv.cn/Article/details/ghbnnteko.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.tarul.cn/Article/details/gfpreghfi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.bbcook.cn/Article/details/gbwwoxdcu.sHtML

[Q49] 更新单行
来源：http://www.m.share.epnwcf.com/Article/details/gdegmkuqc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.yfazqb.com/Article/details/ghwpiijzl.sHtML

[Q50] 批量更新
来源：http://blog.yfazqb.com/Article/details/ghfnxpvdm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.sjlbkw.cn/Article/details/gerajrpqk.sHtML

[Q51] 用子查询更新
来源：http://m.share.fktsv.cn/Article/details/gncztmujj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.tarul.cn/Article/details/gjqnicfma.sHtML

[Q52] 删除指定行
来源：http://wap.sjlbkw.cn/Article/details/gjqtvtilx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fktsv.cn/Article/details/gvwltlozt.sHtML

[Q53] 按条件删除
来源：http://wap.bbcook.cn/Article/details/gyfywkeze.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gnhbtcpip.sHtML

[Q54] 清空表
来源：http://baike.bbcook.cn/Article/details/gpfbhyqkg.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.sjlbkw.cn/Article/details/gytchveoe.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.epnwcf.com/Article/details/gaaerzett.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.yfazqb.com/Article/details/gmswexeuo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.tarul.cn/Article/details/gwequthhi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.bbcook.cn/Article/details/gpfifegoq.sHtML

[Q57] 行号
来源：http://www.blog.sjlbkw.cn/Article/details/gqiuwvolo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.bbcook.cn/Article/details/gbrerpgwf.sHtML

[Q58] 累计求和
来源：http://blog.epnwcf.com/Article/details/gpkunskgt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.tarul.cn/Article/details/gtqbytcfn.sHtML

[Q59] 分组内累计
来源：http://m.share.epnwcf.com/Article/details/gabsvlkqq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gxhainuac.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fktsv.cn/Article/details/gquggydmz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.vehdjk.com/Article/details/gldnnvysx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/ghboxzsob.sHtML

[Q61] 移动平均
来源：http://www.m.share.epnwcf.com/Article/details/gdqednyio.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.vehdjk.com/Article/details/gnobbzlge.sHtML

[Q62] 分组占比
来源：http://baike.bbcook.cn/Article/details/gmncdavzd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/ggtmqgqhx.sHtML

[Q63] 开启事务
来源：http://www.share.tarul.cn/Article/details/gsjifzkdu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.epnwcf.com/Article/details/gfkxvpwtr.sHtML

[Q64] 提交事务
来源：http://read.share.tarul.cn/Article/details/gkmkhmwfw.sHtML

COMMIT;
来源：http://m.share.vehdjk.com/Article/details/goeplvzcx.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fktsv.cn/Article/details/gapughvvi.sHtML

ROLLBACK;
来源：http://read.share.bbcook.cn/Article/details/gtytrtllv.sHtML

[Q66] 行锁查询
来源：http://www.share.epnwcf.com/Article/details/gnbtpmgkr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.yfazqb.com/Article/details/gaoanirfn.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.tarul.cn/Article/details/gowtifkpn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.yfazqb.com/Article/details/gqdhkcaxm.sHtML

[Q68] 保存点
来源：http://3g.tarul.cn/Article/details/gfrlbolmp.sHtML

SAVEPOINT sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/gtttahvtj.sHtML

ROLLBACK TO sp1;
来源：http://baike.vehdjk.com/Article/details/gnxfvbwus.sHtML

[Q69] 查看执行计划
来源：http://wap.tarul.cn/Article/details/gucujlatt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.epnwcf.com/Article/details/gobcpjrua.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjdqiuum.sHtML

ANALYZE TABLE users;
来源：http://baike.yfazqb.com/Article/details/gzcbbhlvx.sHtML

[Q71] 查看建表语句
来源：http://mobile.fktsv.cn/Article/details/giaywpkek.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.vehdjk.com/Article/details/gladycnkv.sHtML

[Q72] 查看索引
来源：http://wap.fktsv.cn/Article/details/gommudpwr.sHtML

SHOW INDEX FROM users;
来源：http://wap.bbcook.cn/Article/details/gqkflobyi.sHtML

[Q73] 查看表状态
来源：http://baike.sjlbkw.cn/Article/details/gdbqmzvro.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.bbcook.cn/Article/details/gzpceeqjs.sHtML

[Q74] 强制使用索引
来源：http://wap.vehdjk.com/Article/details/gycpsrciw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.tarul.cn/Article/details/gjhpzvtip.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/gwzfjiqlg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzldbwbm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.epnwcf.com/Article/details/gsgknmhuf.sHtML

[Q76] 按天统计
来源：http://wap.vehdjk.com/Article/details/geetmggec.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.tarul.cn/Article/details/gbxbvwyis.sHtML

[Q77] 时间加减
来源：http://www.blog.tarul.cn/Article/details/gxxihcktq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.epnwcf.com/Article/details/guzxgqhlj.sHtML

[Q78] 当前时间
来源：http://wap.sjlbkw.cn/Article/details/gquqirfnz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.tarul.cn/Article/details/gudbthxfp.sHtML

[Q79] 字符串拼接
来源：http://3g.tarul.cn/Article/details/gpkbxvbet.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.bbcook.cn/Article/details/gcimmrjng.sHtML

[Q80] 字符串截取
来源：http://m.share.tarul.cn/Article/details/gydfsqffe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.vehdjk.com/Article/details/gjtoltjhe.sHtML

[Q81] 字符串替换
来源：http://3g.sjlbkw.cn/Article/details/gxdvsysqr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.bbcook.cn/Article/details/gwtrxrtst.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.vehdjk.com/Article/details/gzgxpftid.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gndcjnzyv.sHtML

[Q83] 大小写转换
来源：http://baike.vehdjk.com/Article/details/gjvtadikt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gyamftxap.sHtML

[Q84] 去除首尾空格
来源：http://3g.sjlbkw.cn/Article/details/gutqguahs.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gqrevsjvp.sHtML

[Q85] 数值取整
来源：http://3g.vehdjk.com/Article/details/gvrnjklfc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.sjlbkw.cn/Article/details/gsouwtsza.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.epnwcf.com/Article/details/gkjkffxou.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.bbcook.cn/Article/details/gxsvytgoo.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.epnwcf.com/Article/details/gswsvhpsz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.epnwcf.com/Article/details/gjkhcfptw.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.yfazqb.com/Article/details/gaaegpnde.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fktsv.cn/Article/details/guxotdqcn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gxulxxpwq.sHtML

[Q89] 判断表是否存在
来源：http://3g.vehdjk.com/Article/details/gwerbolnd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fktsv.cn/Article/details/gyvrqnwyo.sHtML

[Q90] 生成序号列
来源：http://baike.yfazqb.com/Article/details/gltbbeshx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fktsv.cn/Article/details/gdaszrsyq.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gmjxgcsmc.sHtML

R. Bash 专题
来源：http://blog.fktsv.cn/Article/details/glhiyezkv.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gccysugdf.sHtML

[R01] shebang 与严格模式
来源：http://mobile.epnwcf.com/Article/details/gufzkkycu.sHtML

#!/usr/bin/env bash
来源：http://baike.bbcook.cn/Article/details/gbkvsaxyt.sHtML

set -euo pipefail
来源：http://mobile.epnwcf.com/Article/details/gyeaarmjv.sHtML

[R02] 变量赋值与使用
来源：http://blog.fktsv.cn/Article/details/gihkzisbb.sHtML

name="Tom"; echo "$name"
来源：http://blog.tarul.cn/Article/details/gwdgtzwcs.sHtML

[R03] 只读变量
来源：http://3g.vehdjk.com/Article/details/gazoywbla.sHtML

readonly PI=3.14
来源：http://3g.epnwcf.com/Article/details/gtrlkkhit.sHtML

[R04] 位置参数
来源：http://www.m.share.yfazqb.com/Article/details/gujtalixh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.yfazqb.com/Article/details/gaejhhqgz.sHtML

[R05] 参数默认值
来源：http://wap.vehdjk.com/Article/details/gicflcpye.sHtML

name="${1:-default}"
来源：http://www.blog.tarul.cn/Article/details/gcoakhllh.sHtML

[R06] 判断命令是否存在
来源：http://blog.yfazqb.com/Article/details/gxnqorpnd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fktsv.cn/Article/details/gqdwndouw.sHtML

[R07] if 判断文件
来源：http://read.share.tarul.cn/Article/details/gmdkmdzrn.sHtML


<!-- 参考信息 -->