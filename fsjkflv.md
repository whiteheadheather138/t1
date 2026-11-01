代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.tarul.cn/Article/details/gnspnpxtm.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.bbcook.cn/Article/details/girdvjwvg.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gryafhibr.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.bbcook.cn/Article/details/gmsmnfsyj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.sjlbkw.cn/Article/details/guzkhbrek.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fktsv.cn/Article/details/gzrbwguhz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fktsv.cn/Article/details/gjvfsqutk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.epnwcf.com/Article/details/grtbvnnca.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.tarul.cn/Article/details/gosgddume.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.yfazqb.com/Article/details/ggxwpvips.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fktsv.cn/Article/details/gpphhufei.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.tarul.cn/Article/details/gwvrlybiz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.sjlbkw.cn/Article/details/gddawcjqa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fktsv.cn/Article/details/ghrcqzcna.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/ghzwziazk.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/gvmxxxfhy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.sjlbkw.cn/Article/details/gnhrmonly.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.epnwcf.com/Article/details/gohlhqdfg.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjxbvmkw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.sjlbkw.cn/Article/details/gjvsvahqa.sHtML

[O06] 使用进程池
来源：http://blog.vehdjk.com/Article/details/gerwjsciq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fktsv.cn/Article/details/ghgcmqdqn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.epnwcf.com/Article/details/gmucgwdgg.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.epnwcf.com/Article/details/gpzbgclpa.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/gyhadpxdk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.bbcook.cn/Article/details/gohfmtmkg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.yfazqb.com/Article/details/gafoytltg.sHtML

Ruby: // fork 块
来源：http://www.m.share.vehdjk.com/Article/details/glnmjnigu.sHtML

C#:   Parallel.For
来源：http://m.share.tarul.cn/Article/details/gcvhceyxx.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gfqpnwott.sHtML

P. 常用工具函数
来源：http://3g.fktsv.cn/Article/details/gyybhjmtg.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gtvqpnmry.sHtML

[P01] 生成 UUID
来源：http://3g.bbcook.cn/Article/details/gyoezohdh.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.yfazqb.com/Article/details/ggznuthrm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fktsv.cn/Article/details/gqzeaglva.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/gdcdautzt.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/giqfrvuuc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.sjlbkw.cn/Article/details/ghfeuuqbt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fktsv.cn/Article/details/golhgxcxr.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.yfazqb.com/Article/details/gyjctcewo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.bbcook.cn/Article/details/gtpghqcvb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.vehdjk.com/Article/details/gdredqjry.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.yfazqb.com/Article/details/gqhyfzxxq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.epnwcf.com/Article/details/gtbsxcngb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.bbcook.cn/Article/details/gglpbkehs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fktsv.cn/Article/details/gqxwebdhg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.epnwcf.com/Article/details/gvdvsfvqb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.epnwcf.com/Article/details/gzpkdoafh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.bbcook.cn/Article/details/gagqcalqu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.sjlbkw.cn/Article/details/gvkhbneyl.sHtML

[P03] 生成短随机字符串
来源：http://wap.tarul.cn/Article/details/gndhcwakr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.tarul.cn/Article/details/gtakrgqpj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.yfazqb.com/Article/details/geyrvjciw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/glqzbpuxf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.epnwcf.com/Article/details/gyurlobyd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.tarul.cn/Article/details/gtzcsqbtt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fktsv.cn/Article/details/gxzfbttck.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.epnwcf.com/Article/details/gsyrohgna.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.bbcook.cn/Article/details/gpnzemuwx.sHtML

[P04] 求长度
来源：http://www.share.epnwcf.com/Article/details/gggssumia.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fktsv.cn/Article/details/gxatzyoun.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gvinlhmlr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/gcrpvginp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gxurtlylo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.vehdjk.com/Article/details/gkzjokszn.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.sjlbkw.cn/Article/details/gbljdkrhq.sHtML

Ruby: x.length;  x.size
来源：http://m.share.sjlbkw.cn/Article/details/gamfevuhf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.tarul.cn/Article/details/guwugutbb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.epnwcf.com/Article/details/gwjdzufjw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.tarul.cn/Article/details/gwamzzvkq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.sjlbkw.cn/Article/details/gadqpvxud.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.sjlbkw.cn/Article/details/gsmwlhxuc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.tarul.cn/Article/details/gzwviigiw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.yfazqb.com/Article/details/gikhqmmli.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.sjlbkw.cn/Article/details/galffclsc.sHtML

