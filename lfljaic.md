代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.sjlbkw.cn/Article/details/glnusfpfh.sHtML

[O03] 加锁保护共享数据
来源：http://3g.sjlbkw.cn/Article/details/gsrjeazyi.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.epnwcf.com/Article/details/gzdkxbcvv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.tarul.cn/Article/details/gpmasnyqs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.sjlbkw.cn/Article/details/gstjscdhf.sHtML

TS:   // 同 JS
来源：http://baike.tarul.cn/Article/details/gdixppjmm.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gzfvrsucr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.yfazqb.com/Article/details/guxgbycbv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.yfazqb.com/Article/details/gytsmicyi.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.bbcook.cn/Article/details/gioeavkeb.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.vehdjk.com/Article/details/gtgyvzwve.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.sjlbkw.cn/Article/details/grvwsudyd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.epnwcf.com/Article/details/gpcfergps.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.tarul.cn/Article/details/gmgoojfjw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.yfazqb.com/Article/details/gdyoejuil.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.vehdjk.com/Article/details/ggjcjtjvi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.yfazqb.com/Article/details/gtjsoqsll.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.vehdjk.com/Article/details/ggffkrnln.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fktsv.cn/Article/details/gjxyyqjml.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.epnwcf.com/Article/details/gbbjvywhs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.vehdjk.com/Article/details/grfmydhyx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.vehdjk.com/Article/details/grwszkklo.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzxwocsf.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.yfazqb.com/Article/details/ghwhiwjyk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.vehdjk.com/Article/details/gewovthwv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.sjlbkw.cn/Article/details/gdqdefwbg.sHtML

Ruby: threads.map(&:join)
来源：http://baike.sjlbkw.cn/Article/details/gwbthybrl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.bbcook.cn/Article/details/gokpgokoy.sHtML

[O06] 使用进程池
来源：http://mobile.epnwcf.com/Article/details/gykqgvmcd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fktsv.cn/Article/details/gdoidmikn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.tarul.cn/Article/details/gcirfnvyr.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fktsv.cn/Article/details/gptxkinyw.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.vehdjk.com/Article/details/gndrttlva.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.bbcook.cn/Article/details/gzxhirutx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fktsv.cn/Article/details/gyknnbybz.sHtML

Ruby: // fork 块
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxzytuos.sHtML

C#:   Parallel.For
来源：http://baike.epnwcf.com/Article/details/gpijdvnnx.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gsnihdsqv.sHtML

P. 常用工具函数
来源：http://read.share.tarul.cn/Article/details/glwlqblbg.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gjvbqifaf.sHtML

[P01] 生成 UUID
来源：http://mobile.epnwcf.com/Article/details/gwwjqnpub.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.yfazqb.com/Article/details/gjhtjujcw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.yfazqb.com/Article/details/gvtgziawh.sHtML

JS:   crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/gigvgligy.sHtML

TS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gmijyjpoj.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.yfazqb.com/Article/details/giroyyffg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.yfazqb.com/Article/details/glcskexpk.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.vehdjk.com/Article/details/gipnjzbzp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.vehdjk.com/Article/details/gvohvdjym.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.epnwcf.com/Article/details/gcoqmufnm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fktsv.cn/Article/details/gufeyulio.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.tarul.cn/Article/details/gslrigmqe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fktsv.cn/Article/details/gqakmurrm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.tarul.cn/Article/details/gclypjfcg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.tarul.cn/Article/details/gcqibxnhp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.vehdjk.com/Article/details/ggrkfkkyf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.epnwcf.com/Article/details/gejdtoban.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.epnwcf.com/Article/details/gnigylwct.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.yfazqb.com/Article/details/gesxdlqeu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.vehdjk.com/Article/details/glpvxmoij.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.tarul.cn/Article/details/gdaagqdyd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.sjlbkw.cn/Article/details/geafwbhlc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.vehdjk.com/Article/details/gzajwthwv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.epnwcf.com/Article/details/gbqivqknc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.yfazqb.com/Article/details/gloyvrfgn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.sjlbkw.cn/Article/details/gequshiid.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.bbcook.cn/Article/details/gukvwvagb.sHtML

