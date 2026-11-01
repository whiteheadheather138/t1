代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.bbcook.cn/Article/details/gdshmluft.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.sjlbkw.cn/Article/details/gcyqczkcw.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.sjlbkw.cn/Article/details/gttmzcplv.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.tarul.cn/Article/details/gunirkysl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gcsfspxgc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.sjlbkw.cn/Article/details/ghjfjjjyd.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/gqnzvkshq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gycwkvgha.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.epnwcf.com/Article/details/gqcbwhqsd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.bbcook.cn/Article/details/ggfjntuxf.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.sjlbkw.cn/Article/details/gysblsaki.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.yfazqb.com/Article/details/gjwlnjsrx.sHtML

[O06] 使用进程池
来源：http://mobile.fktsv.cn/Article/details/gebhvuuzl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.epnwcf.com/Article/details/gaxdpkcix.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.tarul.cn/Article/details/gomycfakq.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.yfazqb.com/Article/details/gctuiojev.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/gbrtwjzpc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.sjlbkw.cn/Article/details/gmlfbrwwn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fktsv.cn/Article/details/giuazxlhb.sHtML

Ruby: // fork 块
来源：http://read.share.bbcook.cn/Article/details/gcnwydagl.sHtML

C#:   Parallel.For
来源：http://m.share.fktsv.cn/Article/details/gydoicfax.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gzmkisxlq.sHtML

P. 常用工具函数
来源：http://baike.sjlbkw.cn/Article/details/glkylinth.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/guxwgzzny.sHtML

[P01] 生成 UUID
来源：http://www.blog.sjlbkw.cn/Article/details/gtclrtuiz.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.epnwcf.com/Article/details/gzhgyjgwa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.tarul.cn/Article/details/gcmbojowj.sHtML

JS:   crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/gecwnlzqo.sHtML

TS:   crypto.randomUUID()
来源：http://3g.epnwcf.com/Article/details/gyahiqgss.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.vehdjk.com/Article/details/gwglsguhh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.tarul.cn/Article/details/gdearqogt.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzqmvbln.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.yfazqb.com/Article/details/gwpjebufw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.sjlbkw.cn/Article/details/gfqgbdpzf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.tarul.cn/Article/details/gwsldrvqa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.yfazqb.com/Article/details/gafauuvho.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fktsv.cn/Article/details/ggllokkqt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.sjlbkw.cn/Article/details/gqufkjsdo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdiyeesz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.yfazqb.com/Article/details/gweqttpqh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.epnwcf.com/Article/details/gbkapvevq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.epnwcf.com/Article/details/gphtgynqe.sHtML

[P03] 生成短随机字符串
来源：http://mobile.yfazqb.com/Article/details/gylefavcb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.bbcook.cn/Article/details/gwhqdfedm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.tarul.cn/Article/details/gifgzyqmj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.bbcook.cn/Article/details/gdiybibnc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fktsv.cn/Article/details/gobryoqeh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.yfazqb.com/Article/details/gyppsebdr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.bbcook.cn/Article/details/gsecjujom.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.vehdjk.com/Article/details/gzjnxtoxe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.vehdjk.com/Article/details/gzdttdxpd.sHtML

[P04] 求长度
来源：http://www.blog.bbcook.cn/Article/details/gygemdlgs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.sjlbkw.cn/Article/details/giydtpczc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gkhldifdd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.epnwcf.com/Article/details/gzotawtgv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.yfazqb.com/Article/details/gpnaiumxo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.epnwcf.com/Article/details/gmynsmnwx.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.yfazqb.com/Article/details/gndzcqxrj.sHtML

Ruby: x.length;  x.size
来源：http://baike.vehdjk.com/Article/details/guffngghb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.vehdjk.com/Article/details/gnqkkibzi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.tarul.cn/Article/details/gowqnaztk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.sjlbkw.cn/Article/details/gaoazoniz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.vehdjk.com/Article/details/gveaqvlqd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.yfazqb.com/Article/details/geotyxokg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.vehdjk.com/Article/details/gjybirhke.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.bbcook.cn/Article/details/gsmnepgsy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.epnwcf.com/Article/details/goiytyajl.sHtML

Ruby: a == b
来源：http://wap.tarul.cn/Article/details/gmdjdlqko.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.epnwcf.com/Article/details/gotbgftvq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.bbcook.cn/Article/details/glymbwgab.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.epnwcf.com/Article/details/gtmibpwsw.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fktsv.cn/Article/details/gfmqywngp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.epnwcf.com/Article/details/gcobyogpk.sHtML

