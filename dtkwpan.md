代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.tarul.cn/Article/details/gkqrdhqby.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.yfazqb.com/Article/details/ghdlcrmuy.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fktsv.cn/Article/details/gaewtppno.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fktsv.cn/Article/details/ghpsgkqkd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fktsv.cn/Article/details/gjywtkyjf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.bbcook.cn/Article/details/gizvnyzlu.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.tarul.cn/Article/details/gzmlyjxew.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.bbcook.cn/Article/details/gonknvbyd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.tarul.cn/Article/details/ghgdqyccy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.vehdjk.com/Article/details/gawhipaug.sHtML

Ruby: threads.map(&:join)
来源：http://blog.yfazqb.com/Article/details/gzljqwcbz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.bbcook.cn/Article/details/gdtmxhlxc.sHtML

[O06] 使用进程池
来源：http://www.blog.epnwcf.com/Article/details/gjpnoysvq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.tarul.cn/Article/details/gvrpzwywa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.epnwcf.com/Article/details/gusrjounz.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/goypykyng.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fktsv.cn/Article/details/gwiltzvtk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.epnwcf.com/Article/details/gqdhgvlax.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.yfazqb.com/Article/details/gqcnawuqe.sHtML

Ruby: // fork 块
来源：http://www.share.sjlbkw.cn/Article/details/gbkkjlxhp.sHtML

C#:   Parallel.For
来源：http://www.blog.bbcook.cn/Article/details/gtpusozuc.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gnqavvnza.sHtML

P. 常用工具函数
来源：http://baike.bbcook.cn/Article/details/glfaovzna.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gqdxusvuw.sHtML

[P01] 生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/ggugtuoxc.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.bbcook.cn/Article/details/gbpxqrozm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fktsv.cn/Article/details/gefcpisnq.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/ghdhnohps.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gvzmrkbdi.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.tarul.cn/Article/details/gaywsbklx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.bbcook.cn/Article/details/gnmscwxlz.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.tarul.cn/Article/details/gnqaibnki.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.tarul.cn/Article/details/gvbycrjma.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.bbcook.cn/Article/details/gkvayqqyp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.bbcook.cn/Article/details/ghawmbmqg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.sjlbkw.cn/Article/details/goggrjsbu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.yfazqb.com/Article/details/gzenazgrx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.yfazqb.com/Article/details/gnvstvfvm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gqhmxhzcd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.epnwcf.com/Article/details/gzzibvyeh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.sjlbkw.cn/Article/details/gnjdesijd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.yfazqb.com/Article/details/gyvsujxnr.sHtML

[P03] 生成短随机字符串
来源：http://3g.bbcook.cn/Article/details/gmahbduia.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.vehdjk.com/Article/details/gjqtdovow.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.bbcook.cn/Article/details/ghsylbobi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/gsysywkmn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.tarul.cn/Article/details/gggzwxjnc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.epnwcf.com/Article/details/gxhwjptqw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.bbcook.cn/Article/details/gylbfhyco.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.vehdjk.com/Article/details/glmyqsvmf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.sjlbkw.cn/Article/details/gcafjhmek.sHtML

[P04] 求长度
来源：http://mobile.epnwcf.com/Article/details/gibgwirll.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.tarul.cn/Article/details/grdafbyrs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gxmtfwhsw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.yfazqb.com/Article/details/gbgwntlgq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.epnwcf.com/Article/details/gmqzeswlv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.bbcook.cn/Article/details/gyburowwf.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.tarul.cn/Article/details/gwefiwhfc.sHtML

Ruby: x.length;  x.size
来源：http://read.share.sjlbkw.cn/Article/details/gmmgxmtiz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.sjlbkw.cn/Article/details/guozrrook.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.tarul.cn/Article/details/gvlhoutua.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.tarul.cn/Article/details/gqdltrpud.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.sjlbkw.cn/Article/details/gnpzpnmiv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fktsv.cn/Article/details/ggexcbvbr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.yfazqb.com/Article/details/gdyuvvtmb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.yfazqb.com/Article/details/gwdpnehif.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.vehdjk.com/Article/details/gotiwrxcr.sHtML

Ruby: a == b
来源：http://blog.fktsv.cn/Article/details/gpudcxeyb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fktsv.cn/Article/details/glegsnqjh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.vehdjk.com/Article/details/gpbdlritm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fktsv.cn/Article/details/gllcjhieu.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gyscnoetz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.yfazqb.com/Article/details/gvwlbsdeo.sHtML