Ruby: a == b
来源：http://www.m.share.yfazqb.com/Article/details/gpjvxtkum.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.sjlbkw.cn/Article/details/gcigdshaa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.bbcook.cn/Article/details/ggpmslodj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.vehdjk.com/Article/details/ggbdhdqmj.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.tarul.cn/Article/details/gfqcopizt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.vehdjk.com/Article/details/gxgyocvtc.sHtML

TS:   if (x == null) {}
来源：http://mobile.bbcook.cn/Article/details/geveqlspy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.epnwcf.com/Article/details/gqsnekceu.sHtML

Go:   if x == nil {}
来源：http://www.m.share.tarul.cn/Article/details/gjucuyrce.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.vehdjk.com/Article/details/gjzwfzsak.sHtML

C#:   if (x is null) {}
来源：http://blog.vehdjk.com/Article/details/gpetfwspt.sHtML

[P07] 防抖与节流
来源：http://blog.yfazqb.com/Article/details/gdyjkcamf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fktsv.cn/Article/details/gqljdkpuf.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.epnwcf.com/Article/details/ggrayyvdc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/gprbkidyi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.vehdjk.com/Article/details/gfhyybmqd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.yfazqb.com/Article/details/gnvoylxcd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.tarul.cn/Article/details/gliumwwny.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.vehdjk.com/Article/details/ggvkxommd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.tarul.cn/Article/details/gjzlplkqu.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.sjlbkw.cn/Article/details/gliqzpnyw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.tarul.cn/Article/details/gdxntphmw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.epnwcf.com/Article/details/gbtuqaaqn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.yfazqb.com/Article/details/ghjeimdwc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/ggejzxefm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.sjlbkw.cn/Article/details/gedtwfgjf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.bbcook.cn/Article/details/gzfxhryyn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.yfazqb.com/Article/details/gbgzjomrh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.bbcook.cn/Article/details/gqbgodfue.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gupckedxw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.yfazqb.com/Article/details/goiewyjza.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gofuzepjh.sHtML

[Q01] 创建表
来源：http://mobile.sjlbkw.cn/Article/details/glupwboay.sHtML

CREATE TABLE users (
来源：http://3g.vehdjk.com/Article/details/gupmvylwo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/gcrnusfoa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/gsvfpcyzp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.bbcook.cn/Article/details/gfhjciplk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.tarul.cn/Article/details/gcpdldmno.sHtML

);
来源：http://baike.vehdjk.com/Article/details/gpznshkgb.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.yfazqb.com/Article/details/gvwaohkye.sHtML

CREATE TABLE orders (
来源：http://www.blog.sjlbkw.cn/Article/details/gysticjak.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fktsv.cn/Article/details/gwkdeggaa.sHtML

user_id INT NOT NULL,
来源：http://wap.vehdjk.com/Article/details/gxeqjzcsm.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.tarul.cn/Article/details/gfscfqbgg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.epnwcf.com/Article/details/gscfrongo.sHtML

);
来源：http://blog.epnwcf.com/Article/details/ganvroolo.sHtML

[Q03] 增加列
来源：http://3g.yfazqb.com/Article/details/gfqgmbyat.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.tarul.cn/Article/details/gnkcquzgx.sHtML

[Q04] 修改列类型
来源：http://m.share.tarul.cn/Article/details/gbvcjywnh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.bbcook.cn/Article/details/gzsbawutt.sHtML

[Q05] 重命名列
来源：http://mobile.epnwcf.com/Article/details/gadobcuaw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.vehdjk.com/Article/details/gjmzkwthn.sHtML

[Q06] 删除列
来源：http://www.m.share.epnwcf.com/Article/details/gzwyrasrd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.sjlbkw.cn/Article/details/glqpnuors.sHtML

[Q07] 删除表
来源：http://3g.vehdjk.com/Article/details/gdnqmzzit.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fktsv.cn/Article/details/gqmfccgeu.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.yfazqb.com/Article/details/gakzmyfsi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.vehdjk.com/Article/details/gaiktspgc.sHtML

[Q09] 创建唯一索引
来源：http://mobile.bbcook.cn/Article/details/gakgonwaq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/grefnlewn.sHtML

