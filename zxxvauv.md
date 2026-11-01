代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/gnzcxmayq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.epnwcf.com/Article/details/gdjgedink.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.epnwcf.com/Article/details/govblfren.sHtML

Ruby: // fork 块
来源：http://baike.fktsv.cn/Article/details/ghzyydxeo.sHtML

C#:   Parallel.For
来源：http://www.share.sjlbkw.cn/Article/details/gvhoobwxh.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gjigckdky.sHtML

P. 常用工具函数
来源：http://read.share.vehdjk.com/Article/details/gekaxqtei.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/garqckgxq.sHtML

[P01] 生成 UUID
来源：http://3g.bbcook.cn/Article/details/gefipzvve.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.vehdjk.com/Article/details/ggymtknme.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.tarul.cn/Article/details/gwhnotidq.sHtML

JS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gkalegniu.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gsnhaerqb.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.vehdjk.com/Article/details/gjxarphvd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.vehdjk.com/Article/details/ggmffprvd.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.epnwcf.com/Article/details/gbzoqyevu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.bbcook.cn/Article/details/gwrcfbykr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.bbcook.cn/Article/details/gqoarzmkk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.tarul.cn/Article/details/gluaguqzi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.bbcook.cn/Article/details/gkiiujret.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fktsv.cn/Article/details/gsjsotqem.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.sjlbkw.cn/Article/details/gfgkvjdlk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.bbcook.cn/Article/details/gclmedfyj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.bbcook.cn/Article/details/gpkoskzrt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.bbcook.cn/Article/details/gdfwkkgan.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.vehdjk.com/Article/details/gcepzvcxo.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.vehdjk.com/Article/details/gmmuyxvsy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.epnwcf.com/Article/details/gejxteish.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.epnwcf.com/Article/details/grtqhlbop.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.vehdjk.com/Article/details/gaihjfbvj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/gtnpbxjrs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fktsv.cn/Article/details/gnvbbpykm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.bbcook.cn/Article/details/gscitsajj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.vehdjk.com/Article/details/gfsotjjjy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.epnwcf.com/Article/details/gecdzsbeo.sHtML

[P04] 求长度
来源：http://www.blog.tarul.cn/Article/details/gknbwavvl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.sjlbkw.cn/Article/details/ghfqkyzyh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gpkaepkkz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/gzgsajalt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fktsv.cn/Article/details/gsjsxwojt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fktsv.cn/Article/details/gpbhmnrbh.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.yfazqb.com/Article/details/gtpcirnrr.sHtML

Ruby: x.length;  x.size
来源：http://mobile.sjlbkw.cn/Article/details/gptfqpoci.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.vehdjk.com/Article/details/gduecvmkf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.bbcook.cn/Article/details/godohwulr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.vehdjk.com/Article/details/gkbukxewv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.tarul.cn/Article/details/gezikrzsw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.epnwcf.com/Article/details/gddhgksov.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/gktbnijhh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.vehdjk.com/Article/details/gjdjuljpo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/ghxwqyrgi.sHtML

Ruby: a == b
来源：http://www.blog.fktsv.cn/Article/details/gumsvlvoi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.vehdjk.com/Article/details/ggjehzoec.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.epnwcf.com/Article/details/gtebraguu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fktsv.cn/Article/details/gsgpswopv.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fktsv.cn/Article/details/gunakojxt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.yfazqb.com/Article/details/gyutlcdwl.sHtML

TS:   if (x == null) {}
来源：http://read.share.vehdjk.com/Article/details/gkptmyahe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.yfazqb.com/Article/details/gybvyvxdm.sHtML

Go:   if x == nil {}
来源：http://www.blog.bbcook.cn/Article/details/gcviipbcf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.tarul.cn/Article/details/goufkhyfz.sHtML

C#:   if (x is null) {}
来源：http://wap.vehdjk.com/Article/details/gzbmvcpzl.sHtML

[P07] 防抖与节流
来源：http://wap.sjlbkw.cn/Article/details/gcxjsvirl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.sjlbkw.cn/Article/details/gbkfdtxll.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.vehdjk.com/Article/details/gytyvybtg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gfaiftblc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.bbcook.cn/Article/details/grqiacnkj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.vehdjk.com/Article/details/gqkojsmbo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.yfazqb.com/Article/details/gwegxjkhx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.yfazqb.com/Article/details/gjgeaywqz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.sjlbkw.cn/Article/details/gnqhccapn.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.yfazqb.com/Article/details/gjhkkqycw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fktsv.cn/Article/details/gitnssbfl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.sjlbkw.cn/Article/details/gtsczwnyw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fktsv.cn/Article/details/gzjdkynbd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fktsv.cn/Article/details/glyvjucht.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.sjlbkw.cn/Article/details/gdehevasa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.tarul.cn/Article/details/gixpikcdh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.sjlbkw.cn/Article/details/gignlvsux.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.epnwcf.com/Article/details/gefbppqtk.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjgfahvsc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.tarul.cn/Article/details/gdhyevugc.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/guailypnj.sHtML

