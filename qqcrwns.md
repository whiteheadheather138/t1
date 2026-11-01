代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://3g.tarul.cn/Article/details/ggfoztlqt.sHtML

Go:   go f()
来源：http://wap.tarul.cn/Article/details/glepvqmih.sHtML

Ruby: Thread.new { f }
来源：http://3g.sjlbkw.cn/Article/details/gmonewyqs.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.epnwcf.com/Article/details/glebhvimt.sHtML

[O02] 使用线程池
来源：http://3g.bbcook.cn/Article/details/gzbjepjmi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.bbcook.cn/Article/details/gzswdvuci.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fktsv.cn/Article/details/gvyvboavd.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fktsv.cn/Article/details/gkhucfezc.sHtML

TS:   // worker_threads 线程池
来源：http://baike.epnwcf.com/Article/details/gdwlkpcot.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.sjlbkw.cn/Article/details/genbuofjr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.epnwcf.com/Article/details/ggxjuzsso.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fktsv.cn/Article/details/gxqouexza.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.tarul.cn/Article/details/gstoblyys.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.epnwcf.com/Article/details/gvsgbwdoe.sHtML

Py:   with lock: shared += 1
来源：http://mobile.vehdjk.com/Article/details/gtgvaiabv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.sjlbkw.cn/Article/details/gaxatndmo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.sjlbkw.cn/Article/details/gpruvaxuv.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/gqgzpokjg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.tarul.cn/Article/details/ghvkbahtw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.yfazqb.com/Article/details/gtilvrogl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fktsv.cn/Article/details/geslcxhbg.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.epnwcf.com/Article/details/gukkvjorf.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.vehdjk.com/Article/details/gdxddacft.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.vehdjk.com/Article/details/gblfhffza.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.epnwcf.com/Article/details/gsnbvcrzy.sHtML

JS:   async function f() { await g(); }
来源：http://blog.tarul.cn/Article/details/guosmavje.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fktsv.cn/Article/details/gbglpweab.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fktsv.cn/Article/details/gfvhyrxqb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.tarul.cn/Article/details/gavttcebm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fktsv.cn/Article/details/ghunvyino.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.bbcook.cn/Article/details/gcfcibmou.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fktsv.cn/Article/details/gqioleylw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.vehdjk.com/Article/details/gssshzsxe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.bbcook.cn/Article/details/glspsngxd.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.sjlbkw.cn/Article/details/gogtaveer.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.vehdjk.com/Article/details/gassltcls.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.epnwcf.com/Article/details/gyxlxrwdl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fktsv.cn/Article/details/gdxmxfudx.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.sjlbkw.cn/Article/details/ghztdycky.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.sjlbkw.cn/Article/details/gtdleiirn.sHtML

[O06] 使用进程池
来源：http://wap.vehdjk.com/Article/details/gsxadmcju.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.sjlbkw.cn/Article/details/gpexkoxrd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fktsv.cn/Article/details/gexvziatj.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.epnwcf.com/Article/details/ghqsknprz.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.vehdjk.com/Article/details/glkosoubp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.tarul.cn/Article/details/gkbqxsnvk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.vehdjk.com/Article/details/gxwuadrmq.sHtML

Ruby: // fork 块
来源：http://www.blog.vehdjk.com/Article/details/gbrjflnrt.sHtML

C#:   Parallel.For
来源：http://3g.tarul.cn/Article/details/gjsrjmjgz.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gfefjhuiw.sHtML

P. 常用工具函数
来源：http://3g.sjlbkw.cn/Article/details/geypxytqf.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gjlemfmbd.sHtML

[P01] 生成 UUID
来源：http://mobile.tarul.cn/Article/details/gdotynfeb.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.tarul.cn/Article/details/gdngpcjem.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.vehdjk.com/Article/details/gjjqwdpas.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/gbodgmulb.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gpzuyoiwb.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.yfazqb.com/Article/details/gqqfaujyo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.yfazqb.com/Article/details/gifjwuxfz.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.tarul.cn/Article/details/gwfnowiuy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.bbcook.cn/Article/details/gazoqvslk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.epnwcf.com/Article/details/gbkamwpez.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.tarul.cn/Article/details/gqhazliai.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.tarul.cn/Article/details/gfcjvlarc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.tarul.cn/Article/details/gdevhapbf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.sjlbkw.cn/Article/details/gvsjrlqxl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.vehdjk.com/Article/details/gdbqtrknl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fktsv.cn/Article/details/gcprdkxst.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.bbcook.cn/Article/details/gdnpxrbcu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.yfazqb.com/Article/details/gokgdkmkn.sHtML

