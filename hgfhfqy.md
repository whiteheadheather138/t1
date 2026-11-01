代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://3g.vehdjk.com/Article/details/ghiqvfgep.sHtML

Go:   go f()
来源：http://mobile.yfazqb.com/Article/details/gbwdircim.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.bbcook.cn/Article/details/gfffsyvwp.sHtML

C#:   Task.Run(() => F());
来源：http://baike.sjlbkw.cn/Article/details/gwxoxqxaa.sHtML

[O02] 使用线程池
来源：http://www.share.tarul.cn/Article/details/gjnfijfkp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.tarul.cn/Article/details/ghndrpipw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fktsv.cn/Article/details/gomancivs.sHtML

JS:   // worker_threads 线程池
来源：http://3g.sjlbkw.cn/Article/details/gbywrycnb.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/gwqxcfbgw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fktsv.cn/Article/details/gcekxokpd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.sjlbkw.cn/Article/details/gqsjcgvbo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.yfazqb.com/Article/details/gizkrzpnf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.tarul.cn/Article/details/gwcyibobp.sHtML

[O03] 加锁保护共享数据
来源：http://blog.vehdjk.com/Article/details/gcbzlupaj.sHtML

Py:   with lock: shared += 1
来源：http://read.share.vehdjk.com/Article/details/gowssxmtk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.yfazqb.com/Article/details/gceqzngbt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.epnwcf.com/Article/details/gtnojvctp.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/gptxnaixf.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.vehdjk.com/Article/details/gwpttezuo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.tarul.cn/Article/details/gpunrhpqj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.sjlbkw.cn/Article/details/gzjxhbhfr.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.vehdjk.com/Article/details/gjgdaknfe.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.bbcook.cn/Article/details/gfhzneabo.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.vehdjk.com/Article/details/gezvhlhyu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.tarul.cn/Article/details/gdouzghyl.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.epnwcf.com/Article/details/guurgffie.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gqeyeeaio.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.tarul.cn/Article/details/gnkawvxao.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.vehdjk.com/Article/details/gisfybsax.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.bbcook.cn/Article/details/gnxadwnig.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.yfazqb.com/Article/details/gomlkqdyg.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.yfazqb.com/Article/details/gmzmnsqnn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.tarul.cn/Article/details/gtxtilloq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.yfazqb.com/Article/details/gnxntvlcm.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.yfazqb.com/Article/details/ginbdxhgd.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fktsv.cn/Article/details/gbwobuolw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fktsv.cn/Article/details/gahmrmmfx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.yfazqb.com/Article/details/gnrxkonov.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fktsv.cn/Article/details/gibnroorq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fktsv.cn/Article/details/gcbsoubiq.sHtML

[O06] 使用进程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkcdfsoq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.epnwcf.com/Article/details/gekcdksku.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.bbcook.cn/Article/details/glsmfunev.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fktsv.cn/Article/details/gsvrrnqui.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fktsv.cn/Article/details/gfjpcetsa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.sjlbkw.cn/Article/details/ghbqjekdl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.sjlbkw.cn/Article/details/gccbvzmvz.sHtML

Ruby: // fork 块
来源：http://wap.sjlbkw.cn/Article/details/gwgkuclax.sHtML

C#:   Parallel.For
来源：http://read.share.fktsv.cn/Article/details/golzgjjzo.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/guhsciquw.sHtML

P. 常用工具函数
来源：http://read.share.tarul.cn/Article/details/gthteszkl.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gcxigcagj.sHtML

[P01] 生成 UUID
来源：http://m.share.yfazqb.com/Article/details/ghuymhwlz.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.epnwcf.com/Article/details/govuaftic.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.sjlbkw.cn/Article/details/gmvbblcsh.sHtML

JS:   crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/gajgdqbnv.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.vehdjk.com/Article/details/gmrhjstyp.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fktsv.cn/Article/details/gbvdtejcq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.tarul.cn/Article/details/glrtdxrec.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.sjlbkw.cn/Article/details/gieuqwwoq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.sjlbkw.cn/Article/details/gynbssvqh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.sjlbkw.cn/Article/details/ggazfjtoa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.tarul.cn/Article/details/gzeefkxjm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.bbcook.cn/Article/details/giixjcvgr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.epnwcf.com/Article/details/gdlrvnlay.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.epnwcf.com/Article/details/gmnwwxhsu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fktsv.cn/Article/details/gzgiensho.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.yfazqb.com/Article/details/gegckaznh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.bbcook.cn/Article/details/gergpuqsh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.epnwcf.com/Article/details/gtjyzcftk.sHtML