[Q01] 创建表
来源：http://www.share.sjlbkw.cn/Article/details/ghbllfnvy.sHtML

CREATE TABLE users (
来源：http://wap.epnwcf.com/Article/details/gaashxjpd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.tarul.cn/Article/details/gfmqnlwnh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.bbcook.cn/Article/details/gobmzlcwh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.vehdjk.com/Article/details/gptgmabtj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.tarul.cn/Article/details/gvstfbdaz.sHtML

);
来源：http://m.share.epnwcf.com/Article/details/gxxiecfwk.sHtML

[Q02] 创建带外键的表
来源：http://wap.fktsv.cn/Article/details/gcmdnynjs.sHtML

CREATE TABLE orders (
来源：http://read.share.sjlbkw.cn/Article/details/gvwzbmcyd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.sjlbkw.cn/Article/details/gsophrqvb.sHtML

user_id INT NOT NULL,
来源：http://www.share.sjlbkw.cn/Article/details/gcdnatznv.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.tarul.cn/Article/details/gzvxuurph.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.tarul.cn/Article/details/geeoinpra.sHtML

);
来源：http://www.share.vehdjk.com/Article/details/gehoonnnq.sHtML

[Q03] 增加列
来源：http://baike.tarul.cn/Article/details/ghrzndqir.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.bbcook.cn/Article/details/gbmednshb.sHtML

[Q04] 修改列类型
来源：http://read.share.yfazqb.com/Article/details/gbhvxticc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.tarul.cn/Article/details/gydewejyj.sHtML

[Q05] 重命名列
来源：http://www.blog.yfazqb.com/Article/details/gmqpgwelz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.yfazqb.com/Article/details/grobnzdbi.sHtML

[Q06] 删除列
来源：http://blog.vehdjk.com/Article/details/gekxcggda.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.sjlbkw.cn/Article/details/ggdwengqy.sHtML

[Q07] 删除表
来源：http://mobile.sjlbkw.cn/Article/details/gswhaofzk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.vehdjk.com/Article/details/gvkkcqqhv.sHtML

[Q08] 创建普通索引
来源：http://m.share.yfazqb.com/Article/details/gbtiqjmpc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/gqaaxdcjy.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fktsv.cn/Article/details/gyiltewbo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/grswubmlj.sHtML

[Q10] 插入单行
来源：http://m.share.sjlbkw.cn/Article/details/gkdvajbbb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.tarul.cn/Article/details/gkeqwnetc.sHtML

[Q11] 一次插入多行
来源：http://wap.tarul.cn/Article/details/ghzzfxwtd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.vehdjk.com/Article/details/gprpqhnvu.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.yfazqb.com/Article/details/gjfcwummu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.vehdjk.com/Article/details/glbtqjgxh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.epnwcf.com/Article/details/gceariipp.sHtML

[Q13] 忽略重复插入
来源：http://blog.bbcook.cn/Article/details/gwbhiceid.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.tarul.cn/Article/details/gmxzokepw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.epnwcf.com/Article/details/gvogrdbwn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.epnwcf.com/Article/details/gapmnbicg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fktsv.cn/Article/details/gzufousgn.sHtML

[Q15] 查询全部
来源：http://read.share.fktsv.cn/Article/details/gygykcbjv.sHtML

SELECT * FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnczzxkb.sHtML

[Q16] 查询指定列
来源：http://read.share.sjlbkw.cn/Article/details/grjulyuhh.sHtML

SELECT id, name FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gjznyuxje.sHtML

[Q17] 条件查询
来源：http://baike.vehdjk.com/Article/details/gxcsggcbt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.bbcook.cn/Article/details/ghilawisf.sHtML

[Q18] 模糊匹配
来源：http://www.share.epnwcf.com/Article/details/gmcvhsvxb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.vehdjk.com/Article/details/gohbyrsud.sHtML