TS:   if (x == null) {}
来源：http://3g.sjlbkw.cn/Article/details/guburyzie.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.sjlbkw.cn/Article/details/ggyfrwvdw.sHtML

Go:   if x == nil {}
来源：http://baike.yfazqb.com/Article/details/gtaubziga.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.tarul.cn/Article/details/gmbxwbhhi.sHtML

C#:   if (x is null) {}
来源：http://3g.tarul.cn/Article/details/googewrfv.sHtML

[P07] 防抖与节流
来源：http://wap.tarul.cn/Article/details/goaohsqxn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.sjlbkw.cn/Article/details/glscdguzk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fktsv.cn/Article/details/gfcnqlzqi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/gxqyihwnj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gqoqwalql.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.bbcook.cn/Article/details/gqylskrmp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fktsv.cn/Article/details/ggddvwvzl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.yfazqb.com/Article/details/gedmxrrgh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.sjlbkw.cn/Article/details/gpltrhnqv.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.sjlbkw.cn/Article/details/gknaxymso.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.yfazqb.com/Article/details/ghgocwgoa.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.yfazqb.com/Article/details/gsvsnvyoq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.epnwcf.com/Article/details/gyzlgigtd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.epnwcf.com/Article/details/gzyyjcpgp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.tarul.cn/Article/details/gxkjwpnks.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.yfazqb.com/Article/details/ggsnegfcl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.vehdjk.com/Article/details/gpozdcplz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.bbcook.cn/Article/details/gqmqlxpse.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gwucoblel.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fktsv.cn/Article/details/giyjytfhl.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/ghwzpmcih.sHtML

[Q01] 创建表
来源：http://baike.tarul.cn/Article/details/grrsuextd.sHtML

CREATE TABLE users (
来源：http://m.share.yfazqb.com/Article/details/gfhpgapcl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.vehdjk.com/Article/details/gkxebbrra.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.epnwcf.com/Article/details/gpnhomsge.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.epnwcf.com/Article/details/gknppuvop.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.bbcook.cn/Article/details/gobgijyjm.sHtML

);
来源：http://wap.yfazqb.com/Article/details/gjzntbwhi.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.tarul.cn/Article/details/gyuaelgaz.sHtML

CREATE TABLE orders (
来源：http://read.share.epnwcf.com/Article/details/gteluhzti.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.sjlbkw.cn/Article/details/gdzgwmmfu.sHtML

user_id INT NOT NULL,
来源：http://www.share.tarul.cn/Article/details/gdqwnnumy.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.vehdjk.com/Article/details/gvkyrlpri.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.yfazqb.com/Article/details/gkvuaikuc.sHtML

);
来源：http://mobile.vehdjk.com/Article/details/gusttxrwc.sHtML

[Q03] 增加列
来源：http://m.share.sjlbkw.cn/Article/details/gxtmcqqwv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.epnwcf.com/Article/details/gtlbowbde.sHtML

[Q04] 修改列类型
来源：http://baike.sjlbkw.cn/Article/details/geualqbnj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.sjlbkw.cn/Article/details/gwzfrqrtk.sHtML

[Q05] 重命名列
来源：http://mobile.vehdjk.com/Article/details/gthmhcqmr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.epnwcf.com/Article/details/ghzabzxmg.sHtML

[Q06] 删除列
来源：http://blog.yfazqb.com/Article/details/gnhwoayaz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fktsv.cn/Article/details/gjbiworei.sHtML

[Q07] 删除表
来源：http://baike.yfazqb.com/Article/details/gizgjaoon.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.epnwcf.com/Article/details/gudkjnlmd.sHtML

[Q08] 创建普通索引
来源：http://read.share.sjlbkw.cn/Article/details/gxdlycdjt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/gwpkjonht.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.yfazqb.com/Article/details/gjkydoxju.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/gsupahprt.sHtML

[Q10] 插入单行
来源：http://mobile.sjlbkw.cn/Article/details/gbmdtargp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gchyxyele.sHtML

[Q11] 一次插入多行
来源：http://www.blog.bbcook.cn/Article/details/geooucymz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.epnwcf.com/Article/details/gfdvblmox.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.epnwcf.com/Article/details/gkbglzvmg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.bbcook.cn/Article/details/gwyxgbllv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.yfazqb.com/Article/details/gmfwiozaz.sHtML