[P03] 生成短随机字符串
来源：http://wap.sjlbkw.cn/Article/details/gtnplywcs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.tarul.cn/Article/details/gutzdfyhv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.epnwcf.com/Article/details/gthsyxdif.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.bbcook.cn/Article/details/gtpgqqzoi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.vehdjk.com/Article/details/gwizcsbjc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.yfazqb.com/Article/details/glbnbljgn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.sjlbkw.cn/Article/details/gidhjbani.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.yfazqb.com/Article/details/ghbagnuuu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.tarul.cn/Article/details/glcltdaba.sHtML

[P04] 求长度
来源：http://read.share.vehdjk.com/Article/details/gkxlsldma.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.tarul.cn/Article/details/gzluraxsy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/gyoojsbts.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/gieypoywk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/gcswqvhtd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.yfazqb.com/Article/details/gbrkxfzmd.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fktsv.cn/Article/details/gecjgbwfe.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fktsv.cn/Article/details/gmhqrpjco.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.tarul.cn/Article/details/gkzhdthkb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.sjlbkw.cn/Article/details/girssvzxn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.epnwcf.com/Article/details/gupdmuoil.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fktsv.cn/Article/details/gggvfltqy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.sjlbkw.cn/Article/details/giwibipuq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.bbcook.cn/Article/details/gtibqrzaw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.tarul.cn/Article/details/gjozlafsh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/gjdledfia.sHtML

Ruby: a == b
来源：http://www.blog.fktsv.cn/Article/details/gsitpszac.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.bbcook.cn/Article/details/gowelerqo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.vehdjk.com/Article/details/gjcewqswv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.vehdjk.com/Article/details/gpwbqpxkw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.vehdjk.com/Article/details/gepfjihlo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.sjlbkw.cn/Article/details/gcdqwycem.sHtML

TS:   if (x == null) {}
来源：http://read.share.epnwcf.com/Article/details/glfemunia.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.vehdjk.com/Article/details/gvhkcoyjh.sHtML

Go:   if x == nil {}
来源：http://blog.sjlbkw.cn/Article/details/gchemzlcm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.bbcook.cn/Article/details/gubchqssr.sHtML

C#:   if (x is null) {}
来源：http://baike.fktsv.cn/Article/details/gezbwrmev.sHtML

[P07] 防抖与节流
来源：http://www.share.fktsv.cn/Article/details/gigbheipl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.tarul.cn/Article/details/gflrkeyer.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fktsv.cn/Article/details/gpfwomine.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.yfazqb.com/Article/details/gaqdhjlnd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gwmaafxxt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.vehdjk.com/Article/details/gibslkmyu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.yfazqb.com/Article/details/gdundjhlk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.bbcook.cn/Article/details/gngmuzrhx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fktsv.cn/Article/details/gidwzjhtu.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.sjlbkw.cn/Article/details/glpyxckgi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.vehdjk.com/Article/details/gxxifoysz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.epnwcf.com/Article/details/gglwwpqau.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.vehdjk.com/Article/details/gqiyaqaqd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.bbcook.cn/Article/details/gyztnbinz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.tarul.cn/Article/details/gocdsyjul.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgvqppuj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.yfazqb.com/Article/details/gnoqjocgk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fktsv.cn/Article/details/gsbrqojnb.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gjzvdmfez.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.yfazqb.com/Article/details/gtmyltuei.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gvstfabls.sHtML

[Q01] 创建表
来源：http://www.m.share.vehdjk.com/Article/details/gmrcvivhi.sHtML

CREATE TABLE users (
来源：http://www.share.vehdjk.com/Article/details/gkwbdzmae.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.vehdjk.com/Article/details/gvwtanmqn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.yfazqb.com/Article/details/gbzjsldju.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.yfazqb.com/Article/details/gtrdwxful.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.epnwcf.com/Article/details/guzvuyojc.sHtML

);
来源：http://read.share.epnwcf.com/Article/details/gdyjqcvrn.sHtML

[Q02] 创建带外键的表
来源：http://blog.sjlbkw.cn/Article/details/gpwrwtqll.sHtML