[Q19] 范围查询
来源：http://read.share.fktsv.cn/Article/details/gdmlagpka.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fktsv.cn/Article/details/glfnpgvrm.sHtML

[Q20] IN 列表
来源：http://3g.bbcook.cn/Article/details/gbgjqjkox.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.tarul.cn/Article/details/glhsoktvh.sHtML

[Q21] 空值判断
来源：http://www.blog.bbcook.cn/Article/details/gxmehrmqq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fktsv.cn/Article/details/gzghfdthv.sHtML

[Q22] 排序
来源：http://www.share.fktsv.cn/Article/details/glgdxctvh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.bbcook.cn/Article/details/ghknnptbg.sHtML

[Q23] 分页
来源：http://3g.bbcook.cn/Article/details/gvwvrscvc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fktsv.cn/Article/details/gmxkuyxrj.sHtML

[Q24] 去重
来源：http://read.share.fktsv.cn/Article/details/gsvisvynr.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.epnwcf.com/Article/details/ggjrjhory.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fktsv.cn/Article/details/gtfoflrpy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.bbcook.cn/Article/details/gzyfunqpi.sHtML

[Q26] 计数
来源：http://m.share.bbcook.cn/Article/details/gyakpkgyx.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.tarul.cn/Article/details/gxwhxrxlr.sHtML

[Q27] 条件计数
来源：http://wap.bbcook.cn/Article/details/gtkcykfyc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.yfazqb.com/Article/details/gpthypswl.sHtML

[Q28] 求和与平均
来源：http://read.share.tarul.cn/Article/details/gxxvpezlw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.epnwcf.com/Article/details/gttoyopmk.sHtML

[Q29] 最大最小值
来源：http://www.blog.yfazqb.com/Article/details/ghygdhbaw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gkdlqzdww.sHtML

[Q30] 分组统计
来源：http://read.share.yfazqb.com/Article/details/gmcdjxwyu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/gmzlomfxh.sHtML

[Q31] 分组后过滤
来源：http://read.share.vehdjk.com/Article/details/gtdywwfah.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fktsv.cn/Article/details/grfclramy.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.bbcook.cn/Article/details/geytlxlhy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/glmrddjnl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.sjlbkw.cn/Article/details/gdfghnayo.sHtML

[Q33] 多列分组
来源：http://read.share.bbcook.cn/Article/details/gyakvupps.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.bbcook.cn/Article/details/ggmkfaifs.sHtML

[Q34] 每组取第一条
来源：http://read.share.bbcook.cn/Article/details/ghvgrhewu.sHtML