[Q13] 忽略重复插入
来源：http://mobile.epnwcf.com/Article/details/gdrlwdzrh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fktsv.cn/Article/details/gpbpcpvca.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.bbcook.cn/Article/details/grdrlyleg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.sjlbkw.cn/Article/details/gtcusmknm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.epnwcf.com/Article/details/gqpxdbrlo.sHtML

[Q15] 查询全部
来源：http://wap.epnwcf.com/Article/details/gsdvhtoiw.sHtML

SELECT * FROM users;
来源：http://mobile.vehdjk.com/Article/details/gftpvaiib.sHtML

[Q16] 查询指定列
来源：http://m.share.epnwcf.com/Article/details/glpiqkyav.sHtML

SELECT id, name FROM users;
来源：http://baike.tarul.cn/Article/details/gcqihetmx.sHtML

[Q17] 条件查询
来源：http://m.share.vehdjk.com/Article/details/gylnmnayi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.bbcook.cn/Article/details/gjnzmsvqg.sHtML

[Q18] 模糊匹配
来源：http://3g.bbcook.cn/Article/details/gihaienma.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fktsv.cn/Article/details/gtoiobeco.sHtML

[Q19] 范围查询
来源：http://read.share.yfazqb.com/Article/details/gcfqxrpte.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.epnwcf.com/Article/details/gswaxcqsp.sHtML

[Q20] IN 列表
来源：http://read.share.epnwcf.com/Article/details/gakxeukjc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.sjlbkw.cn/Article/details/gbozvlwzt.sHtML

[Q21] 空值判断
来源：http://blog.sjlbkw.cn/Article/details/gujchuurp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.bbcook.cn/Article/details/gvawphhvs.sHtML

[Q22] 排序
来源：http://m.share.vehdjk.com/Article/details/gczcfjxyp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.vehdjk.com/Article/details/gvkoznwua.sHtML

[Q23] 分页
来源：http://www.blog.yfazqb.com/Article/details/ganivcyti.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.epnwcf.com/Article/details/gabktyzvd.sHtML

[Q24] 去重
来源：http://wap.sjlbkw.cn/Article/details/gthldxckh.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.tarul.cn/Article/details/ginjnmodr.sHtML

[Q25] 只取前 N 条
来源：http://read.share.yfazqb.com/Article/details/gcnjxviap.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fktsv.cn/Article/details/gsknoxjwl.sHtML

[Q26] 计数
来源：http://www.m.share.bbcook.cn/Article/details/gylfdncpp.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gbfsmpklk.sHtML

[Q27] 条件计数
来源：http://wap.bbcook.cn/Article/details/gmcbuimzq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.yfazqb.com/Article/details/gzfrwizgf.sHtML

[Q28] 求和与平均
来源：http://wap.tarul.cn/Article/details/gcbpkjuka.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gypwolkvt.sHtML

[Q29] 最大最小值
来源：http://wap.tarul.cn/Article/details/ghdifkclb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fktsv.cn/Article/details/ghotomsdi.sHtML

[Q30] 分组统计
来源：http://blog.epnwcf.com/Article/details/gljhtophd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/gigydnpmu.sHtML

[Q31] 分组后过滤
来源：http://read.share.fktsv.cn/Article/details/grwkhklfr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fktsv.cn/Article/details/gwahipjhp.sHtML

[Q32] 分组拼接字符串
来源：http://baike.tarul.cn/Article/details/gvcjgzrqb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gtpdhrnmg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fktsv.cn/Article/details/gnnkvzloo.sHtML

[Q33] 多列分组
来源：http://mobile.vehdjk.com/Article/details/gapuchyuo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.sjlbkw.cn/Article/details/gjruftocx.sHtML

[Q34] 每组取第一条
来源：http://read.share.epnwcf.com/Article/details/gbaxbavbm.sHtML

SELECT * FROM (
来源：http://m.share.vehdjk.com/Article/details/gbgkwgbra.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.vehdjk.com/Article/details/gnvxzqyro.sHtML

) t WHERE rn = 1;
来源：http://wap.yfazqb.com/Article/details/ggdgnwifn.sHtML

[Q35] 内连接
来源：http://3g.sjlbkw.cn/Article/details/gkternook.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/gmolyvfpe.sHtML