[P03] 生成短随机字符串
来源：http://mobile.sjlbkw.cn/Article/details/glynslicr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.tarul.cn/Article/details/grkccvdnq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.yfazqb.com/Article/details/gplxcuzau.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.epnwcf.com/Article/details/gytwexywx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.epnwcf.com/Article/details/guetxzrxn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fktsv.cn/Article/details/gxrirhojb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.yfazqb.com/Article/details/gpebbkrsx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.tarul.cn/Article/details/gvumxhatd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.epnwcf.com/Article/details/gchetcqcl.sHtML

[P04] 求长度
来源：http://blog.tarul.cn/Article/details/ggbnxqcit.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fktsv.cn/Article/details/gqhwtlhms.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gsltvduld.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.epnwcf.com/Article/details/gdybgivod.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gvnkapoxd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.epnwcf.com/Article/details/gvybqfjjn.sHtML

Go:   len(arr);  len(m)
来源：http://blog.bbcook.cn/Article/details/gnvqvbaqd.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.vehdjk.com/Article/details/gjoifuefu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.sjlbkw.cn/Article/details/gvoddhpge.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.sjlbkw.cn/Article/details/gwlzyjvws.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.vehdjk.com/Article/details/gjfplqrhe.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.tarul.cn/Article/details/ggapdtaob.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.sjlbkw.cn/Article/details/giytwqtqj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gveeynamd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.sjlbkw.cn/Article/details/gsrknykcu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.vehdjk.com/Article/details/gfjnuyopr.sHtML

Ruby: a == b
来源：http://3g.yfazqb.com/Article/details/ganwsehgk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fktsv.cn/Article/details/gbxdjfkxs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.vehdjk.com/Article/details/gqtuidfep.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.bbcook.cn/Article/details/gbpjwrjce.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fktsv.cn/Article/details/gwqjmxgsx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.vehdjk.com/Article/details/gbrnrquje.sHtML

TS:   if (x == null) {}
来源：http://blog.fktsv.cn/Article/details/ggqklrayc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/glcxscukx.sHtML

Go:   if x == nil {}
来源：http://m.share.yfazqb.com/Article/details/gwvfuyjiv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fktsv.cn/Article/details/gpaofuohj.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.epnwcf.com/Article/details/gbpiiewrb.sHtML

[P07] 防抖与节流
来源：http://m.share.yfazqb.com/Article/details/gcbrokwda.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fktsv.cn/Article/details/gojerjshd.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.bbcook.cn/Article/details/gmhhlcyhu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/gsveverdl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/gqarlulea.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.bbcook.cn/Article/details/gmeyvnkdw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.yfazqb.com/Article/details/ghlgvyfej.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.tarul.cn/Article/details/ggsujhoqr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.tarul.cn/Article/details/ggiruqtyi.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.yfazqb.com/Article/details/gvnnxujjc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.tarul.cn/Article/details/gpjtsxhvi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.tarul.cn/Article/details/gfidllwax.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fktsv.cn/Article/details/gzgyizpyp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.yfazqb.com/Article/details/gujtxzneq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fktsv.cn/Article/details/gfyrtxbxu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.epnwcf.com/Article/details/gbdkgqqmz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.vehdjk.com/Article/details/gakljnbqu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.tarul.cn/Article/details/gdvsakyvu.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gdhtdiwci.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.bbcook.cn/Article/details/gfprnxgqn.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gtuumxteo.sHtML

[Q01] 创建表
来源：http://wap.bbcook.cn/Article/details/gysxdparo.sHtML