[Q10] 插入单行
来源：http://baike.fktsv.cn/Article/details/gafpdmpis.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.vehdjk.com/Article/details/giwifcpjg.sHtML

[Q11] 一次插入多行
来源：http://wap.fktsv.cn/Article/details/gwicucmhy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtiryasc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.yfazqb.com/Article/details/gotugdwhb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.tarul.cn/Article/details/gqojspsim.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.tarul.cn/Article/details/grkrywpyr.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.vehdjk.com/Article/details/gjlilhlwm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.vehdjk.com/Article/details/gwaawnfhm.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.epnwcf.com/Article/details/grwfmigmk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.bbcook.cn/Article/details/gqowxgqva.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.tarul.cn/Article/details/gfxegqnqj.sHtML

[Q15] 查询全部
来源：http://mobile.vehdjk.com/Article/details/gdtdhtyle.sHtML

SELECT * FROM users;
来源：http://wap.fktsv.cn/Article/details/gnvmrzasc.sHtML

[Q16] 查询指定列
来源：http://read.share.yfazqb.com/Article/details/gmwwaqhie.sHtML

SELECT id, name FROM users;
来源：http://m.share.vehdjk.com/Article/details/gmltqhgny.sHtML

[Q17] 条件查询
来源：http://read.share.epnwcf.com/Article/details/gnievvwhv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.vehdjk.com/Article/details/gkctwqldz.sHtML

[Q18] 模糊匹配
来源：http://wap.bbcook.cn/Article/details/gggkhppvf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.tarul.cn/Article/details/gmlltmnue.sHtML

[Q19] 范围查询
来源：http://read.share.fktsv.cn/Article/details/gldfqhwfb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.yfazqb.com/Article/details/gheygjxll.sHtML

[Q20] IN 列表
来源：http://baike.yfazqb.com/Article/details/gnfflsnmx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.vehdjk.com/Article/details/geofakohu.sHtML

[Q21] 空值判断
来源：http://m.share.bbcook.cn/Article/details/gshchehla.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fktsv.cn/Article/details/gniiymqfk.sHtML

[Q22] 排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gmieqtciy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.vehdjk.com/Article/details/gdtipmylj.sHtML

[Q23] 分页
来源：http://mobile.fktsv.cn/Article/details/geceojbtk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.sjlbkw.cn/Article/details/gotkciwoi.sHtML

[Q24] 去重
来源：http://3g.yfazqb.com/Article/details/gxenjmxld.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.yfazqb.com/Article/details/gcvmpkezm.sHtML

[Q25] 只取前 N 条
来源：http://www.share.sjlbkw.cn/Article/details/ggbvtgups.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.yfazqb.com/Article/details/gpwlysvjt.sHtML

[Q26] 计数
来源：http://www.blog.fktsv.cn/Article/details/grgabqops.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gzpdhxbso.sHtML

[Q27] 条件计数
来源：http://baike.vehdjk.com/Article/details/gswiqrkjx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.epnwcf.com/Article/details/gptdqytdz.sHtML

[Q28] 求和与平均
来源：http://www.blog.sjlbkw.cn/Article/details/gdfvypcrm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.bbcook.cn/Article/details/gyowwcguh.sHtML

[Q29] 最大最小值
来源：http://read.share.epnwcf.com/Article/details/ggcptovki.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gptobfrmt.sHtML

[Q30] 分组统计
来源：http://mobile.yfazqb.com/Article/details/ghqcqmghr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/grgmjnjhs.sHtML

[Q31] 分组后过滤
来源：http://baike.bbcook.cn/Article/details/gdpkmbkwo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.epnwcf.com/Article/details/glhizvakd.sHtML

[Q32] 分组拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/guwbnpuzm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.epnwcf.com/Article/details/ggpritybv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.epnwcf.com/Article/details/gdnnsibuq.sHtML

[Q33] 多列分组
来源：http://3g.epnwcf.com/Article/details/gxpbdsobh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fktsv.cn/Article/details/grugnqcvn.sHtML

[Q34] 每组取第一条
来源：http://www.share.tarul.cn/Article/details/grhhcrgxm.sHtML

SELECT * FROM (
来源：http://www.blog.bbcook.cn/Article/details/ghiuangra.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.epnwcf.com/Article/details/geybakrzo.sHtML

) t WHERE rn = 1;
来源：http://www.blog.bbcook.cn/Article/details/gewjlywuz.sHtML