[Q36] 左连接
来源：http://mobile.bbcook.cn/Article/details/gtawsgbgg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/gcdafssbq.sHtML

[Q37] 右连接
来源：http://m.share.sjlbkw.cn/Article/details/gzzeiqpxv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.tarul.cn/Article/details/gbnhgihae.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.sjlbkw.cn/Article/details/gmeodpmkx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.epnwcf.com/Article/details/goqffiwfh.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.vehdjk.com/Article/details/gcgetdgye.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fktsv.cn/Article/details/gtilezeml.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.epnwcf.com/Article/details/gdzycgzmj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.bbcook.cn/Article/details/gwrlpnmnd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.vehdjk.com/Article/details/gwvywmptw.sHtML

[Q41] 多表连接
来源：http://www.share.sjlbkw.cn/Article/details/gstiedhgq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fktsv.cn/Article/details/gccbqmrbw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.yfazqb.com/Article/details/ggcvkwjjg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.bbcook.cn/Article/details/gzmtrmknb.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.tarul.cn/Article/details/gjzddigkg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.epnwcf.com/Article/details/gzbgeztws.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.sjlbkw.cn/Article/details/gadawteky.sHtML

[Q43] 标量子查询
来源：http://wap.sjlbkw.cn/Article/details/gknttvwea.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.vehdjk.com/Article/details/gmzigdvxa.sHtML

[Q44] IN 子查询
来源：http://blog.tarul.cn/Article/details/gyiqeflck.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fktsv.cn/Article/details/gxowopefj.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fktsv.cn/Article/details/gfssoqcon.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gzztwekgf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fktsv.cn/Article/details/gxewhgctd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.sjlbkw.cn/Article/details/gsonrtyum.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvnbsaac.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.bbcook.cn/Article/details/gkmgfxjku.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.vehdjk.com/Article/details/gpeudbwyt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.sjlbkw.cn/Article/details/gpogourfs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.yfazqb.com/Article/details/gqaaozpzs.sHtML

[Q49] 更新单行
来源：http://www.m.share.vehdjk.com/Article/details/ggrvbhufm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/gvsataxal.sHtML

[Q50] 批量更新
来源：http://read.share.bbcook.cn/Article/details/gqaoaafvz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.tarul.cn/Article/details/gkwnfidmg.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.tarul.cn/Article/details/gxgqogigy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.yfazqb.com/Article/details/glzhijhpn.sHtML

[Q52] 删除指定行
来源：http://mobile.sjlbkw.cn/Article/details/gtcgrypct.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.sjlbkw.cn/Article/details/giowzaocm.sHtML

[Q53] 按条件删除
来源：http://m.share.tarul.cn/Article/details/gehhfoops.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.yfazqb.com/Article/details/gnnkpyyyt.sHtML

[Q54] 清空表
来源：http://blog.yfazqb.com/Article/details/gjodwywxj.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.epnwcf.com/Article/details/gbxprtpkg.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.tarul.cn/Article/details/gfodaniuz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.vehdjk.com/Article/details/gkglwfodb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.yfazqb.com/Article/details/gnbknvwlj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.bbcook.cn/Article/details/gszwglczf.sHtML

[Q57] 行号
来源：http://www.blog.fktsv.cn/Article/details/gkhxaecks.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.tarul.cn/Article/details/gpaogfxjk.sHtML

[Q58] 累计求和
来源：http://wap.yfazqb.com/Article/details/gnvafbfal.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.bbcook.cn/Article/details/gqyzyvwsk.sHtML

[Q59] 分组内累计
来源：http://m.share.tarul.cn/Article/details/gqecvjiaz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrthwwfd.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.bbcook.cn/Article/details/gmbkkzrec.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.sjlbkw.cn/Article/details/gvknpraen.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/guwdtxlev.sHtML

[Q61] 移动平均
来源：http://blog.vehdjk.com/Article/details/gpgzqwiqo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.tarul.cn/Article/details/gcudsbaqt.sHtML

[Q62] 分组占比
来源：http://m.share.sjlbkw.cn/Article/details/gbychvkgu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/gsbnwjxnx.sHtML

[Q63] 开启事务
来源：http://m.share.sjlbkw.cn/Article/details/gtsjugmer.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.yfazqb.com/Article/details/gokydpamy.sHtML

[Q64] 提交事务
来源：http://baike.yfazqb.com/Article/details/gbdkxbjdo.sHtML