[P04] 求长度
来源：http://www.blog.vehdjk.com/Article/details/gvzvtnlqg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.yfazqb.com/Article/details/grzwpwbuq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gqpvtwvud.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.sjlbkw.cn/Article/details/ghmyjfjor.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.vehdjk.com/Article/details/gycxsdyzo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.tarul.cn/Article/details/gixbddkyw.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.epnwcf.com/Article/details/gkozijhwq.sHtML

Ruby: x.length;  x.size
来源：http://m.share.tarul.cn/Article/details/geumadtin.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.sjlbkw.cn/Article/details/gmwooyidw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.bbcook.cn/Article/details/ggoazlmjz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.vehdjk.com/Article/details/gydytfmvw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.epnwcf.com/Article/details/gypjluqnf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.bbcook.cn/Article/details/gunjjdsce.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.yfazqb.com/Article/details/ggtkmecas.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fktsv.cn/Article/details/gdcbcomtd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.epnwcf.com/Article/details/gqisiztzh.sHtML

Ruby: a == b
来源：http://www.blog.fktsv.cn/Article/details/ggjctujoe.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fktsv.cn/Article/details/gdvurufjx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.bbcook.cn/Article/details/grbmswopl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fktsv.cn/Article/details/gfhyxpljw.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.tarul.cn/Article/details/gnndrtkxk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.vehdjk.com/Article/details/gqfxdsgqb.sHtML

TS:   if (x == null) {}
来源：http://m.share.bbcook.cn/Article/details/gwbnevwni.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/gxcjrcenj.sHtML

Go:   if x == nil {}
来源：http://m.share.sjlbkw.cn/Article/details/glmbbivbq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.yfazqb.com/Article/details/gnnhdltfc.sHtML

C#:   if (x is null) {}
来源：http://www.share.bbcook.cn/Article/details/grhpmpeao.sHtML

[P07] 防抖与节流
来源：http://www.m.share.sjlbkw.cn/Article/details/gdalwjadj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fktsv.cn/Article/details/gftmgiohd.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.bbcook.cn/Article/details/gtnwrqnja.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.vehdjk.com/Article/details/gqdgnavhl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.sjlbkw.cn/Article/details/gaadrlwyi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.epnwcf.com/Article/details/gmchtfkxp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.vehdjk.com/Article/details/ggehkopse.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.tarul.cn/Article/details/gctllsdik.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.vehdjk.com/Article/details/ghjmhmtza.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.bbcook.cn/Article/details/gkuzffsnl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fktsv.cn/Article/details/gzvzxmtab.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.epnwcf.com/Article/details/gzwtzipym.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpxeaudh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fktsv.cn/Article/details/gwpixysqc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.tarul.cn/Article/details/grzltnfyf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.yfazqb.com/Article/details/gkvmulhwi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.sjlbkw.cn/Article/details/grprxpape.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.bbcook.cn/Article/details/gaggoagxd.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gizwmwmuk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.yfazqb.com/Article/details/guedqzzrd.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ggapfqdrp.sHtML

[Q01] 创建表
来源：http://mobile.bbcook.cn/Article/details/gmkijrnef.sHtML