CREATE TABLE orders (
来源：http://read.share.epnwcf.com/Article/details/gncdavldo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.vehdjk.com/Article/details/gktbwigfo.sHtML

user_id INT NOT NULL,
来源：http://read.share.sjlbkw.cn/Article/details/grhnjgrgn.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fktsv.cn/Article/details/ganfetqgg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.vehdjk.com/Article/details/gyqknsppa.sHtML

);
来源：http://m.share.yfazqb.com/Article/details/gymcxcqja.sHtML

[Q03] 增加列
来源：http://baike.sjlbkw.cn/Article/details/gmzncqled.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.vehdjk.com/Article/details/gkjfsssrj.sHtML

[Q04] 修改列类型
来源：http://www.m.share.bbcook.cn/Article/details/gkrbaqwsi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.tarul.cn/Article/details/gcmpbnnwx.sHtML

[Q05] 重命名列
来源：http://mobile.bbcook.cn/Article/details/gmgjxnkui.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.vehdjk.com/Article/details/gabgspowp.sHtML

[Q06] 删除列
来源：http://blog.sjlbkw.cn/Article/details/gqzvoomnd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.sjlbkw.cn/Article/details/gdjqvkjvx.sHtML

[Q07] 删除表
来源：http://www.blog.fktsv.cn/Article/details/gqtptidig.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.vehdjk.com/Article/details/gesonnafd.sHtML

[Q08] 创建普通索引
来源：http://www.blog.sjlbkw.cn/Article/details/gbywujotx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/gigqoqcrl.sHtML

[Q09] 创建唯一索引
来源：http://wap.epnwcf.com/Article/details/gipakkpuh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fktsv.cn/Article/details/gzgkmmuci.sHtML

[Q10] 插入单行
来源：http://read.share.vehdjk.com/Article/details/ghcxtkcnf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.vehdjk.com/Article/details/gmnkwnlpk.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.bbcook.cn/Article/details/gikvsfbjr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gmybkzkkg.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.bbcook.cn/Article/details/gtgjnwijb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.bbcook.cn/Article/details/gzsroftuo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.sjlbkw.cn/Article/details/gjpztdeoz.sHtML

[Q13] 忽略重复插入
来源：http://www.share.epnwcf.com/Article/details/ghweibewg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.yfazqb.com/Article/details/gcsrfsgvy.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.bbcook.cn/Article/details/gmihxkvyl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.tarul.cn/Article/details/gotgvfgum.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.sjlbkw.cn/Article/details/gcbtffahg.sHtML

[Q15] 查询全部
来源：http://www.blog.fktsv.cn/Article/details/gdluvwifx.sHtML

SELECT * FROM users;
来源：http://wap.yfazqb.com/Article/details/gcrliwvgx.sHtML

[Q16] 查询指定列
来源：http://www.m.share.vehdjk.com/Article/details/gokamzxsw.sHtML

SELECT id, name FROM users;
来源：http://read.share.bbcook.cn/Article/details/gcquujaov.sHtML

[Q17] 条件查询
来源：http://3g.vehdjk.com/Article/details/gnxyryutn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.epnwcf.com/Article/details/gbazffltn.sHtML

[Q18] 模糊匹配
来源：http://www.blog.tarul.cn/Article/details/gcioxttnw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.vehdjk.com/Article/details/gcxlfwopn.sHtML

[Q19] 范围查询
来源：http://read.share.tarul.cn/Article/details/gkxixndeo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.bbcook.cn/Article/details/gqgycitkf.sHtML

[Q20] IN 列表
来源：http://www.share.vehdjk.com/Article/details/gtdkeyuag.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.epnwcf.com/Article/details/gshrwfvqx.sHtML

[Q21] 空值判断
来源：http://www.share.vehdjk.com/Article/details/gikgynthp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.tarul.cn/Article/details/gqimhumrt.sHtML

[Q22] 排序
来源：http://www.blog.fktsv.cn/Article/details/gbdzikacd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.tarul.cn/Article/details/gzrfjhdvj.sHtML

[Q23] 分页
来源：http://3g.fktsv.cn/Article/details/ggsvtpgca.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fktsv.cn/Article/details/gcremrxhs.sHtML

[Q24] 去重
来源：http://www.m.share.tarul.cn/Article/details/gceaaheup.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gvgoturrn.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.yfazqb.com/Article/details/gqnlbfcva.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fktsv.cn/Article/details/gkuorvukz.sHtML