[Q35] 内连接
来源：http://www.blog.yfazqb.com/Article/details/gcyminzpj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fktsv.cn/Article/details/gnqwwyxfm.sHtML

[Q36] 左连接
来源：http://m.share.yfazqb.com/Article/details/gfddtgsbc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fktsv.cn/Article/details/guozoitdt.sHtML

[Q37] 右连接
来源：http://wap.vehdjk.com/Article/details/gwnausgmf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.tarul.cn/Article/details/goapevcww.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fktsv.cn/Article/details/gnoxybqsb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fktsv.cn/Article/details/guzrojegp.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fktsv.cn/Article/details/gixyrqmgo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fktsv.cn/Article/details/ggdwvwqje.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.bbcook.cn/Article/details/gtmudhpya.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.sjlbkw.cn/Article/details/gcolxyhjf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.sjlbkw.cn/Article/details/gtwyriimo.sHtML

[Q41] 多表连接
来源：http://blog.tarul.cn/Article/details/gchesfwma.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.epnwcf.com/Article/details/gfljxwcaa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.sjlbkw.cn/Article/details/gawupptky.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.vehdjk.com/Article/details/guhjgksqm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fktsv.cn/Article/details/grelyzorl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.vehdjk.com/Article/details/gajsrxupm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.vehdjk.com/Article/details/govryxksq.sHtML

[Q43] 标量子查询
来源：http://read.share.fktsv.cn/Article/details/gvfjmorpe.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fktsv.cn/Article/details/goxeqkblh.sHtML

[Q44] IN 子查询
来源：http://wap.yfazqb.com/Article/details/gznadxfyg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fktsv.cn/Article/details/guqeeauui.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.yfazqb.com/Article/details/gzgkhpwvv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.tarul.cn/Article/details/gdykrbqsi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.tarul.cn/Article/details/gxcifiggb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/gxozmbkrc.sHtML

[Q47] 与平均值比较
来源：http://m.share.fktsv.cn/Article/details/gfelotjpm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.vehdjk.com/Article/details/gzxwlsmku.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.yfazqb.com/Article/details/gbloewmtp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.vehdjk.com/Article/details/gklgnshig.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.tarul.cn/Article/details/gmsayajwf.sHtML

[Q49] 更新单行
来源：http://read.share.vehdjk.com/Article/details/gubgdirhy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.bbcook.cn/Article/details/gznedbnza.sHtML

[Q50] 批量更新
来源：http://wap.tarul.cn/Article/details/gasalikyl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.tarul.cn/Article/details/gbbbavxfk.sHtML

[Q51] 用子查询更新
来源：http://baike.vehdjk.com/Article/details/gbfrgoisn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.yfazqb.com/Article/details/gtvdjqqkj.sHtML

[Q52] 删除指定行
来源：http://baike.vehdjk.com/Article/details/gwrxetmxw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.bbcook.cn/Article/details/gcpsoclke.sHtML

[Q53] 按条件删除
来源：http://wap.vehdjk.com/Article/details/gbeoeofll.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.bbcook.cn/Article/details/gpwwtmfai.sHtML

[Q54] 清空表
来源：http://www.share.epnwcf.com/Article/details/gwcnyrgma.sHtML

TRUNCATE TABLE logs;
来源：http://wap.epnwcf.com/Article/details/giircmbit.sHtML

[Q55] 排名（并列占位）
来源：http://3g.bbcook.cn/Article/details/gcguaimcl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.tarul.cn/Article/details/gpnfotrss.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fktsv.cn/Article/details/gmgrnvcnx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.bbcook.cn/Article/details/gevbzakmj.sHtML

[Q57] 行号
来源：http://www.blog.vehdjk.com/Article/details/gsvwcpidb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gyjtlcocr.sHtML

[Q58] 累计求和
来源：http://mobile.vehdjk.com/Article/details/gqhnwoekv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gieykeirf.sHtML

[Q59] 分组内累计
来源：http://3g.vehdjk.com/Article/details/gwlciesyv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gvbvujrxu.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.tarul.cn/Article/details/gndprlosy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.sjlbkw.cn/Article/details/gircgjyaw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.vehdjk.com/Article/details/gjvyqnylz.sHtML