TS:   if (x == null) {}
来源：http://www.share.bbcook.cn/Article/details/ginztundj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.epnwcf.com/Article/details/gesxltfkn.sHtML

Go:   if x == nil {}
来源：http://baike.fktsv.cn/Article/details/gmcfqrltv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.sjlbkw.cn/Article/details/gguiimciq.sHtML

C#:   if (x is null) {}
来源：http://read.share.tarul.cn/Article/details/gcynjayyb.sHtML

[P07] 防抖与节流
来源：http://mobile.vehdjk.com/Article/details/ghphpaewo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.bbcook.cn/Article/details/gdcfzsxjc.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.epnwcf.com/Article/details/gkrdoebdl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/gykmmnzhq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.yfazqb.com/Article/details/gghdgkmob.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.sjlbkw.cn/Article/details/gkexslltx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.vehdjk.com/Article/details/gxgfkwepw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.bbcook.cn/Article/details/gwgbciyac.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.yfazqb.com/Article/details/gulkolbaw.sHtML

[P08] 处理浮点精度问题
来源：http://3g.tarul.cn/Article/details/gnssckjvu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.tarul.cn/Article/details/gfkwyceyl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.tarul.cn/Article/details/gfdcrqcjv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.yfazqb.com/Article/details/gfxbxskiy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.yfazqb.com/Article/details/gmqogbcuc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.vehdjk.com/Article/details/glciepthj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.bbcook.cn/Article/details/gktwzfbqd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fktsv.cn/Article/details/gtxrcztgx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.tarul.cn/Article/details/gdoidaziq.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gtduvdlox.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.bbcook.cn/Article/details/gmllyvecj.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ggmmmshpn.sHtML

[Q01] 创建表
来源：http://blog.epnwcf.com/Article/details/gcnvnpamk.sHtML

CREATE TABLE users (
来源：http://baike.yfazqb.com/Article/details/gqbjsjpnm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.vehdjk.com/Article/details/gvcnixdkk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.sjlbkw.cn/Article/details/gomvdxdlk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.tarul.cn/Article/details/gpfwambqo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.tarul.cn/Article/details/gxrwzalvj.sHtML

);
来源：http://www.share.bbcook.cn/Article/details/gzwtvhnka.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.bbcook.cn/Article/details/gkqpskbva.sHtML