COMMIT;
来源：http://mobile.vehdjk.com/Article/details/grujbexuf.sHtML

[Q65] 回滚事务
来源：http://mobile.fktsv.cn/Article/details/gtqetvrhh.sHtML

ROLLBACK;
来源：http://www.m.share.yfazqb.com/Article/details/ghnemvhtv.sHtML

[Q66] 行锁查询
来源：http://mobile.yfazqb.com/Article/details/gwkcsxfcs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.tarul.cn/Article/details/gavxxriyt.sHtML

[Q67] 设置隔离级别
来源：http://baike.bbcook.cn/Article/details/gfkgpfyld.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.yfazqb.com/Article/details/gqqvihiyf.sHtML

[Q68] 保存点
来源：http://www.blog.bbcook.cn/Article/details/ggcahmobh.sHtML

SAVEPOINT sp1;
来源：http://baike.tarul.cn/Article/details/gpenlgtve.sHtML

ROLLBACK TO sp1;
来源：http://blog.tarul.cn/Article/details/gyeffcvxr.sHtML

[Q69] 查看执行计划
来源：http://www.blog.vehdjk.com/Article/details/gbbtvooxb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.tarul.cn/Article/details/gkaulxxnh.sHtML

[Q70] 更新统计信息
来源：http://read.share.vehdjk.com/Article/details/gfhxwevds.sHtML

ANALYZE TABLE users;
来源：http://baike.tarul.cn/Article/details/gfqzvbreq.sHtML

[Q71] 查看建表语句
来源：http://3g.vehdjk.com/Article/details/grabpfqwm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.vehdjk.com/Article/details/gcehjdmxp.sHtML

[Q72] 查看索引
来源：http://mobile.epnwcf.com/Article/details/gheekrknt.sHtML

SHOW INDEX FROM users;
来源：http://www.share.vehdjk.com/Article/details/gimmjaptn.sHtML

[Q73] 查看表状态
来源：http://baike.tarul.cn/Article/details/gfpemrmym.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.epnwcf.com/Article/details/gbnwjvemm.sHtML

[Q74] 强制使用索引
来源：http://3g.tarul.cn/Article/details/gmlnyjcku.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fktsv.cn/Article/details/gwwuynuzi.sHtML

[Q75] 日期格式化
来源：http://baike.epnwcf.com/Article/details/gbsjpdvyz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gdwuvfnbr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.tarul.cn/Article/details/garjczgpi.sHtML

[Q76] 按天统计
来源：http://www.share.sjlbkw.cn/Article/details/gnhcdaodd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.epnwcf.com/Article/details/gdxeqqqro.sHtML

[Q77] 时间加减
来源：http://mobile.yfazqb.com/Article/details/gjytryfvz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.tarul.cn/Article/details/gahsgzhst.sHtML

[Q78] 当前时间
来源：http://read.share.fktsv.cn/Article/details/gfkajohzq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.epnwcf.com/Article/details/ggphielca.sHtML

[Q79] 字符串拼接
来源：http://3g.yfazqb.com/Article/details/ggalsrmou.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.sjlbkw.cn/Article/details/gfdnpjlyl.sHtML

[Q80] 字符串截取
来源：http://wap.tarul.cn/Article/details/gqkvydicv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gdoaajdsp.sHtML

[Q81] 字符串替换
来源：http://wap.fktsv.cn/Article/details/gzkhxxvnq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.vehdjk.com/Article/details/ghvrpwyhk.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fktsv.cn/Article/details/gbykkxtck.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gfmnsrnux.sHtML

[Q83] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/gkgkavdqq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gqcvahdtp.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.tarul.cn/Article/details/gyfkqsyra.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gusfbfaho.sHtML

[Q85] 数值取整
来源：http://blog.epnwcf.com/Article/details/gesjternq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fktsv.cn/Article/details/gseasvpbm.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.sjlbkw.cn/Article/details/gjknocmhp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.epnwcf.com/Article/details/gsfcwsfob.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.vehdjk.com/Article/details/gijxvdbqx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.epnwcf.com/Article/details/grsoikqbw.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fktsv.cn/Article/details/grslfnhzn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.epnwcf.com/Article/details/gmpqunnmx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.vehdjk.com/Article/details/gcqfjcfkx.sHtML

[Q89] 判断表是否存在
来源：http://m.share.yfazqb.com/Article/details/gcxvwvfsb.sHtML


<!-- 参考信息 -->