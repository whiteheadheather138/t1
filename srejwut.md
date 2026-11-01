代发 wailian999

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gbfjdclca.sHtML

O. 并发与异步
来源：http://3g.epnwcf.com/Article/details/gbipubwff.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gegpcekyq.sHtML

[O01] 启动一个线程
来源：http://blog.vehdjk.com/Article/details/gweqfbnfn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fktsv.cn/Article/details/gnmyumhxi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.bbcook.cn/Article/details/gdmdmwyfc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.vehdjk.com/Article/details/gcrulewgm.sHtML

TS:   // 同 JS
来源：http://www.m.share.tarul.cn/Article/details/gouhmuwlq.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.yfazqb.com/Article/details/grnwxytll.sHtML

Go:   go f()
来源：http://www.share.bbcook.cn/Article/details/gtfcourcu.sHtML

Ruby: Thread.new { f }
来源：http://baike.epnwcf.com/Article/details/gjwcukfsd.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.tarul.cn/Article/details/gafernsli.sHtML

[O02] 使用线程池
来源：http://3g.tarul.cn/Article/details/gqnudoubu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.tarul.cn/Article/details/gugkgcnhb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.bbcook.cn/Article/details/gdfpgkdzh.sHtML

JS:   // worker_threads 线程池
来源：http://3g.sjlbkw.cn/Article/details/gnyiqrnkc.sHtML

TS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/gmjothzfn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fktsv.cn/Article/details/gnlztowrt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.epnwcf.com/Article/details/grpfbtikd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.vehdjk.com/Article/details/glhkpsnzl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.yfazqb.com/Article/details/gthganebg.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.yfazqb.com/Article/details/gmckbovqt.sHtML

Py:   with lock: shared += 1
来源：http://read.share.epnwcf.com/Article/details/gfhpqxuuh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.vehdjk.com/Article/details/gnzcxhwlk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.tarul.cn/Article/details/grszargzl.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/geykjyfla.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.bbcook.cn/Article/details/gfjciqzgg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.bbcook.cn/Article/details/gyqyuluhf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.yfazqb.com/Article/details/gzoxeskjb.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.epnwcf.com/Article/details/ggfbrmqoq.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.sjlbkw.cn/Article/details/gjjoiajqz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.epnwcf.com/Article/details/gigawzkjg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.epnwcf.com/Article/details/girgvvklb.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.vehdjk.com/Article/details/gmpgaaryz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.tarul.cn/Article/details/goktoimie.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fktsv.cn/Article/details/gjarjyzff.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.vehdjk.com/Article/details/gjjbeluhs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.epnwcf.com/Article/details/gziagcpby.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.yfazqb.com/Article/details/guqkpynmg.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.bbcook.cn/Article/details/grlnmcdll.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggigrafol.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.sjlbkw.cn/Article/details/gnrxkvyds.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.yfazqb.com/Article/details/gykqulrnb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gnheydufl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.bbcook.cn/Article/details/ghaztwgka.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.sjlbkw.cn/Article/details/geictotfy.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.epnwcf.com/Article/details/gsuxxhcxz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.vehdjk.com/Article/details/guvoagaix.sHtML

[O06] 使用进程池
来源：http://wap.sjlbkw.cn/Article/details/goqcmcbut.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.bbcook.cn/Article/details/gzrwwzdjx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fktsv.cn/Article/details/gxmmlbpbq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.epnwcf.com/Article/details/gbokijqgy.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fktsv.cn/Article/details/gkfaneayg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.yfazqb.com/Article/details/glcbtuwsu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.bbcook.cn/Article/details/ggbslgkot.sHtML

Ruby: // fork 块
来源：http://m.share.tarul.cn/Article/details/gxkvffjsa.sHtML

C#:   Parallel.For
来源：http://blog.fktsv.cn/Article/details/grednwdxj.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gtciqmoaa.sHtML

P. 常用工具函数
来源：http://www.blog.fktsv.cn/Article/details/gecqtroof.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gikxpdavg.sHtML