CREATE TABLE users (
来源：http://blog.sjlbkw.cn/Article/details/grhonbtev.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.epnwcf.com/Article/details/gwuddlodq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.sjlbkw.cn/Article/details/ggklzwplc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.yfazqb.com/Article/details/ggdppwnmx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.epnwcf.com/Article/details/gmmruqgby.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/gnbwnutro.sHtML

[Q02] 创建带外键的表
来源：http://www.share.epnwcf.com/Article/details/gisyibwdj.sHtML

CREATE TABLE orders (
来源：http://read.share.yfazqb.com/Article/details/gddqwyaio.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.yfazqb.com/Article/details/gxvzqgnmf.sHtML

user_id INT NOT NULL,
来源：http://baike.yfazqb.com/Article/details/goirrspli.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.vehdjk.com/Article/details/gtjrlogzy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.sjlbkw.cn/Article/details/gtjhstpcc.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gwgsyspmq.sHtML

[Q03] 增加列
来源：http://blog.yfazqb.com/Article/details/gfjcfsteb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.sjlbkw.cn/Article/details/gjithwecr.sHtML

[Q04] 修改列类型
来源：http://m.share.fktsv.cn/Article/details/goredplpj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.tarul.cn/Article/details/getrkqffk.sHtML

[Q05] 重命名列
来源：http://mobile.sjlbkw.cn/Article/details/gkntpcops.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.epnwcf.com/Article/details/gfkqzigfp.sHtML

[Q06] 删除列
来源：http://3g.fktsv.cn/Article/details/gffugsxpv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.bbcook.cn/Article/details/gbwagioye.sHtML

[Q07] 删除表
来源：http://m.share.bbcook.cn/Article/details/ghtckqzek.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.tarul.cn/Article/details/gssxckdhv.sHtML

[Q08] 创建普通索引
来源：http://baike.bbcook.cn/Article/details/gccyrsgki.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/govfmswis.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.yfazqb.com/Article/details/gtmtvocom.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/gixooahiy.sHtML

[Q10] 插入单行
来源：http://blog.sjlbkw.cn/Article/details/gievkzbbb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gywbptngs.sHtML

[Q11] 一次插入多行
来源：http://read.share.fktsv.cn/Article/details/gtnrhxadc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.epnwcf.com/Article/details/gnznawupi.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.bbcook.cn/Article/details/geujisvqg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fktsv.cn/Article/details/gtytoiquq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fktsv.cn/Article/details/giatigluo.sHtML

[Q13] 忽略重复插入
来源：http://baike.epnwcf.com/Article/details/gxlhnlbvv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fktsv.cn/Article/details/gzigssadp.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fktsv.cn/Article/details/gcacvloaf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.yfazqb.com/Article/details/gpaelqtew.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.vehdjk.com/Article/details/gwcqeinas.sHtML

[Q15] 查询全部
来源：http://www.share.tarul.cn/Article/details/gmaxuatry.sHtML

SELECT * FROM users;
来源：http://blog.yfazqb.com/Article/details/gsukspapt.sHtML

[Q16] 查询指定列
来源：http://read.share.fktsv.cn/Article/details/govhievsi.sHtML

SELECT id, name FROM users;
来源：http://wap.vehdjk.com/Article/details/gzwysnspl.sHtML

[Q17] 条件查询
来源：http://www.share.fktsv.cn/Article/details/gtzqnjfst.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.bbcook.cn/Article/details/gftkirbyk.sHtML

[Q18] 模糊匹配
来源：http://3g.tarul.cn/Article/details/gnfictrcu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.tarul.cn/Article/details/gkoaddikp.sHtML

[Q19] 范围查询
来源：http://www.m.share.yfazqb.com/Article/details/gslfuxqqq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.epnwcf.com/Article/details/grrajwumm.sHtML

[Q20] IN 列表
来源：http://m.share.vehdjk.com/Article/details/ghoovwzay.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.bbcook.cn/Article/details/gecvyxejj.sHtML

[Q21] 空值判断
来源：http://mobile.epnwcf.com/Article/details/gicrwpdjs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.epnwcf.com/Article/details/gpsbhroyf.sHtML

[Q22] 排序
来源：http://www.m.share.fktsv.cn/Article/details/gctqvjqzi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fktsv.cn/Article/details/gmdzahxqr.sHtML

[Q23] 分页
来源：http://mobile.tarul.cn/Article/details/gwyunvacb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.sjlbkw.cn/Article/details/grsdmsvge.sHtML

[Q24] 去重
来源：http://www.share.sjlbkw.cn/Article/details/gguzbrpan.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.epnwcf.com/Article/details/gxvsgvfhh.sHtML

[Q25] 只取前 N 条
来源：http://3g.bbcook.cn/Article/details/gepmqmwvg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.bbcook.cn/Article/details/gvkfyadhd.sHtML

[Q26] 计数
来源：http://m.share.fktsv.cn/Article/details/gkyogruds.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.vehdjk.com/Article/details/gwdzzoxdi.sHtML

[Q27] 条件计数
来源：http://3g.bbcook.cn/Article/details/gvlgxoycf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/glzialich.sHtML

[Q28] 求和与平均
来源：http://wap.vehdjk.com/Article/details/gjxezxksg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gjfneukty.sHtML

[Q29] 最大最小值
来源：http://wap.tarul.cn/Article/details/gvzjfgyje.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gyguybicu.sHtML

[Q30] 分组统计
来源：http://3g.bbcook.cn/Article/details/gatixxscd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/ghrtwovsr.sHtML

[Q31] 分组后过滤
来源：http://www.blog.yfazqb.com/Article/details/gcydvqmkw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fktsv.cn/Article/details/gupybuqec.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gddisuxht.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/gldifrvzu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.vehdjk.com/Article/details/goknrzjwq.sHtML

[Q33] 多列分组
来源：http://baike.epnwcf.com/Article/details/gcmwnxjvl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.yfazqb.com/Article/details/gebfgrmin.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fktsv.cn/Article/details/gzjqzlqnn.sHtML

SELECT * FROM (
来源：http://www.share.fktsv.cn/Article/details/ggllzbche.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.vehdjk.com/Article/details/ggxjtotut.sHtML

) t WHERE rn = 1;
来源：http://blog.vehdjk.com/Article/details/gdwqrdble.sHtML

[Q35] 内连接
来源：http://blog.yfazqb.com/Article/details/grvjqcpcs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fktsv.cn/Article/details/gprwjobpg.sHtML

[Q36] 左连接
来源：http://www.m.share.vehdjk.com/Article/details/gmvehxfmh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.bbcook.cn/Article/details/guhiphycj.sHtML

[Q37] 右连接
来源：http://www.share.fktsv.cn/Article/details/gzjshafoh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.epnwcf.com/Article/details/gcqdqnkuf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.epnwcf.com/Article/details/gzsndfblw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.tarul.cn/Article/details/gmlovcdwj.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.yfazqb.com/Article/details/gqwftfuuh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.epnwcf.com/Article/details/gydrerurz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.epnwcf.com/Article/details/gvtdsnhfl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbsgxnnd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.yfazqb.com/Article/details/gtxdrugem.sHtML

[Q41] 多表连接
来源：http://m.share.bbcook.cn/Article/details/gqtdncdks.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.sjlbkw.cn/Article/details/gplnmxclk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.tarul.cn/Article/details/gccsonaoh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.yfazqb.com/Article/details/gknqzmnfc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.bbcook.cn/Article/details/gcwiwxhnb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.vehdjk.com/Article/details/gafjhetcm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.bbcook.cn/Article/details/gcqxgqyxv.sHtML

[Q43] 标量子查询
来源：http://www.blog.bbcook.cn/Article/details/gnyiofods.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fktsv.cn/Article/details/gyrqejmpc.sHtML

[Q44] IN 子查询
来源：http://read.share.vehdjk.com/Article/details/gctiohskn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.sjlbkw.cn/Article/details/gndrszvcb.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.yfazqb.com/Article/details/gpkqfdlbf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/gffjgotqk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.epnwcf.com/Article/details/gjruivtbp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.vehdjk.com/Article/details/gpnftklli.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fktsv.cn/Article/details/gfyhvxcib.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.tarul.cn/Article/details/gcyhpjsxx.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.bbcook.cn/Article/details/godmgtrhu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fktsv.cn/Article/details/gdsillboi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.sjlbkw.cn/Article/details/grwrohfyg.sHtML

[Q49] 更新单行
来源：http://3g.sjlbkw.cn/Article/details/gpkgcfvvn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.yfazqb.com/Article/details/gqnivhnvp.sHtML

[Q50] 批量更新
来源：http://3g.epnwcf.com/Article/details/giksworvu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.yfazqb.com/Article/details/gcjbgayuk.sHtML

[Q51] 用子查询更新
来源：http://read.share.bbcook.cn/Article/details/ggapkdrtl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.epnwcf.com/Article/details/gqxunncdm.sHtML

[Q52] 删除指定行
来源：http://mobile.epnwcf.com/Article/details/gswslbwtm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.vehdjk.com/Article/details/gdqcztifw.sHtML

[Q53] 按条件删除
来源：http://www.share.fktsv.cn/Article/details/gblpcozeu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.yfazqb.com/Article/details/ganreuxng.sHtML

[Q54] 清空表
来源：http://baike.sjlbkw.cn/Article/details/gtazkqvvl.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fktsv.cn/Article/details/ginuknxrs.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.sjlbkw.cn/Article/details/ggmiphifz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.epnwcf.com/Article/details/gpqlqgbkc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.tarul.cn/Article/details/gatnzhmny.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.vehdjk.com/Article/details/gncbxvgpl.sHtML

[Q57] 行号
来源：http://www.m.share.vehdjk.com/Article/details/gmeafnqre.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gmdyrfrls.sHtML

[Q58] 累计求和
来源：http://baike.vehdjk.com/Article/details/ggkeispuo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.yfazqb.com/Article/details/gukblnxcf.sHtML

[Q59] 分组内累计
来源：http://blog.epnwcf.com/Article/details/gkhdpjmtz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gnhtusxxj.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.sjlbkw.cn/Article/details/gaklcpiuu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.bbcook.cn/Article/details/gikodkhng.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.bbcook.cn/Article/details/gknvpbjrh.sHtML

[Q61] 移动平均
来源：http://m.share.epnwcf.com/Article/details/gdeisgpga.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gtjvsmusi.sHtML

[Q62] 分组占比
来源：http://www.share.epnwcf.com/Article/details/gnkulrdvh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gcyxaibgs.sHtML

[Q63] 开启事务
来源：http://www.m.share.tarul.cn/Article/details/gizztyxjp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fktsv.cn/Article/details/gppzfrzru.sHtML

[Q64] 提交事务
来源：http://blog.yfazqb.com/Article/details/gvvatxzge.sHtML

COMMIT;
来源：http://mobile.tarul.cn/Article/details/gqtwddmpo.sHtML

[Q65] 回滚事务
来源：http://www.share.yfazqb.com/Article/details/gajfmtpui.sHtML

ROLLBACK;
来源：http://blog.yfazqb.com/Article/details/gqrgypggm.sHtML

[Q66] 行锁查询
来源：http://www.share.yfazqb.com/Article/details/gzymcifgz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.tarul.cn/Article/details/gcfotsiez.sHtML

[Q67] 设置隔离级别
来源：http://blog.bbcook.cn/Article/details/gktcvfohc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.bbcook.cn/Article/details/gdokeahsx.sHtML

[Q68] 保存点
来源：http://read.share.sjlbkw.cn/Article/details/grpkxlccv.sHtML

SAVEPOINT sp1;
来源：http://read.share.yfazqb.com/Article/details/ghupnicno.sHtML

ROLLBACK TO sp1;
来源：http://blog.tarul.cn/Article/details/gzgwewlre.sHtML

[Q69] 查看执行计划
来源：http://www.share.yfazqb.com/Article/details/gxrqkzukz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.epnwcf.com/Article/details/gyldudytv.sHtML

[Q70] 更新统计信息
来源：http://3g.fktsv.cn/Article/details/gehsyylkj.sHtML

ANALYZE TABLE users;
来源：http://m.share.fktsv.cn/Article/details/gsflbtbhy.sHtML

[Q71] 查看建表语句
来源：http://baike.sjlbkw.cn/Article/details/ggmvzbnri.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.vehdjk.com/Article/details/gjpfyhoys.sHtML

[Q72] 查看索引
来源：http://3g.yfazqb.com/Article/details/gajdblqza.sHtML

SHOW INDEX FROM users;
来源：http://baike.yfazqb.com/Article/details/garbwwgfu.sHtML

[Q73] 查看表状态
来源：http://wap.sjlbkw.cn/Article/details/guyzgioom.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.bbcook.cn/Article/details/glwskjara.sHtML

[Q74] 强制使用索引
来源：http://baike.yfazqb.com/Article/details/gddavbdlm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.sjlbkw.cn/Article/details/gvzjedemq.sHtML

[Q75] 日期格式化
来源：http://blog.vehdjk.com/Article/details/gruqtgnzk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gidhhagqu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.vehdjk.com/Article/details/gfwwubegf.sHtML


<!-- 参考信息 -->