CREATE TABLE orders (
来源：http://m.share.tarul.cn/Article/details/grmsycqem.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.sjlbkw.cn/Article/details/gllrwsvbm.sHtML

user_id INT NOT NULL,
来源：http://wap.fktsv.cn/Article/details/gabmpxtvw.sHtML

amount DECIMAL(10, 2),
来源：http://wap.vehdjk.com/Article/details/gqbzqjpog.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.epnwcf.com/Article/details/gwgaqyczn.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gkfibvryp.sHtML

[Q03] 增加列
来源：http://3g.tarul.cn/Article/details/gmzrxwazo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fktsv.cn/Article/details/gdigrftip.sHtML

[Q04] 修改列类型
来源：http://mobile.epnwcf.com/Article/details/gsulmpgvn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fktsv.cn/Article/details/gsufqmvaz.sHtML

[Q05] 重命名列
来源：http://www.share.sjlbkw.cn/Article/details/gcjpfyvek.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.vehdjk.com/Article/details/gxmphzqmr.sHtML

[Q06] 删除列
来源：http://wap.sjlbkw.cn/Article/details/ghxsnjacj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.tarul.cn/Article/details/gezludhmq.sHtML

[Q07] 删除表
来源：http://wap.sjlbkw.cn/Article/details/gchobcpgs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.epnwcf.com/Article/details/gijrkljsv.sHtML

[Q08] 创建普通索引
来源：http://read.share.sjlbkw.cn/Article/details/gnxvmmwbw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.sjlbkw.cn/Article/details/gofdsbfgt.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fktsv.cn/Article/details/gldbtnktt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.bbcook.cn/Article/details/gooburdtz.sHtML

[Q10] 插入单行
来源：http://blog.yfazqb.com/Article/details/glyomqjmh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.bbcook.cn/Article/details/gbuyjltsy.sHtML

[Q11] 一次插入多行
来源：http://www.share.fktsv.cn/Article/details/gantjkzjf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gtufphntb.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.yfazqb.com/Article/details/gxdnhbzkz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.sjlbkw.cn/Article/details/ghuguzdgl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.epnwcf.com/Article/details/gyabkuokz.sHtML

[Q13] 忽略重复插入
来源：http://wap.bbcook.cn/Article/details/gsjdyhikt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/gygvjhuru.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.vehdjk.com/Article/details/gtevlneya.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.bbcook.cn/Article/details/glijufuvz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.sjlbkw.cn/Article/details/geaqactao.sHtML

[Q15] 查询全部
来源：http://3g.yfazqb.com/Article/details/gesvpdxnx.sHtML

SELECT * FROM users;
来源：http://wap.vehdjk.com/Article/details/gsfqoolbz.sHtML

[Q16] 查询指定列
来源：http://baike.fktsv.cn/Article/details/ghrdgygvd.sHtML

SELECT id, name FROM users;
来源：http://mobile.fktsv.cn/Article/details/gmunrzlbu.sHtML

[Q17] 条件查询
来源：http://www.blog.sjlbkw.cn/Article/details/gigcoykok.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gyikutyhs.sHtML

[Q18] 模糊匹配
来源：http://www.share.fktsv.cn/Article/details/gefjfmrxf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fktsv.cn/Article/details/gmwrxqeci.sHtML

[Q19] 范围查询
来源：http://www.share.yfazqb.com/Article/details/guzuulvut.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.epnwcf.com/Article/details/glkdeunqm.sHtML

[Q20] IN 列表
来源：http://www.share.sjlbkw.cn/Article/details/gezbdfxtj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fktsv.cn/Article/details/gjclvimcd.sHtML

[Q21] 空值判断
来源：http://m.share.tarul.cn/Article/details/gmxbuvzpv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.sjlbkw.cn/Article/details/ghmmqvaob.sHtML

[Q22] 排序
来源：http://baike.tarul.cn/Article/details/gqgdymxqp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.yfazqb.com/Article/details/gwxxmopmh.sHtML

[Q23] 分页
来源：http://www.m.share.yfazqb.com/Article/details/gwkxzxynx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.vehdjk.com/Article/details/gmetbieym.sHtML

[Q24] 去重
来源：http://www.share.bbcook.cn/Article/details/gqsfsilpr.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.tarul.cn/Article/details/grgxlzdib.sHtML

[Q25] 只取前 N 条
来源：http://wap.bbcook.cn/Article/details/gqknvshjg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.bbcook.cn/Article/details/gpwrvxtoj.sHtML

[Q26] 计数
来源：http://m.share.fktsv.cn/Article/details/gussxfrja.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.tarul.cn/Article/details/gsezmjolc.sHtML

[Q27] 条件计数
来源：http://www.share.epnwcf.com/Article/details/gdkalhyyr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.vehdjk.com/Article/details/ggumrvjsm.sHtML

[Q28] 求和与平均
来源：http://www.blog.bbcook.cn/Article/details/glesxobpl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.epnwcf.com/Article/details/gmfzdaqii.sHtML

[Q29] 最大最小值
来源：http://www.m.share.vehdjk.com/Article/details/gtvejfdfl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gjiyojjds.sHtML

[Q30] 分组统计
来源：http://3g.yfazqb.com/Article/details/gfyhyuoqo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/gxttvahsw.sHtML

[Q31] 分组后过滤
来源：http://www.blog.vehdjk.com/Article/details/gjklggjly.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.epnwcf.com/Article/details/gzkfqszze.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.epnwcf.com/Article/details/gqfcgivqd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/gxmbvsxha.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.yfazqb.com/Article/details/grjxvulxf.sHtML

[Q33] 多列分组
来源：http://blog.vehdjk.com/Article/details/gfvrxqxxz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.yfazqb.com/Article/details/gyixlcruq.sHtML

[Q34] 每组取第一条
来源：http://blog.sjlbkw.cn/Article/details/geaekluju.sHtML

SELECT * FROM (
来源：http://blog.fktsv.cn/Article/details/gdmjcvcgo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.sjlbkw.cn/Article/details/gwwuwvmjb.sHtML

) t WHERE rn = 1;
来源：http://baike.sjlbkw.cn/Article/details/gyepcvnpi.sHtML

[Q35] 内连接
来源：http://blog.bbcook.cn/Article/details/gqpjqwssc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.tarul.cn/Article/details/gpmlxfxzv.sHtML

[Q36] 左连接
来源：http://read.share.fktsv.cn/Article/details/ghwuwrwdx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.bbcook.cn/Article/details/gwgihkcau.sHtML

[Q37] 右连接
来源：http://www.blog.yfazqb.com/Article/details/grnsivlga.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.bbcook.cn/Article/details/gxdmgwath.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.epnwcf.com/Article/details/gcjdexqmy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fktsv.cn/Article/details/gycxfppsv.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.yfazqb.com/Article/details/gwatourge.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.yfazqb.com/Article/details/giqxsbdgx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fktsv.cn/Article/details/gyfrcyrtf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.epnwcf.com/Article/details/gzunxvrpi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.yfazqb.com/Article/details/gykozuetw.sHtML

[Q41] 多表连接
来源：http://blog.fktsv.cn/Article/details/gxyznnfqe.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.bbcook.cn/Article/details/gbburhlhh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fktsv.cn/Article/details/gjhwseuye.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.tarul.cn/Article/details/grbcvxsnw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxqsnxei.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.sjlbkw.cn/Article/details/gmodxktpi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.bbcook.cn/Article/details/gdyrmyltq.sHtML

[Q43] 标量子查询
来源：http://mobile.bbcook.cn/Article/details/gufbecvrz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpmiwvkm.sHtML

[Q44] IN 子查询
来源：http://baike.tarul.cn/Article/details/gqdleiikk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fktsv.cn/Article/details/glnrhrrpn.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.tarul.cn/Article/details/ghjpfzdsb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/gxzmbfoat.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.bbcook.cn/Article/details/gfnygsgiy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/gbknruieh.sHtML

[Q47] 与平均值比较
来源：http://read.share.sjlbkw.cn/Article/details/gdugqshlb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.vehdjk.com/Article/details/gdrkutged.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.vehdjk.com/Article/details/glblyfwuu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fktsv.cn/Article/details/gozvncwpj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.epnwcf.com/Article/details/guzxrzgqh.sHtML

[Q49] 更新单行
来源：http://mobile.fktsv.cn/Article/details/gyhsvpaiw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.epnwcf.com/Article/details/gxhrkbjdd.sHtML

[Q50] 批量更新
来源：http://www.blog.bbcook.cn/Article/details/ganrcqifg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.sjlbkw.cn/Article/details/gdmwyrmbj.sHtML

[Q51] 用子查询更新
来源：http://3g.vehdjk.com/Article/details/gvqszuhge.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.yfazqb.com/Article/details/gwgiurnnf.sHtML

[Q52] 删除指定行
来源：http://www.blog.tarul.cn/Article/details/gffgwlxeg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fktsv.cn/Article/details/grolgsyxm.sHtML

[Q53] 按条件删除
来源：http://read.share.vehdjk.com/Article/details/gtcpcilvd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fktsv.cn/Article/details/gmfsuunyf.sHtML

[Q54] 清空表
来源：http://m.share.yfazqb.com/Article/details/gvyctqain.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.bbcook.cn/Article/details/gajacthdg.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.tarul.cn/Article/details/gqvhlpkvi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fktsv.cn/Article/details/gzzgsoywz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.yfazqb.com/Article/details/gpeeefsnn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.vehdjk.com/Article/details/gazkqadam.sHtML

[Q57] 行号
来源：http://baike.vehdjk.com/Article/details/glumryjnu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.tarul.cn/Article/details/gykdoljup.sHtML

[Q58] 累计求和
来源：http://www.m.share.tarul.cn/Article/details/gwhexefpm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.epnwcf.com/Article/details/gyvwggjij.sHtML

[Q59] 分组内累计
来源：http://read.share.yfazqb.com/Article/details/gflxhtlac.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gisxpocku.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.yfazqb.com/Article/details/grvaizlqx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.bbcook.cn/Article/details/gwboihjxg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.tarul.cn/Article/details/gdkluxnsu.sHtML

[Q61] 移动平均
来源：http://m.share.bbcook.cn/Article/details/glxaaqtzs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gtptuaiwn.sHtML

[Q62] 分组占比
来源：http://read.share.bbcook.cn/Article/details/gjuysugug.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.vehdjk.com/Article/details/gmrmycuxa.sHtML

[Q63] 开启事务
来源：http://www.m.share.epnwcf.com/Article/details/gdxxxapmg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.yfazqb.com/Article/details/gzntgqgod.sHtML

[Q64] 提交事务
来源：http://wap.epnwcf.com/Article/details/gxqvavztk.sHtML

COMMIT;
来源：http://m.share.tarul.cn/Article/details/ghtvuzzzd.sHtML

[Q65] 回滚事务
来源：http://baike.bbcook.cn/Article/details/gmlldzmco.sHtML

ROLLBACK;
来源：http://mobile.epnwcf.com/Article/details/gvmxnwurq.sHtML

[Q66] 行锁查询
来源：http://www.share.fktsv.cn/Article/details/gxsgmuvcs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.yfazqb.com/Article/details/grhbpyrrq.sHtML

[Q67] 设置隔离级别
来源：http://m.share.sjlbkw.cn/Article/details/goilwwwzq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fktsv.cn/Article/details/gljdytccj.sHtML

[Q68] 保存点
来源：http://www.m.share.vehdjk.com/Article/details/gertdsxzz.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.bbcook.cn/Article/details/gdyojqwvb.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fktsv.cn/Article/details/gxzxxgvry.sHtML

[Q69] 查看执行计划
来源：http://3g.sjlbkw.cn/Article/details/gbpwdbtov.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.bbcook.cn/Article/details/gbqjgncqg.sHtML

[Q70] 更新统计信息
来源：http://blog.sjlbkw.cn/Article/details/gctvpbyiy.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.vehdjk.com/Article/details/gnkklsfjx.sHtML

[Q71] 查看建表语句
来源：http://m.share.fktsv.cn/Article/details/gmuppdlrl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.sjlbkw.cn/Article/details/gwybzozmh.sHtML

[Q72] 查看索引
来源：http://www.m.share.fktsv.cn/Article/details/genkiohus.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fktsv.cn/Article/details/gebuixjte.sHtML

[Q73] 查看表状态
来源：http://www.m.share.vehdjk.com/Article/details/gtermopgw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fktsv.cn/Article/details/gghnyiogy.sHtML

[Q74] 强制使用索引
来源：http://www.blog.sjlbkw.cn/Article/details/gsdwofvhp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.yfazqb.com/Article/details/gidpzxkzq.sHtML

[Q75] 日期格式化
来源：http://3g.fktsv.cn/Article/details/gthhnimvh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gvnwzfvst.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fktsv.cn/Article/details/gdhfpixgq.sHtML

[Q76] 按天统计
来源：http://blog.yfazqb.com/Article/details/gnvqkmjaz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fktsv.cn/Article/details/gnogrvkcj.sHtML

[Q77] 时间加减
来源：http://3g.fktsv.cn/Article/details/gbtioiggg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.yfazqb.com/Article/details/gbmpjkabo.sHtML

[Q78] 当前时间
来源：http://read.share.vehdjk.com/Article/details/gxabccwme.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.tarul.cn/Article/details/gzviwshvy.sHtML

[Q79] 字符串拼接
来源：http://3g.vehdjk.com/Article/details/giesjwfgn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.yfazqb.com/Article/details/geeucdtrv.sHtML

[Q80] 字符串截取
来源：http://baike.tarul.cn/Article/details/gmcbredou.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.vehdjk.com/Article/details/gafcdidja.sHtML

[Q81] 字符串替换
来源：http://mobile.sjlbkw.cn/Article/details/gilkdteah.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.epnwcf.com/Article/details/gfgsyvbel.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.yfazqb.com/Article/details/gnubtivyr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gqgamkpxz.sHtML

[Q83] 大小写转换
来源：http://baike.epnwcf.com/Article/details/geuzwrzvs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/ghwlgvppc.sHtML

[Q84] 去除首尾空格
来源：http://m.share.tarul.cn/Article/details/gdaqfznmi.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gfxsbtewc.sHtML

[Q85] 数值取整
来源：http://mobile.yfazqb.com/Article/details/grbtydmcu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.sjlbkw.cn/Article/details/gxwmhxmnq.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.yfazqb.com/Article/details/ghjxidilr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.yfazqb.com/Article/details/gkprbrsga.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.vehdjk.com/Article/details/giccmpnlg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.epnwcf.com/Article/details/gqnqhygkc.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.bbcook.cn/Article/details/gokiqxaex.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.yfazqb.com/Article/details/ggyxialye.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.vehdjk.com/Article/details/gdspyiabb.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.vehdjk.com/Article/details/gdsfpyhcd.sHtML


<!-- 参考信息 -->