[P01] 生成 UUID
来源：http://baike.tarul.cn/Article/details/gqwhibfwk.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.yfazqb.com/Article/details/gvgybomvw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fktsv.cn/Article/details/gealdeeyw.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gemrqiysh.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/gxuecbpkg.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.vehdjk.com/Article/details/ghsyxlybw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fktsv.cn/Article/details/gwoxxfmyl.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fktsv.cn/Article/details/gcbfsrfrj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.epnwcf.com/Article/details/gsktrrldf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.bbcook.cn/Article/details/gyrpwiwtk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fktsv.cn/Article/details/gxkoinrid.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.yfazqb.com/Article/details/gwsysjqpf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.sjlbkw.cn/Article/details/ggctlzenf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.vehdjk.com/Article/details/gbgstblph.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fktsv.cn/Article/details/gtwiphyzh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.tarul.cn/Article/details/gvqmkvbcu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.tarul.cn/Article/details/gqxtlessy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.bbcook.cn/Article/details/gwbjkqhzz.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.yfazqb.com/Article/details/gildilkyl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.epnwcf.com/Article/details/gwldfssrg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fktsv.cn/Article/details/gkzjoilxy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fktsv.cn/Article/details/gkjthcjtn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.tarul.cn/Article/details/gcvepgghc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.epnwcf.com/Article/details/gbdtvvhii.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.sjlbkw.cn/Article/details/gmkwjdxwf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.epnwcf.com/Article/details/gbkzkcsap.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.bbcook.cn/Article/details/goqyeafbp.sHtML

[P04] 求长度
来源：http://3g.sjlbkw.cn/Article/details/gqmffhsch.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.sjlbkw.cn/Article/details/glhnuiquw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gomaxqwrl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.yfazqb.com/Article/details/gisdlbrbs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fktsv.cn/Article/details/gwxdnksuw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.tarul.cn/Article/details/gptsnnhbw.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.epnwcf.com/Article/details/gbxbgrreq.sHtML

Ruby: x.length;  x.size
来源：http://baike.bbcook.cn/Article/details/gggibdgfp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.yfazqb.com/Article/details/grgbmlpkb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.vehdjk.com/Article/details/gtzrbdyar.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.sjlbkw.cn/Article/details/gxfpjbbfm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.sjlbkw.cn/Article/details/gbgrzfrrc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.tarul.cn/Article/details/gbdddkeug.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.bbcook.cn/Article/details/gjgqjnxmm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.vehdjk.com/Article/details/ghhkesmzj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.tarul.cn/Article/details/gdkfejwga.sHtML

Ruby: a == b
来源：http://3g.bbcook.cn/Article/details/gmtahtwta.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.vehdjk.com/Article/details/gikozsgvt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.epnwcf.com/Article/details/gahbhjtet.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.bbcook.cn/Article/details/gcdjfqset.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.vehdjk.com/Article/details/gnnfvjmui.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.tarul.cn/Article/details/gyhlkyowj.sHtML

TS:   if (x == null) {}
来源：http://www.blog.bbcook.cn/Article/details/gyvdzukqh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.sjlbkw.cn/Article/details/grybunbsi.sHtML

Go:   if x == nil {}
来源：http://www.m.share.yfazqb.com/Article/details/gxdtgoyii.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fktsv.cn/Article/details/gfdpscxql.sHtML

C#:   if (x is null) {}
来源：http://m.share.bbcook.cn/Article/details/gbenfedsp.sHtML

[P07] 防抖与节流
来源：http://m.share.epnwcf.com/Article/details/gmsknlrzh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.epnwcf.com/Article/details/gldwqflfj.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.epnwcf.com/Article/details/gwcdgzjzy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/geicattcz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fktsv.cn/Article/details/gaspbiwax.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.tarul.cn/Article/details/gbdgmgvbo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.bbcook.cn/Article/details/grvenrboh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.tarul.cn/Article/details/gmvmskgdf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.epnwcf.com/Article/details/gqkguhkow.sHtML

[P08] 处理浮点精度问题
来源：http://3g.tarul.cn/Article/details/ghiajxuaf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.epnwcf.com/Article/details/goqwukvma.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.tarul.cn/Article/details/ghwuapytb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.tarul.cn/Article/details/gjlpvultd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.epnwcf.com/Article/details/galzpwjhm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.tarul.cn/Article/details/gxzcszvlp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.sjlbkw.cn/Article/details/gkxezmcxa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.sjlbkw.cn/Article/details/gpolkbqox.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fktsv.cn/Article/details/geuivphun.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ggpdqtmtq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.yfazqb.com/Article/details/ggrencbhs.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gtdulneow.sHtML

[Q01] 创建表
来源：http://www.blog.sjlbkw.cn/Article/details/gttsppjxy.sHtML