CREATE TABLE users (
来源：http://www.share.vehdjk.com/Article/details/gvjhucjsg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.epnwcf.com/Article/details/grmifgjdi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.sjlbkw.cn/Article/details/garffcpfy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fktsv.cn/Article/details/ggwsnwdvq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.bbcook.cn/Article/details/gidkwidnu.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/ghsgxbwwx.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.yfazqb.com/Article/details/giwuzmnnx.sHtML

CREATE TABLE orders (
来源：http://mobile.epnwcf.com/Article/details/gtuzzfjzy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.vehdjk.com/Article/details/ggumquaxd.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fktsv.cn/Article/details/gvdfdhuny.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.vehdjk.com/Article/details/gcjphfpcs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.epnwcf.com/Article/details/gndmfcqvn.sHtML

);
来源：http://www.share.vehdjk.com/Article/details/gebhwvkqh.sHtML

[Q03] 增加列
来源：http://read.share.sjlbkw.cn/Article/details/goprifgcc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.bbcook.cn/Article/details/grgxisfgr.sHtML

[Q04] 修改列类型
来源：http://wap.fktsv.cn/Article/details/gyixovefw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.sjlbkw.cn/Article/details/gjeikrbji.sHtML

[Q05] 重命名列
来源：http://3g.sjlbkw.cn/Article/details/geqzhbktn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.bbcook.cn/Article/details/gayulvemq.sHtML

[Q06] 删除列
来源：http://blog.fktsv.cn/Article/details/gjslbfnjy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.bbcook.cn/Article/details/gpashwitq.sHtML

[Q07] 删除表
来源：http://www.blog.tarul.cn/Article/details/gslabckxt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.vehdjk.com/Article/details/gepijrkwq.sHtML

[Q08] 创建普通索引
来源：http://m.share.tarul.cn/Article/details/gfzwsdfcy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.vehdjk.com/Article/details/grksgbxbn.sHtML

[Q09] 创建唯一索引
来源：http://blog.epnwcf.com/Article/details/ggvlcfgoj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.tarul.cn/Article/details/gahkasigl.sHtML

[Q10] 插入单行
来源：http://mobile.sjlbkw.cn/Article/details/gbonvxtfg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/gphzvkvdq.sHtML

[Q11] 一次插入多行
来源：http://www.blog.tarul.cn/Article/details/gibgvwmue.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.bbcook.cn/Article/details/gsjrepoic.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.sjlbkw.cn/Article/details/gejfgnviq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.bbcook.cn/Article/details/gouxeulec.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.epnwcf.com/Article/details/gjyogeaop.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.tarul.cn/Article/details/ggylreaul.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/ggmfspxzl.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fktsv.cn/Article/details/ghbcsajgo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.tarul.cn/Article/details/gxqzaosrv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fktsv.cn/Article/details/gqcknyaqz.sHtML

[Q15] 查询全部
来源：http://m.share.epnwcf.com/Article/details/gseglfqlo.sHtML

SELECT * FROM users;
来源：http://3g.yfazqb.com/Article/details/gutyuavlp.sHtML

[Q16] 查询指定列
来源：http://m.share.yfazqb.com/Article/details/giucwwxpa.sHtML

SELECT id, name FROM users;
来源：http://baike.fktsv.cn/Article/details/gqhlovezl.sHtML

[Q17] 条件查询
来源：http://blog.epnwcf.com/Article/details/gmetanokx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.vehdjk.com/Article/details/gmshhfhxd.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.tarul.cn/Article/details/gxebcchxb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.bbcook.cn/Article/details/glcrwfwfc.sHtML

[Q19] 范围查询
来源：http://blog.vehdjk.com/Article/details/gkjbbbipv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.vehdjk.com/Article/details/gdchkozch.sHtML

[Q20] IN 列表
来源：http://m.share.tarul.cn/Article/details/grgjltnzm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.vehdjk.com/Article/details/gxrmunawe.sHtML

[Q21] 空值判断
来源：http://www.share.epnwcf.com/Article/details/gegjzluoo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fktsv.cn/Article/details/gqydpusvd.sHtML

[Q22] 排序
来源：http://wap.sjlbkw.cn/Article/details/gewlhbevj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.tarul.cn/Article/details/gykqsxxxm.sHtML

[Q23] 分页
来源：http://3g.vehdjk.com/Article/details/gqbalkdym.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.vehdjk.com/Article/details/gtxaydced.sHtML

[Q24] 去重
来源：http://mobile.yfazqb.com/Article/details/gqarviflf.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.tarul.cn/Article/details/gtblhsxem.sHtML

[Q25] 只取前 N 条
来源：http://blog.fktsv.cn/Article/details/ggtlmuhke.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.yfazqb.com/Article/details/gmjpbtltj.sHtML

[Q26] 计数
来源：http://3g.sjlbkw.cn/Article/details/gwzcuepvb.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gfxhbmwzs.sHtML

[Q27] 条件计数
来源：http://www.share.fktsv.cn/Article/details/ggdxxocqv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gvbukipib.sHtML

[Q28] 求和与平均
来源：http://wap.vehdjk.com/Article/details/gnegkbgjm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gehohofak.sHtML

[Q29] 最大最小值
来源：http://baike.vehdjk.com/Article/details/gqesgakjg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gzpzqbltk.sHtML

[Q30] 分组统计
来源：http://blog.tarul.cn/Article/details/gcmqygaef.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/gkomqblas.sHtML

[Q31] 分组后过滤
来源：http://3g.tarul.cn/Article/details/gdmlfabxi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.tarul.cn/Article/details/gwrpmhwsq.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gitrogtzu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/ggcnxupqj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.sjlbkw.cn/Article/details/glffhhyxo.sHtML

[Q33] 多列分组
来源：http://www.m.share.vehdjk.com/Article/details/gyajtuqut.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.bbcook.cn/Article/details/gftfzqohm.sHtML

[Q34] 每组取第一条
来源：http://wap.sjlbkw.cn/Article/details/gyanrloyb.sHtML

SELECT * FROM (
来源：http://www.blog.sjlbkw.cn/Article/details/gkgcflmyr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.epnwcf.com/Article/details/geelvqzkb.sHtML

) t WHERE rn = 1;
来源：http://www.blog.epnwcf.com/Article/details/gijkfribm.sHtML

[Q35] 内连接
来源：http://blog.yfazqb.com/Article/details/gxhympcbi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.sjlbkw.cn/Article/details/gpyezlekb.sHtML

[Q36] 左连接
来源：http://www.m.share.yfazqb.com/Article/details/gbevmoiyk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.sjlbkw.cn/Article/details/gisvjbnqp.sHtML

[Q37] 右连接
来源：http://baike.tarul.cn/Article/details/gzlzichhp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.epnwcf.com/Article/details/gclraiwaz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.epnwcf.com/Article/details/ghankzofu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fktsv.cn/Article/details/gfaxhwndy.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.yfazqb.com/Article/details/gnkdsqgzu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.tarul.cn/Article/details/gpllloili.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.vehdjk.com/Article/details/gsytnqvqr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.sjlbkw.cn/Article/details/ggevpnjwk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.sjlbkw.cn/Article/details/ggkpnjeht.sHtML

[Q41] 多表连接
来源：http://mobile.epnwcf.com/Article/details/ghaaneewj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvkurfrh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.vehdjk.com/Article/details/gsgfphvyr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.yfazqb.com/Article/details/gxswqvwwo.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.bbcook.cn/Article/details/gjsimtzqh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.bbcook.cn/Article/details/ghzrbtauh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.sjlbkw.cn/Article/details/gqfeefkqt.sHtML

[Q43] 标量子查询
来源：http://m.share.tarul.cn/Article/details/gzunijdcq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.vehdjk.com/Article/details/gjwlxunyx.sHtML

[Q44] IN 子查询
来源：http://wap.epnwcf.com/Article/details/gbnrrhprd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fktsv.cn/Article/details/grlrmpqko.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.sjlbkw.cn/Article/details/gqcwrrwtg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.vehdjk.com/Article/details/guqrtbjva.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.tarul.cn/Article/details/ggqgowqbu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.bbcook.cn/Article/details/gskwwfqyj.sHtML

[Q47] 与平均值比较
来源：http://blog.fktsv.cn/Article/details/gfldpwaqa.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.epnwcf.com/Article/details/gqynhxrte.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.epnwcf.com/Article/details/grjpxlazy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.bbcook.cn/Article/details/gzfzifrpl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.vehdjk.com/Article/details/gtqxxspsn.sHtML

[Q49] 更新单行
来源：http://www.m.share.bbcook.cn/Article/details/gwieryzeu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.sjlbkw.cn/Article/details/gxkzuuzxz.sHtML

[Q50] 批量更新
来源：http://blog.yfazqb.com/Article/details/gzbhkjhty.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.bbcook.cn/Article/details/gnaulowxv.sHtML

[Q51] 用子查询更新
来源：http://blog.tarul.cn/Article/details/goocyvzcs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.yfazqb.com/Article/details/gmjaueazi.sHtML

[Q52] 删除指定行
来源：http://baike.epnwcf.com/Article/details/geikbqzxg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.tarul.cn/Article/details/gqeqhpfao.sHtML

[Q53] 按条件删除
来源：http://www.share.sjlbkw.cn/Article/details/gqbtgwovm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.epnwcf.com/Article/details/gruzallue.sHtML

[Q54] 清空表
来源：http://www.share.fktsv.cn/Article/details/gfznkhewl.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.yfazqb.com/Article/details/gmzbivoiq.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.bbcook.cn/Article/details/gajacckre.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.vehdjk.com/Article/details/gfxwjrtda.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.vehdjk.com/Article/details/gaxrvnnkx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.bbcook.cn/Article/details/gloylizek.sHtML

[Q57] 行号
来源：http://www.m.share.epnwcf.com/Article/details/gnmcecryb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gcyexifwc.sHtML

[Q58] 累计求和
来源：http://m.share.sjlbkw.cn/Article/details/gaoiwxyjx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gbpfwqqwg.sHtML

[Q59] 分组内累计
来源：http://www.m.share.bbcook.cn/Article/details/gnmckwodl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gzmodefok.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.tarul.cn/Article/details/gairatiij.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.vehdjk.com/Article/details/gkuhwypyp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gjtxglune.sHtML

[Q61] 移动平均
来源：http://www.m.share.yfazqb.com/Article/details/gjpwvunxx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/ggkbdhrdk.sHtML

[Q62] 分组占比
来源：http://wap.yfazqb.com/Article/details/gudynanso.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/grwaoyqqx.sHtML

[Q63] 开启事务
来源：http://blog.bbcook.cn/Article/details/ggdpzbxlf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.tarul.cn/Article/details/gbjdyewno.sHtML

[Q64] 提交事务
来源：http://wap.fktsv.cn/Article/details/guxwvkwde.sHtML

COMMIT;
来源：http://wap.yfazqb.com/Article/details/gpazkvjwh.sHtML

[Q65] 回滚事务
来源：http://www.share.vehdjk.com/Article/details/guxvzdwvy.sHtML

ROLLBACK;
来源：http://baike.tarul.cn/Article/details/gohuazhoj.sHtML

[Q66] 行锁查询
来源：http://mobile.fktsv.cn/Article/details/gcwtotqzs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.tarul.cn/Article/details/gcyvpjeaz.sHtML

[Q67] 设置隔离级别
来源：http://3g.yfazqb.com/Article/details/gkrxgitgc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.bbcook.cn/Article/details/gapndqmlh.sHtML

[Q68] 保存点
来源：http://mobile.fktsv.cn/Article/details/gcgjztbbk.sHtML

SAVEPOINT sp1;
来源：http://www.blog.vehdjk.com/Article/details/guqumsvmf.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.tarul.cn/Article/details/ggfkawgxm.sHtML

[Q69] 查看执行计划
来源：http://baike.fktsv.cn/Article/details/gpglnyhyv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.vehdjk.com/Article/details/ghjiyqdba.sHtML

[Q70] 更新统计信息
来源：http://blog.tarul.cn/Article/details/gzbbnqwbz.sHtML

ANALYZE TABLE users;
来源：http://mobile.vehdjk.com/Article/details/gkrdagqwo.sHtML

[Q71] 查看建表语句
来源：http://mobile.bbcook.cn/Article/details/gxcbqhesk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fktsv.cn/Article/details/golrazcfk.sHtML

[Q72] 查看索引
来源：http://read.share.bbcook.cn/Article/details/gpigvuxfx.sHtML

SHOW INDEX FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gnefmgsdh.sHtML

[Q73] 查看表状态
来源：http://www.m.share.epnwcf.com/Article/details/gyxpqtake.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.vehdjk.com/Article/details/gyickvdcm.sHtML

[Q74] 强制使用索引
来源：http://m.share.bbcook.cn/Article/details/gfljgswnk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.sjlbkw.cn/Article/details/gkpiyenpu.sHtML

[Q75] 日期格式化
来源：http://baike.tarul.cn/Article/details/gmaptoazv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.epnwcf.com/Article/details/gmhmrhnio.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.vehdjk.com/Article/details/gkxzlxbmw.sHtML

[Q76] 按天统计
来源：http://m.share.fktsv.cn/Article/details/gjkjpmfsq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fktsv.cn/Article/details/gkfyscsuk.sHtML

[Q77] 时间加减
来源：http://blog.bbcook.cn/Article/details/gzvwlvpae.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.bbcook.cn/Article/details/gltyswblk.sHtML

[Q78] 当前时间
来源：http://wap.epnwcf.com/Article/details/gesbioebn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.sjlbkw.cn/Article/details/gslhlzebz.sHtML

[Q79] 字符串拼接
来源：http://www.blog.sjlbkw.cn/Article/details/gjsnidilj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.sjlbkw.cn/Article/details/glchtjgvz.sHtML

[Q80] 字符串截取
来源：http://baike.sjlbkw.cn/Article/details/gqpclmnix.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.bbcook.cn/Article/details/grrgeyxtu.sHtML

[Q81] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/gvunvnzzz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fktsv.cn/Article/details/gkbolumkb.sHtML


<!-- 参考信息 -->