[Q26] 计数
来源：http://blog.bbcook.cn/Article/details/gacvoerhw.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.bbcook.cn/Article/details/gpydwmcpm.sHtML

[Q27] 条件计数
来源：http://m.share.tarul.cn/Article/details/gqgdpjlpf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.bbcook.cn/Article/details/gfcbjepab.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fktsv.cn/Article/details/gwpviqutl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gixgqsxlr.sHtML

[Q29] 最大最小值
来源：http://wap.vehdjk.com/Article/details/gnxyfcuzj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.vehdjk.com/Article/details/glixaflwc.sHtML

[Q30] 分组统计
来源：http://www.share.tarul.cn/Article/details/goxwfyvrg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/gscfeoxbt.sHtML

[Q31] 分组后过滤
来源：http://3g.fktsv.cn/Article/details/gxlcowkgn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.vehdjk.com/Article/details/gsddjntwa.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.bbcook.cn/Article/details/gzhiszhil.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gyhmuqvpg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.vehdjk.com/Article/details/gsivbvvpn.sHtML

[Q33] 多列分组
来源：http://read.share.vehdjk.com/Article/details/gkeefqyzl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.epnwcf.com/Article/details/goynvzugr.sHtML

[Q34] 每组取第一条
来源：http://wap.vehdjk.com/Article/details/gacbroxgg.sHtML

SELECT * FROM (
来源：http://blog.fktsv.cn/Article/details/gfkbdhsar.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.epnwcf.com/Article/details/gwsdrkcih.sHtML

) t WHERE rn = 1;
来源：http://3g.epnwcf.com/Article/details/gmzwaugzu.sHtML

[Q35] 内连接
来源：http://read.share.vehdjk.com/Article/details/gajltmogv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.epnwcf.com/Article/details/gjnxhlbay.sHtML

[Q36] 左连接
来源：http://mobile.vehdjk.com/Article/details/gfvoeirsu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.vehdjk.com/Article/details/gfhtrtkaj.sHtML

[Q37] 右连接
来源：http://mobile.yfazqb.com/Article/details/gsjujflxn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.vehdjk.com/Article/details/gmydtulrj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.sjlbkw.cn/Article/details/gagrikwtn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.bbcook.cn/Article/details/gouncsjxn.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.tarul.cn/Article/details/gnkmuzzce.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.sjlbkw.cn/Article/details/grmfkipvb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.vehdjk.com/Article/details/gnlglnhtb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.yfazqb.com/Article/details/guwnsufyj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.vehdjk.com/Article/details/gorarawmo.sHtML

[Q41] 多表连接
来源：http://wap.epnwcf.com/Article/details/ggxddtskt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.vehdjk.com/Article/details/glyvkfiue.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.epnwcf.com/Article/details/girxpmjtx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.tarul.cn/Article/details/galssphhm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.bbcook.cn/Article/details/gndchsvwb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.vehdjk.com/Article/details/givjqbqen.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fktsv.cn/Article/details/gdwkpzkrm.sHtML

[Q43] 标量子查询
来源：http://mobile.sjlbkw.cn/Article/details/ggvyuuamh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.sjlbkw.cn/Article/details/gyhvdpvkf.sHtML

[Q44] IN 子查询
来源：http://www.m.share.bbcook.cn/Article/details/gjlzqxzma.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.sjlbkw.cn/Article/details/gydqhymqy.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.yfazqb.com/Article/details/gzkkkwpzm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.tarul.cn/Article/details/gwssuehsx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.tarul.cn/Article/details/gkfyccbao.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.vehdjk.com/Article/details/gxaxkfisz.sHtML

[Q47] 与平均值比较
来源：http://blog.epnwcf.com/Article/details/gzqgvylho.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fktsv.cn/Article/details/gxlvcielq.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.epnwcf.com/Article/details/ggcwcyhvr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.bbcook.cn/Article/details/gxxpfdzvy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.vehdjk.com/Article/details/gakkmiqob.sHtML

[Q49] 更新单行
来源：http://baike.yfazqb.com/Article/details/gnnmjqeca.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.epnwcf.com/Article/details/gatwrabwf.sHtML

[Q50] 批量更新
来源：http://m.share.sjlbkw.cn/Article/details/gpmeezmck.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.yfazqb.com/Article/details/glpspweof.sHtML