CREATE TABLE users (
来源：http://3g.bbcook.cn/Article/details/gzdxyznbw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.sjlbkw.cn/Article/details/gpeqkurnq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.tarul.cn/Article/details/gfqkgnxoh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.vehdjk.com/Article/details/gknqfoiqw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.yfazqb.com/Article/details/goakvwdun.sHtML

);
来源：http://3g.sjlbkw.cn/Article/details/gsujjtrcb.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fktsv.cn/Article/details/gelhkerqa.sHtML

CREATE TABLE orders (
来源：http://3g.tarul.cn/Article/details/gilgdulam.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.epnwcf.com/Article/details/gsnkjamtq.sHtML

user_id INT NOT NULL,
来源：http://mobile.bbcook.cn/Article/details/gpjawojsx.sHtML

amount DECIMAL(10, 2),
来源：http://blog.epnwcf.com/Article/details/gidlgqblk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.tarul.cn/Article/details/grjqfhvws.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gaduomhqk.sHtML

[Q03] 增加列
来源：http://www.m.share.bbcook.cn/Article/details/gswwrxfoo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.bbcook.cn/Article/details/gdpiihqjq.sHtML

[Q04] 修改列类型
来源：http://read.share.fktsv.cn/Article/details/gchdhwrog.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.yfazqb.com/Article/details/gsocxdvqn.sHtML

[Q05] 重命名列
来源：http://wap.bbcook.cn/Article/details/gvbtejtwa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.bbcook.cn/Article/details/gccbxqbli.sHtML

[Q06] 删除列
来源：http://baike.fktsv.cn/Article/details/gppsktnch.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.bbcook.cn/Article/details/gfivgqdnj.sHtML

[Q07] 删除表
来源：http://3g.epnwcf.com/Article/details/gixtdmqqf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.tarul.cn/Article/details/gerxytzra.sHtML

[Q08] 创建普通索引
来源：http://3g.epnwcf.com/Article/details/gkpanuxbb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.sjlbkw.cn/Article/details/gxcrsadpu.sHtML

[Q09] 创建唯一索引
来源：http://blog.sjlbkw.cn/Article/details/gmssdzonf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.epnwcf.com/Article/details/gywkwrjin.sHtML

[Q10] 插入单行
来源：http://www.blog.epnwcf.com/Article/details/gqcpjlanq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.vehdjk.com/Article/details/gxsychjwi.sHtML

[Q11] 一次插入多行
来源：http://m.share.epnwcf.com/Article/details/ghlqkhdrc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.vehdjk.com/Article/details/ggdyxlyhb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.sjlbkw.cn/Article/details/gyjfhqfix.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.bbcook.cn/Article/details/gmjmqhalb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fktsv.cn/Article/details/geygrandr.sHtML

[Q13] 忽略重复插入
来源：http://blog.yfazqb.com/Article/details/gbbeltikb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.tarul.cn/Article/details/gaiftkdjj.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.yfazqb.com/Article/details/gbharonyq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.vehdjk.com/Article/details/gcocvgwmx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.bbcook.cn/Article/details/gayxyfwrc.sHtML

[Q15] 查询全部
来源：http://baike.yfazqb.com/Article/details/gfavojvgv.sHtML

SELECT * FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gcxmxywjy.sHtML

[Q16] 查询指定列
来源：http://m.share.vehdjk.com/Article/details/gfghgwabb.sHtML

SELECT id, name FROM users;
来源：http://baike.tarul.cn/Article/details/gqpjrwnar.sHtML

[Q17] 条件查询
来源：http://3g.vehdjk.com/Article/details/gjifmxbtg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fktsv.cn/Article/details/gsscshtgf.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.vehdjk.com/Article/details/ghylnggfw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.vehdjk.com/Article/details/ggxhqwfga.sHtML

[Q19] 范围查询
来源：http://blog.sjlbkw.cn/Article/details/grrwmnfvr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.yfazqb.com/Article/details/gyqcqbkyn.sHtML

[Q20] IN 列表
来源：http://www.blog.fktsv.cn/Article/details/gzfapdoip.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.yfazqb.com/Article/details/gktjovona.sHtML

[Q21] 空值判断
来源：http://blog.yfazqb.com/Article/details/ghvkuxamx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.bbcook.cn/Article/details/gaowuyufc.sHtML

[Q22] 排序
来源：http://www.m.share.epnwcf.com/Article/details/gvxnslnca.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.vehdjk.com/Article/details/gyhkgiqnh.sHtML

[Q23] 分页
来源：http://mobile.bbcook.cn/Article/details/gghenbvfs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfutdykz.sHtML

[Q24] 去重
来源：http://blog.bbcook.cn/Article/details/gkszyhdwv.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.bbcook.cn/Article/details/goxdjsomz.sHtML

[Q25] 只取前 N 条
来源：http://www.share.tarul.cn/Article/details/ganpuhfpu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.bbcook.cn/Article/details/glfrthfjp.sHtML

[Q26] 计数
来源：http://m.share.tarul.cn/Article/details/gqvuvmkow.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gfmxamawb.sHtML

[Q27] 条件计数
来源：http://mobile.tarul.cn/Article/details/gqmlxbtwo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gdqoyvyyz.sHtML

[Q28] 求和与平均
来源：http://baike.yfazqb.com/Article/details/gxibvewkq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fktsv.cn/Article/details/ghzlbettr.sHtML

[Q29] 最大最小值
来源：http://baike.yfazqb.com/Article/details/gzxislbih.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.tarul.cn/Article/details/ggkzcyixh.sHtML

[Q30] 分组统计
来源：http://mobile.bbcook.cn/Article/details/gprznddhl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fktsv.cn/Article/details/gsiqjbvme.sHtML

[Q31] 分组后过滤
来源：http://mobile.sjlbkw.cn/Article/details/gtltprjcx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.bbcook.cn/Article/details/gjqoipknc.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gnocjbdzn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/gdvyhggow.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.epnwcf.com/Article/details/gokgsiwie.sHtML

[Q33] 多列分组
来源：http://blog.epnwcf.com/Article/details/gjkittmya.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.tarul.cn/Article/details/gmgavgnpe.sHtML

[Q34] 每组取第一条
来源：http://www.share.epnwcf.com/Article/details/gdjracghn.sHtML

SELECT * FROM (
来源：http://m.share.tarul.cn/Article/details/gnymuenlq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.bbcook.cn/Article/details/gnxrzbvxq.sHtML

) t WHERE rn = 1;
来源：http://read.share.vehdjk.com/Article/details/gvrrliysd.sHtML

[Q35] 内连接
来源：http://3g.epnwcf.com/Article/details/gtughanhb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.vehdjk.com/Article/details/gqehcmpvq.sHtML

[Q36] 左连接
来源：http://www.blog.sjlbkw.cn/Article/details/gtgzobjmc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.vehdjk.com/Article/details/ghhnjpmdw.sHtML

[Q37] 右连接
来源：http://www.blog.tarul.cn/Article/details/gsxbjwpvk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fktsv.cn/Article/details/gtjbysjrx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.vehdjk.com/Article/details/gvzanttpl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fktsv.cn/Article/details/gxmhlucaw.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fktsv.cn/Article/details/gimzblahu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fktsv.cn/Article/details/gjovkkipl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.tarul.cn/Article/details/gcbjtsxvd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.sjlbkw.cn/Article/details/gekwcchuq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.vehdjk.com/Article/details/grvvpvekm.sHtML

[Q41] 多表连接
来源：http://read.share.bbcook.cn/Article/details/ggjrhienw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.tarul.cn/Article/details/ghouuuuti.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fktsv.cn/Article/details/gxepkawxy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.yfazqb.com/Article/details/gcycyxvee.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.epnwcf.com/Article/details/gukivdxpw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fktsv.cn/Article/details/gtkuhqsvm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.epnwcf.com/Article/details/givubjtlm.sHtML

[Q43] 标量子查询
来源：http://www.blog.bbcook.cn/Article/details/gjbutcvlj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.sjlbkw.cn/Article/details/ghjacaekq.sHtML

[Q44] IN 子查询
来源：http://baike.fktsv.cn/Article/details/gdigjigdp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.sjlbkw.cn/Article/details/gwwsqwaho.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fktsv.cn/Article/details/gujgnrdue.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.epnwcf.com/Article/details/gutcnjues.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.yfazqb.com/Article/details/ggygzoxje.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.tarul.cn/Article/details/gzbvqesds.sHtML

[Q47] 与平均值比较
来源：http://read.share.sjlbkw.cn/Article/details/gaycqwjwy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fktsv.cn/Article/details/gzlvwpuyq.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.vehdjk.com/Article/details/gkkftxcog.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.yfazqb.com/Article/details/gtkjkigws.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.epnwcf.com/Article/details/gkeudaytl.sHtML

[Q49] 更新单行
来源：http://mobile.vehdjk.com/Article/details/gerzgpzyb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.sjlbkw.cn/Article/details/gfnpwheya.sHtML

[Q50] 批量更新
来源：http://mobile.bbcook.cn/Article/details/gtlmnykyx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.tarul.cn/Article/details/gzbszoogl.sHtML

[Q51] 用子查询更新
来源：http://mobile.sjlbkw.cn/Article/details/ggrftxdaz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.bbcook.cn/Article/details/gjcgcycoy.sHtML

[Q52] 删除指定行
来源：http://read.share.yfazqb.com/Article/details/gdqknflqm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.tarul.cn/Article/details/gnxfxuriw.sHtML

[Q53] 按条件删除
来源：http://www.share.vehdjk.com/Article/details/gopyyspmw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.tarul.cn/Article/details/gnkgierhw.sHtML

[Q54] 清空表
来源：http://blog.epnwcf.com/Article/details/gysabolkq.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.tarul.cn/Article/details/geznncdrt.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fktsv.cn/Article/details/gblojyuwa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.yfazqb.com/Article/details/gjnrugxgk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.sjlbkw.cn/Article/details/gjrepuoqp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.yfazqb.com/Article/details/gnqpkjuww.sHtML

[Q57] 行号
来源：http://www.blog.yfazqb.com/Article/details/gmelqwqod.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.tarul.cn/Article/details/grbulytos.sHtML

[Q58] 累计求和
来源：http://baike.sjlbkw.cn/Article/details/gvfrqhtzj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.bbcook.cn/Article/details/gmavvwbsl.sHtML

[Q59] 分组内累计
来源：http://m.share.yfazqb.com/Article/details/ggivgahic.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gtbfwzlbb.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.tarul.cn/Article/details/gwlzetzwx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.bbcook.cn/Article/details/goznoezdy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gynfiysbe.sHtML

[Q61] 移动平均
来源：http://read.share.epnwcf.com/Article/details/gztdmhkvp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gpxxasuqp.sHtML

[Q62] 分组占比
来源：http://www.share.tarul.cn/Article/details/ghicarmrr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gdazvqtra.sHtML

[Q63] 开启事务
来源：http://baike.tarul.cn/Article/details/ghkjwxxht.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.tarul.cn/Article/details/gqmzfwrcc.sHtML

[Q64] 提交事务
来源：http://www.blog.yfazqb.com/Article/details/ghvzquewq.sHtML

COMMIT;
来源：http://mobile.epnwcf.com/Article/details/gmeqxybjo.sHtML

[Q65] 回滚事务
来源：http://www.share.tarul.cn/Article/details/gvipvjfsc.sHtML

ROLLBACK;
来源：http://m.share.epnwcf.com/Article/details/gegntvjsr.sHtML

[Q66] 行锁查询
来源：http://mobile.bbcook.cn/Article/details/ghqiciiwy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.bbcook.cn/Article/details/glxspdpbw.sHtML

[Q67] 设置隔离级别
来源：http://mobile.vehdjk.com/Article/details/gqdgrteiw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.yfazqb.com/Article/details/gucdfqwpg.sHtML

[Q68] 保存点
来源：http://read.share.fktsv.cn/Article/details/gprtdyrmo.sHtML

SAVEPOINT sp1;
来源：http://blog.vehdjk.com/Article/details/gkvezruki.sHtML

ROLLBACK TO sp1;
来源：http://mobile.sjlbkw.cn/Article/details/grygigzwx.sHtML

[Q69] 查看执行计划
来源：http://blog.vehdjk.com/Article/details/gknzuqcjy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.tarul.cn/Article/details/gghuurwiw.sHtML

[Q70] 更新统计信息
来源：http://3g.sjlbkw.cn/Article/details/gtntpmlpd.sHtML

ANALYZE TABLE users;
来源：http://mobile.sjlbkw.cn/Article/details/gvxsqgmbt.sHtML

[Q71] 查看建表语句
来源：http://wap.sjlbkw.cn/Article/details/gclygysgi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.yfazqb.com/Article/details/gzlyvbamr.sHtML

[Q72] 查看索引
来源：http://www.share.tarul.cn/Article/details/gescsyzbf.sHtML


<!-- 参考信息 -->