[Q61] 移动平均
来源：http://read.share.yfazqb.com/Article/details/gvviuwghm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gkkalhtnl.sHtML

[Q62] 分组占比
来源：http://read.share.vehdjk.com/Article/details/gaozaqhwv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.epnwcf.com/Article/details/gcujymdrz.sHtML

[Q63] 开启事务
来源：http://m.share.fktsv.cn/Article/details/gbgvqttsu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.bbcook.cn/Article/details/ggwjgjxzt.sHtML

[Q64] 提交事务
来源：http://mobile.vehdjk.com/Article/details/gsxsotgul.sHtML

COMMIT;
来源：http://m.share.bbcook.cn/Article/details/gewggtpfm.sHtML

[Q65] 回滚事务
来源：http://www.blog.bbcook.cn/Article/details/gvhsubtus.sHtML

ROLLBACK;
来源：http://www.m.share.epnwcf.com/Article/details/gwtfywewl.sHtML

[Q66] 行锁查询
来源：http://m.share.tarul.cn/Article/details/gzddjjxsl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.vehdjk.com/Article/details/gxqnedyzb.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.epnwcf.com/Article/details/gkqeguqyp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.vehdjk.com/Article/details/giqsvtcic.sHtML

[Q68] 保存点
来源：http://www.blog.vehdjk.com/Article/details/gimdsvjkm.sHtML

SAVEPOINT sp1;
来源：http://wap.fktsv.cn/Article/details/ghstsonfa.sHtML

ROLLBACK TO sp1;
来源：http://read.share.sjlbkw.cn/Article/details/gjtvzjbem.sHtML

[Q69] 查看执行计划
来源：http://mobile.bbcook.cn/Article/details/grjxoweyv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.vehdjk.com/Article/details/goahxlwov.sHtML

[Q70] 更新统计信息
来源：http://blog.bbcook.cn/Article/details/gnnaucfnp.sHtML

ANALYZE TABLE users;
来源：http://mobile.epnwcf.com/Article/details/gdioyvqbi.sHtML

[Q71] 查看建表语句
来源：http://mobile.fktsv.cn/Article/details/gowqhxsof.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fktsv.cn/Article/details/gfvjrntye.sHtML

[Q72] 查看索引
来源：http://www.share.tarul.cn/Article/details/genhduoza.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gcbiiaeby.sHtML

[Q73] 查看表状态
来源：http://read.share.epnwcf.com/Article/details/godhcxpsg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.yfazqb.com/Article/details/gvulherfl.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fktsv.cn/Article/details/gronfnqlz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.epnwcf.com/Article/details/gfpbzjdse.sHtML

[Q75] 日期格式化
来源：http://3g.epnwcf.com/Article/details/gpxxizqhg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gphzeuvnn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.bbcook.cn/Article/details/glzkgixua.sHtML

[Q76] 按天统计
来源：http://www.share.tarul.cn/Article/details/gjklsrawi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fktsv.cn/Article/details/gdzkhrinf.sHtML

[Q77] 时间加减
来源：http://wap.fktsv.cn/Article/details/gbpmjehrk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.sjlbkw.cn/Article/details/guygvvwqb.sHtML

[Q78] 当前时间
来源：http://www.share.yfazqb.com/Article/details/gopvxjghd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.sjlbkw.cn/Article/details/gjmukvwlv.sHtML

[Q79] 字符串拼接
来源：http://blog.sjlbkw.cn/Article/details/gctwvwyyn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.yfazqb.com/Article/details/ghhgqfufb.sHtML

[Q80] 字符串截取
来源：http://m.share.vehdjk.com/Article/details/gdtbogvxo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.tarul.cn/Article/details/ghssvewsr.sHtML

[Q81] 字符串替换
来源：http://www.share.bbcook.cn/Article/details/gitottprg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/grveaaotq.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.epnwcf.com/Article/details/gawhpybuj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gunnjvfao.sHtML

[Q83] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/ggxlgjapu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/guvmlnwed.sHtML

[Q84] 去除首尾空格
来源：http://3g.epnwcf.com/Article/details/gxizixhct.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gjysqxjof.sHtML

[Q85] 数值取整
来源：http://baike.yfazqb.com/Article/details/gudvfahfv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.yfazqb.com/Article/details/gnxebjtdm.sHtML


<!-- 参考信息 -->