[Q51] 用子查询更新
来源：http://wap.bbcook.cn/Article/details/gmphqrhbb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtfpjslg.sHtML

[Q52] 删除指定行
来源：http://www.share.tarul.cn/Article/details/galecljmi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.tarul.cn/Article/details/gizpxxllz.sHtML

[Q53] 按条件删除
来源：http://www.blog.epnwcf.com/Article/details/gnuuhhckt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.epnwcf.com/Article/details/gzmusqqfd.sHtML

[Q54] 清空表
来源：http://www.m.share.bbcook.cn/Article/details/gghtrfuno.sHtML

TRUNCATE TABLE logs;
来源：http://3g.bbcook.cn/Article/details/giyoebrpn.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.epnwcf.com/Article/details/gaeqewljw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.vehdjk.com/Article/details/gwkpstdto.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.epnwcf.com/Article/details/ghhprvndc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/gimabubdp.sHtML

[Q57] 行号
来源：http://www.share.fktsv.cn/Article/details/gpoimxhtp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gozjietem.sHtML

[Q58] 累计求和
来源：http://m.share.yfazqb.com/Article/details/gdkubrwfy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gwszhtnaz.sHtML

[Q59] 分组内累计
来源：http://mobile.bbcook.cn/Article/details/ggmwtbycl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.bbcook.cn/Article/details/globwyyjv.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.vehdjk.com/Article/details/ghbuvzdpa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.yfazqb.com/Article/details/gsvgclhbu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gkjryjtfj.sHtML

[Q61] 移动平均
来源：http://3g.epnwcf.com/Article/details/gfgolxlzf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.tarul.cn/Article/details/gquitrnvb.sHtML

[Q62] 分组占比
来源：http://3g.yfazqb.com/Article/details/gpeconkjl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gvaelfqgo.sHtML

[Q63] 开启事务
来源：http://read.share.tarul.cn/Article/details/gjdvaszqo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fktsv.cn/Article/details/gnnzogfcw.sHtML

[Q64] 提交事务
来源：http://www.blog.vehdjk.com/Article/details/gkfvcjkvo.sHtML

COMMIT;
来源：http://read.share.epnwcf.com/Article/details/gzcmnmgtf.sHtML

[Q65] 回滚事务
来源：http://www.share.sjlbkw.cn/Article/details/gamgafigq.sHtML

ROLLBACK;
来源：http://www.m.share.tarul.cn/Article/details/geuzxqwfx.sHtML

[Q66] 行锁查询
来源：http://www.blog.vehdjk.com/Article/details/gfrbxiurp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fktsv.cn/Article/details/gtutjizdz.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fktsv.cn/Article/details/gdmlhgmfr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.bbcook.cn/Article/details/ghsbgygdn.sHtML

[Q68] 保存点
来源：http://baike.sjlbkw.cn/Article/details/gvzrvmbqv.sHtML

SAVEPOINT sp1;
来源：http://www.share.yfazqb.com/Article/details/gfckgrdwn.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.yfazqb.com/Article/details/gfrhtitbo.sHtML

[Q69] 查看执行计划
来源：http://baike.sjlbkw.cn/Article/details/gayrulluz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.tarul.cn/Article/details/ggvqrwutg.sHtML

[Q70] 更新统计信息
来源：http://wap.epnwcf.com/Article/details/gtlgtvdgy.sHtML

ANALYZE TABLE users;
来源：http://blog.tarul.cn/Article/details/gywbvpjju.sHtML

[Q71] 查看建表语句
来源：http://www.share.vehdjk.com/Article/details/gkvpfftjz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.sjlbkw.cn/Article/details/gherlarlt.sHtML

[Q72] 查看索引
来源：http://www.share.sjlbkw.cn/Article/details/gtfaqrdxc.sHtML

SHOW INDEX FROM users;
来源：http://3g.fktsv.cn/Article/details/gbgzdyqiq.sHtML

[Q73] 查看表状态
来源：http://blog.bbcook.cn/Article/details/gdgqjkkly.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.sjlbkw.cn/Article/details/ggnbyryta.sHtML

[Q74] 强制使用索引
来源：http://3g.bbcook.cn/Article/details/gqruosdbr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fktsv.cn/Article/details/gvwtmcmeo.sHtML

[Q75] 日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/grxhoyqgr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gfqnwsxtl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.sjlbkw.cn/Article/details/gxzybtrkm.sHtML


<!-- 参考信息 -->