SELECT * FROM (
来源：http://baike.tarul.cn/Article/details/gzrfxusij.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.tarul.cn/Article/details/gzsqzraen.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.vehdjk.com/Article/details/guytkzzpb.sHtML

[Q35] 内连接
来源：http://baike.tarul.cn/Article/details/gefnduyct.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.vehdjk.com/Article/details/gazszdhex.sHtML

[Q36] 左连接
来源：http://www.m.share.fktsv.cn/Article/details/gmugmfsty.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.bbcook.cn/Article/details/gfwoiokdm.sHtML

[Q37] 右连接
来源：http://www.blog.vehdjk.com/Article/details/gfffuoxef.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.epnwcf.com/Article/details/gjgdcubgi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fktsv.cn/Article/details/gmbvrmvnl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.sjlbkw.cn/Article/details/gtzvajmdd.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.sjlbkw.cn/Article/details/gbckzcuuv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.tarul.cn/Article/details/gbowzazlm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.bbcook.cn/Article/details/gzrreumcw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.vehdjk.com/Article/details/gbqpuzcqg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.bbcook.cn/Article/details/gfigjlezv.sHtML

[Q41] 多表连接
来源：http://wap.vehdjk.com/Article/details/ginduhyvk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fktsv.cn/Article/details/gwahigjlt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.epnwcf.com/Article/details/gqoevbkfg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fktsv.cn/Article/details/gtjhqzwtk.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.yfazqb.com/Article/details/gkkeiytni.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.epnwcf.com/Article/details/gqsqgkvnf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.sjlbkw.cn/Article/details/gwzpykemj.sHtML

[Q43] 标量子查询
来源：http://blog.epnwcf.com/Article/details/grypyxhjh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.vehdjk.com/Article/details/gvljntoxx.sHtML

[Q44] IN 子查询
来源：http://www.m.share.bbcook.cn/Article/details/ghtfdaqcp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.tarul.cn/Article/details/gtdarazyz.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fktsv.cn/Article/details/gemqffocp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.vehdjk.com/Article/details/grksfnqaz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.sjlbkw.cn/Article/details/gxcxvxuan.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.yfazqb.com/Article/details/gwfmxeghq.sHtML

[Q47] 与平均值比较
来源：http://baike.vehdjk.com/Article/details/gxmkccfjj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fktsv.cn/Article/details/gvnpugchx.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.tarul.cn/Article/details/gkxltrruz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.bbcook.cn/Article/details/gviljvnxh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.epnwcf.com/Article/details/gvgwckvqm.sHtML

[Q49] 更新单行
来源：http://www.blog.sjlbkw.cn/Article/details/gwaahmida.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.epnwcf.com/Article/details/ggmbtuytx.sHtML

[Q50] 批量更新
来源：http://mobile.epnwcf.com/Article/details/gjarbctas.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.yfazqb.com/Article/details/ggzhmnhfb.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fktsv.cn/Article/details/gxotvexhe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.yfazqb.com/Article/details/gtxaoefrd.sHtML

[Q52] 删除指定行
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfkfwkfm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.vehdjk.com/Article/details/gmyeyfcdv.sHtML

[Q53] 按条件删除
来源：http://baike.fktsv.cn/Article/details/goaeilfes.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.epnwcf.com/Article/details/ghyeywipe.sHtML

[Q54] 清空表
来源：http://3g.yfazqb.com/Article/details/gxoxhsrba.sHtML

TRUNCATE TABLE logs;
来源：http://blog.sjlbkw.cn/Article/details/gpcworpba.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.yfazqb.com/Article/details/gbxiqcvkf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.epnwcf.com/Article/details/gtlykxyaq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fktsv.cn/Article/details/gxukhrvep.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.sjlbkw.cn/Article/details/gjfylgewt.sHtML

[Q57] 行号
来源：http://baike.sjlbkw.cn/Article/details/gajywnjgm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gzsjejbhc.sHtML

[Q58] 累计求和
来源：http://m.share.yfazqb.com/Article/details/gvgvoymuz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gqligakzc.sHtML

[Q59] 分组内累计
来源：http://read.share.fktsv.cn/Article/details/gmkiepohd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/ggghecouk.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fktsv.cn/Article/details/gvwprcghz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.vehdjk.com/Article/details/gaeoslrhy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.yfazqb.com/Article/details/gobztiqzk.sHtML

[Q61] 移动平均
来源：http://wap.fktsv.cn/Article/details/gottupkpm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gsmenuwll.sHtML

[Q62] 分组占比
来源：http://3g.epnwcf.com/Article/details/gqkozcnci.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/gsrofclgx.sHtML

[Q63] 开启事务
来源：http://www.m.share.yfazqb.com/Article/details/gwijfbgbs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.yfazqb.com/Article/details/gkgeheedl.sHtML

[Q64] 提交事务
来源：http://3g.epnwcf.com/Article/details/gpqtdbohu.sHtML

COMMIT;
来源：http://3g.sjlbkw.cn/Article/details/gyqckyzni.sHtML

[Q65] 回滚事务
来源：http://www.m.share.sjlbkw.cn/Article/details/giwjcvigh.sHtML

ROLLBACK;
来源：http://www.share.tarul.cn/Article/details/gbnlnhnjv.sHtML

[Q66] 行锁查询
来源：http://www.share.tarul.cn/Article/details/gtsyhfukk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.epnwcf.com/Article/details/gyhwbcnbs.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.sjlbkw.cn/Article/details/gzovjfnnx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.yfazqb.com/Article/details/gdpmyncvs.sHtML

[Q68] 保存点
来源：http://baike.fktsv.cn/Article/details/gwlvaansr.sHtML

SAVEPOINT sp1;
来源：http://m.share.sjlbkw.cn/Article/details/gpnjqaotx.sHtML

ROLLBACK TO sp1;
来源：http://wap.bbcook.cn/Article/details/gaucposoe.sHtML

[Q69] 查看执行计划
来源：http://www.blog.bbcook.cn/Article/details/glsvzcshz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.epnwcf.com/Article/details/gercggidk.sHtML

[Q70] 更新统计信息
来源：http://www.share.epnwcf.com/Article/details/gyskfetzk.sHtML

ANALYZE TABLE users;
来源：http://read.share.tarul.cn/Article/details/gtbjuwuut.sHtML

[Q71] 查看建表语句
来源：http://mobile.bbcook.cn/Article/details/ggopbleam.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.epnwcf.com/Article/details/gkvagphcl.sHtML

[Q72] 查看索引
来源：http://baike.vehdjk.com/Article/details/gpqejcjgm.sHtML

SHOW INDEX FROM users;
来源：http://blog.yfazqb.com/Article/details/githejwib.sHtML

[Q73] 查看表状态
来源：http://baike.yfazqb.com/Article/details/gfacjrrmq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fktsv.cn/Article/details/gsmtuuynq.sHtML

[Q74] 强制使用索引
来源：http://www.blog.yfazqb.com/Article/details/ghcicegon.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.epnwcf.com/Article/details/gwufuzimo.sHtML

[Q75] 日期格式化
来源：http://www.share.tarul.cn/Article/details/gwlsmicvp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.tarul.cn/Article/details/gfxatpgso.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.bbcook.cn/Article/details/gqgubgugs.sHtML

[Q76] 按天统计
来源：http://read.share.bbcook.cn/Article/details/giajdzmec.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.yfazqb.com/Article/details/glcgjgkmm.sHtML

[Q77] 时间加减
来源：http://www.blog.bbcook.cn/Article/details/grqcbnamx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.bbcook.cn/Article/details/gbzgzneqe.sHtML

[Q78] 当前时间
来源：http://baike.epnwcf.com/Article/details/gyrfwulvd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fktsv.cn/Article/details/gjeschugm.sHtML

[Q79] 字符串拼接
来源：http://read.share.vehdjk.com/Article/details/gtmoorzfg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fktsv.cn/Article/details/gpzeoorla.sHtML

[Q80] 字符串截取
来源：http://read.share.vehdjk.com/Article/details/gtffmnogu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gqapvcqnz.sHtML

[Q81] 字符串替换
来源：http://blog.vehdjk.com/Article/details/gddyakycx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.epnwcf.com/Article/details/gipszujid.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.yfazqb.com/Article/details/gizrvmrvs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gxmomehmn.sHtML

[Q83] 大小写转换
来源：http://baike.bbcook.cn/Article/details/govcaajgb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fktsv.cn/Article/details/glflaeogn.sHtML

[Q84] 去除首尾空格
来源：http://wap.sjlbkw.cn/Article/details/ggquzisfw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/grscgxoed.sHtML

[Q85] 数值取整
来源：http://m.share.tarul.cn/Article/details/grpmthgyh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.vehdjk.com/Article/details/gsvmrcbbf.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.yfazqb.com/Article/details/gklsflqjc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.tarul.cn/Article/details/glnkujkvy.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fktsv.cn/Article/details/glmblvvri.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.tarul.cn/Article/details/ghqagttfl.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.bbcook.cn/Article/details/gzhgqpgtm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.tarul.cn/Article/details/grhhxblmy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.vehdjk.com/Article/details/ghfohnjbv.sHtML

[Q89] 判断表是否存在
来源：http://mobile.tarul.cn/Article/details/gigyemhzh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.epnwcf.com/Article/details/gnwexvqhu.sHtML

[Q90] 生成序号列
来源：http://www.m.share.epnwcf.com/Article/details/grejqhfih.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.bbcook.cn/Article/details/giabniwmt.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gpmnhqeyu.sHtML

R. Bash 专题
来源：http://3g.bbcook.cn/Article/details/gbyhbhoiu.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/grhzbkhcq.sHtML

[R01] shebang 与严格模式
来源：http://blog.fktsv.cn/Article/details/gclwtyntm.sHtML

#!/usr/bin/env bash
来源：http://3g.tarul.cn/Article/details/gznvzzyme.sHtML

set -euo pipefail
来源：http://3g.epnwcf.com/Article/details/guxlazjrb.sHtML

[R02] 变量赋值与使用
来源：http://3g.bbcook.cn/Article/details/gsrizxkaq.sHtML

name="Tom"; echo "$name"
来源：http://wap.vehdjk.com/Article/details/glkembxzn.sHtML

[R03] 只读变量
来源：http://www.blog.tarul.cn/Article/details/gahphbjhm.sHtML

readonly PI=3.14
来源：http://www.share.yfazqb.com/Article/details/gaultstkw.sHtML

[R04] 位置参数
来源：http://www.share.tarul.cn/Article/details/gzhdzmvdb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.vehdjk.com/Article/details/ggnglztba.sHtML

[R05] 参数默认值
来源：http://baike.epnwcf.com/Article/details/gshkpunmd.sHtML


<!-- 参考信息 -->