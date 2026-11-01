代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gyarfiwvd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.bbcook.cn/Article/details/grwzsmrlm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fktsv.cn/Article/details/gyidyiycx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.bbcook.cn/Article/details/gslqmjcox.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gafzreuot.sHtML

O. 并发与异步
来源：http://mobile.yfazqb.com/Article/details/grkdbdwor.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gomdxwxrm.sHtML

[O01] 启动一个线程
来源：http://www.blog.sjlbkw.cn/Article/details/gmwnnkgav.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.bbcook.cn/Article/details/grjykjfah.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.sjlbkw.cn/Article/details/gifbepqqo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.epnwcf.com/Article/details/gmzcedbdj.sHtML

TS:   // 同 JS
来源：http://www.share.vehdjk.com/Article/details/gmgolnxyd.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.bbcook.cn/Article/details/gwxpsgafq.sHtML

Go:   go f()
来源：http://www.blog.yfazqb.com/Article/details/gbopivtgs.sHtML

Ruby: Thread.new { f }
来源：http://wap.tarul.cn/Article/details/gzqgarrav.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fktsv.cn/Article/details/gwcajbhqn.sHtML

[O02] 使用线程池
来源：http://www.share.tarul.cn/Article/details/gszillkwb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.vehdjk.com/Article/details/gpccuaiyq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fktsv.cn/Article/details/gdpsidsch.sHtML

JS:   // worker_threads 线程池
来源：http://wap.bbcook.cn/Article/details/glahgtudx.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.yfazqb.com/Article/details/gngazymhc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.yfazqb.com/Article/details/gzfglajgr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fktsv.cn/Article/details/gskcxdpav.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.epnwcf.com/Article/details/gdcdbahcl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.sjlbkw.cn/Article/details/ghgkwqgua.sHtML

[O03] 加锁保护共享数据
来源：http://baike.sjlbkw.cn/Article/details/gewuhjpkw.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fktsv.cn/Article/details/gbungnanf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.sjlbkw.cn/Article/details/gdgzjafjy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.tarul.cn/Article/details/gemjaaucx.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/gygfbpvhv.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fktsv.cn/Article/details/gxmzivjku.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.bbcook.cn/Article/details/gqajbyvlg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fktsv.cn/Article/details/gfyjjfwfv.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fktsv.cn/Article/details/gchtcwzso.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.bbcook.cn/Article/details/gauhpdulg.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.yfazqb.com/Article/details/gbpjotymz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.sjlbkw.cn/Article/details/gikkcwrfl.sHtML

JS:   async function f() { await g(); }
来源：http://baike.bbcook.cn/Article/details/goyejoaqc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/gvnteftlt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fktsv.cn/Article/details/guepdhdvy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.yfazqb.com/Article/details/gkendvkhu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.epnwcf.com/Article/details/gaojzivph.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.bbcook.cn/Article/details/gjusrpiwn.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.yfazqb.com/Article/details/gynaaijsy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.vehdjk.com/Article/details/ggxnpdbmp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.yfazqb.com/Article/details/gbecxtbcg.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.bbcook.cn/Article/details/grlzpwdcm.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gpwneyryd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkuksjdil.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.epnwcf.com/Article/details/gdbfmvfkg.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.vehdjk.com/Article/details/gwxahzifw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.bbcook.cn/Article/details/gyrkhfjzc.sHtML

[O06] 使用进程池
来源：http://mobile.tarul.cn/Article/details/gfgjpceey.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.tarul.cn/Article/details/gndgxsxxl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.tarul.cn/Article/details/gexsmsgyk.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fktsv.cn/Article/details/gwiepquqd.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.tarul.cn/Article/details/gqsjfowjq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.epnwcf.com/Article/details/geupelify.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.vehdjk.com/Article/details/glbllhhzn.sHtML

Ruby: // fork 块
来源：http://www.blog.fktsv.cn/Article/details/gxjummnwy.sHtML

C#:   Parallel.For
来源：http://3g.tarul.cn/Article/details/gfiliyfcr.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gxihvpmoc.sHtML

P. 常用工具函数
来源：http://www.share.fktsv.cn/Article/details/gdchhjavh.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gumwmfddn.sHtML

[P01] 生成 UUID
来源：http://mobile.sjlbkw.cn/Article/details/glwhleezt.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.tarul.cn/Article/details/gvbvgndee.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.epnwcf.com/Article/details/gduzjdnmx.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gwakuiura.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gmsfbnwjk.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gppdetlqu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.sjlbkw.cn/Article/details/gzcicuovw.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.tarul.cn/Article/details/ggtwsbmea.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.sjlbkw.cn/Article/details/gqpyargjo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.vehdjk.com/Article/details/gzcxeaxuf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.yfazqb.com/Article/details/gfcbvsiuw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.sjlbkw.cn/Article/details/gvsweybdw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.tarul.cn/Article/details/ggxzwakbc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.vehdjk.com/Article/details/gatyqrasz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.bbcook.cn/Article/details/gbsvkmtcj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fktsv.cn/Article/details/gdqrjnhbn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fktsv.cn/Article/details/gcsollrhe.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.tarul.cn/Article/details/grwzgqkos.sHtML

[P03] 生成短随机字符串
来源：http://m.share.sjlbkw.cn/Article/details/gocjeqksd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.epnwcf.com/Article/details/gyuhyvgwe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.epnwcf.com/Article/details/gjfihgkws.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/gorcuzful.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/gynqhgdlb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.tarul.cn/Article/details/gluabblvn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.epnwcf.com/Article/details/grlaxqfdy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fktsv.cn/Article/details/gxlpfpcvt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fktsv.cn/Article/details/gglwpmqgx.sHtML

[P04] 求长度
来源：http://read.share.bbcook.cn/Article/details/gkvaktphx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.sjlbkw.cn/Article/details/gdzlffhzr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gvdcojznb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fktsv.cn/Article/details/gqphebmkh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.tarul.cn/Article/details/gubjreeha.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.tarul.cn/Article/details/gvdkwtxow.sHtML

Go:   len(arr);  len(m)
来源：http://baike.epnwcf.com/Article/details/gmxlcwdky.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.epnwcf.com/Article/details/gqekmmpmv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.epnwcf.com/Article/details/gzygcaoml.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.yfazqb.com/Article/details/gcxtawldj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.vehdjk.com/Article/details/gvlcwahev.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.yfazqb.com/Article/details/gpyhddpzt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.vehdjk.com/Article/details/glixnlzxc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.tarul.cn/Article/details/gauxghfaq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.vehdjk.com/Article/details/ghbzgrszm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.yfazqb.com/Article/details/gysmlgnbm.sHtML

Ruby: a == b
来源：http://read.share.vehdjk.com/Article/details/glttkzuls.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.vehdjk.com/Article/details/ggtrhynwx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fktsv.cn/Article/details/gjnosmjop.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fktsv.cn/Article/details/gpgrvwebi.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.epnwcf.com/Article/details/gvnejutpr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fktsv.cn/Article/details/gzncllfis.sHtML

TS:   if (x == null) {}
来源：http://baike.sjlbkw.cn/Article/details/ghvpdnwiv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.tarul.cn/Article/details/gtqfacyxn.sHtML

Go:   if x == nil {}
来源：http://www.share.bbcook.cn/Article/details/gcegwctde.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fktsv.cn/Article/details/gromemgqs.sHtML

C#:   if (x is null) {}
来源：http://wap.vehdjk.com/Article/details/gmrccybfw.sHtML

[P07] 防抖与节流
来源：http://mobile.yfazqb.com/Article/details/gstfoiowi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.bbcook.cn/Article/details/gbnljabxp.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.sjlbkw.cn/Article/details/gyyaourbw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/gzededjel.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/giuhsxylc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.epnwcf.com/Article/details/gzylkecqv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fktsv.cn/Article/details/gizglccls.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.tarul.cn/Article/details/gfsuhldhs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.sjlbkw.cn/Article/details/gmxqbwddv.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.bbcook.cn/Article/details/glmyrctvo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.bbcook.cn/Article/details/gkgrotknf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.vehdjk.com/Article/details/gzjbszrqz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.vehdjk.com/Article/details/gyinckhfm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gxqpupwro.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fktsv.cn/Article/details/gqscgsqak.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.epnwcf.com/Article/details/gpnpglqcm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.yfazqb.com/Article/details/gkwhaykop.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.sjlbkw.cn/Article/details/gzfablesm.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gvohjfbad.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fktsv.cn/Article/details/gclboejmh.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gynnytjkr.sHtML

[Q01] 创建表
来源：http://www.share.bbcook.cn/Article/details/gcwornqpq.sHtML

CREATE TABLE users (
来源：http://www.blog.tarul.cn/Article/details/goumbbnaz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.yfazqb.com/Article/details/ghqnpfbnj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.tarul.cn/Article/details/gaazajidw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.vehdjk.com/Article/details/goiqezsks.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.yfazqb.com/Article/details/gnrcmcwhy.sHtML

);
来源：http://m.share.epnwcf.com/Article/details/gzbzypghp.sHtML

[Q02] 创建带外键的表
来源：http://mobile.bbcook.cn/Article/details/gbamoisox.sHtML

CREATE TABLE orders (
来源：http://www.m.share.epnwcf.com/Article/details/guxoizsvw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gltkeiqzl.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.yfazqb.com/Article/details/gdnmazdeq.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.tarul.cn/Article/details/glmfnluut.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.yfazqb.com/Article/details/gaxbgbzdy.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/geudvvppk.sHtML

[Q03] 增加列
来源：http://www.m.share.tarul.cn/Article/details/gdrxmwnmi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.epnwcf.com/Article/details/gsarqmoga.sHtML

[Q04] 修改列类型
来源：http://3g.bbcook.cn/Article/details/geieejpwy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/gvozmgvbx.sHtML

[Q05] 重命名列
来源：http://www.share.vehdjk.com/Article/details/gdgtvyiij.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.bbcook.cn/Article/details/gnhiaohkh.sHtML

[Q06] 删除列
来源：http://3g.epnwcf.com/Article/details/gstegujpw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.tarul.cn/Article/details/gtdebjqux.sHtML

[Q07] 删除表
来源：http://wap.fktsv.cn/Article/details/gvhxdftox.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.yfazqb.com/Article/details/gsggglzky.sHtML

[Q08] 创建普通索引
来源：http://mobile.yfazqb.com/Article/details/ghgnvwjhf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.vehdjk.com/Article/details/gsssldiid.sHtML

[Q09] 创建唯一索引
来源：http://blog.fktsv.cn/Article/details/goclfvucp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.yfazqb.com/Article/details/golmreqqn.sHtML

[Q10] 插入单行
来源：http://mobile.epnwcf.com/Article/details/gzbhlmlnn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.vehdjk.com/Article/details/gezsngoyl.sHtML

[Q11] 一次插入多行
来源：http://read.share.epnwcf.com/Article/details/gddsmvafo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.bbcook.cn/Article/details/ggrznqvfc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.bbcook.cn/Article/details/gujyokoto.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.epnwcf.com/Article/details/gwrftuveu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.epnwcf.com/Article/details/gcnpasyms.sHtML

[Q13] 忽略重复插入
来源：http://baike.fktsv.cn/Article/details/gwuzsjfgo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gorsilfnk.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.epnwcf.com/Article/details/gserzvmep.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.epnwcf.com/Article/details/giloeireg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.tarul.cn/Article/details/gcyvmzuys.sHtML

[Q15] 查询全部
来源：http://3g.bbcook.cn/Article/details/gimawyxuj.sHtML

SELECT * FROM users;
来源：http://www.share.bbcook.cn/Article/details/gxkertard.sHtML

[Q16] 查询指定列
来源：http://baike.bbcook.cn/Article/details/grmufeoat.sHtML

SELECT id, name FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gqbptwabr.sHtML

[Q17] 条件查询
来源：http://www.m.share.fktsv.cn/Article/details/gamvmzhty.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.epnwcf.com/Article/details/gxvqwvkaf.sHtML

[Q18] 模糊匹配
来源：http://www.blog.bbcook.cn/Article/details/ggzkqslny.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.vehdjk.com/Article/details/gwgowllub.sHtML

[Q19] 范围查询
来源：http://blog.yfazqb.com/Article/details/gizsngqhh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.bbcook.cn/Article/details/gitlezhtp.sHtML

[Q20] IN 列表
来源：http://baike.fktsv.cn/Article/details/gxwxigqfh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fktsv.cn/Article/details/genaoqjzi.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/gmbxzymlk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.yfazqb.com/Article/details/gtwrkefiz.sHtML

[Q22] 排序
来源：http://3g.sjlbkw.cn/Article/details/gmnnqrnnh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.tarul.cn/Article/details/gbmziebii.sHtML

[Q23] 分页
来源：http://read.share.vehdjk.com/Article/details/ghntncunu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.yfazqb.com/Article/details/gfzrxflod.sHtML

[Q24] 去重
来源：http://baike.sjlbkw.cn/Article/details/gtynpgppg.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fktsv.cn/Article/details/gxazwokzu.sHtML

[Q25] 只取前 N 条
来源：http://baike.tarul.cn/Article/details/guopdsoyt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.tarul.cn/Article/details/gizzljioq.sHtML

[Q26] 计数
来源：http://3g.tarul.cn/Article/details/gnvcwxzjb.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gufbidces.sHtML

[Q27] 条件计数
来源：http://www.blog.yfazqb.com/Article/details/gkfqqxdma.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.tarul.cn/Article/details/giducssih.sHtML

[Q28] 求和与平均
来源：http://3g.epnwcf.com/Article/details/gsoutyksd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gbdmriris.sHtML

[Q29] 最大最小值
来源：http://baike.sjlbkw.cn/Article/details/gvhqfdtnv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.tarul.cn/Article/details/gdjsyfbmd.sHtML

[Q30] 分组统计
来源：http://mobile.bbcook.cn/Article/details/gsosuqngf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gpmmuearx.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fktsv.cn/Article/details/ghywafoqm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.bbcook.cn/Article/details/gekqhffyz.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gqtsbtslh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gukeukmux.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.sjlbkw.cn/Article/details/gqxluxjfx.sHtML

[Q33] 多列分组
来源：http://blog.epnwcf.com/Article/details/gnfjcvckp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.sjlbkw.cn/Article/details/gayqogyac.sHtML

[Q34] 每组取第一条
来源：http://3g.yfazqb.com/Article/details/geuwpmbxt.sHtML

SELECT * FROM (
来源：http://3g.fktsv.cn/Article/details/gutkxlxcn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.epnwcf.com/Article/details/gctryjyjx.sHtML

) t WHERE rn = 1;
来源：http://wap.tarul.cn/Article/details/gtxudtwuj.sHtML

[Q35] 内连接
来源：http://www.m.share.epnwcf.com/Article/details/gwrwvmlmw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/gjnkzkzwk.sHtML

[Q36] 左连接
来源：http://baike.tarul.cn/Article/details/gffrjrvsm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.yfazqb.com/Article/details/gdcwvfwdd.sHtML

[Q37] 右连接
来源：http://m.share.vehdjk.com/Article/details/gurxqvdyq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.bbcook.cn/Article/details/gveuaytmr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fktsv.cn/Article/details/gflnogrue.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.epnwcf.com/Article/details/grahmckrh.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.yfazqb.com/Article/details/gpkgdfwwu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.bbcook.cn/Article/details/gcaprodjs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.bbcook.cn/Article/details/grapqqzyd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.sjlbkw.cn/Article/details/gjxlrsbdq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.bbcook.cn/Article/details/gdphjcequ.sHtML

[Q41] 多表连接
来源：http://www.blog.epnwcf.com/Article/details/gxwmqrxut.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.epnwcf.com/Article/details/gwmqztfff.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.tarul.cn/Article/details/gcqbvzxxm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.vehdjk.com/Article/details/gchgfixho.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fktsv.cn/Article/details/gdsgevwrj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.yfazqb.com/Article/details/gvqoxqgib.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fktsv.cn/Article/details/gojxjzhvs.sHtML

[Q43] 标量子查询
来源：http://baike.bbcook.cn/Article/details/gzcsygckz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fktsv.cn/Article/details/gfwwmwvcn.sHtML

[Q44] IN 子查询
来源：http://www.blog.tarul.cn/Article/details/grohxrawy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.tarul.cn/Article/details/gyvsukvbn.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.vehdjk.com/Article/details/goulfvdxp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/gwufrqnwj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.bbcook.cn/Article/details/gddkxzyvd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.bbcook.cn/Article/details/ggkiovjqu.sHtML

[Q47] 与平均值比较
来源：http://wap.tarul.cn/Article/details/gcbzbrazu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.tarul.cn/Article/details/gloxoadmv.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.bbcook.cn/Article/details/ggnizmslg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fktsv.cn/Article/details/gmcgbjntg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.sjlbkw.cn/Article/details/gpvpfohkd.sHtML

[Q49] 更新单行
来源：http://www.m.share.tarul.cn/Article/details/gexelwmva.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/glcqubztz.sHtML

[Q50] 批量更新
来源：http://mobile.vehdjk.com/Article/details/gyaxhbspn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.sjlbkw.cn/Article/details/gfvnaaatv.sHtML

[Q51] 用子查询更新
来源：http://read.share.epnwcf.com/Article/details/gnhzqocnm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.tarul.cn/Article/details/gexfizkcc.sHtML

[Q52] 删除指定行
来源：http://baike.fktsv.cn/Article/details/gibnctuqx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.sjlbkw.cn/Article/details/gbrjgrrvl.sHtML

[Q53] 按条件删除
来源：http://3g.yfazqb.com/Article/details/gagysvbeq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.epnwcf.com/Article/details/grdziudob.sHtML

[Q54] 清空表
来源：http://wap.vehdjk.com/Article/details/gzsyvhkze.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fktsv.cn/Article/details/gkucmuiad.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.yfazqb.com/Article/details/gtgzhxquo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.sjlbkw.cn/Article/details/gqlbbvueq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.yfazqb.com/Article/details/gsvczsmiz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.yfazqb.com/Article/details/gmxpsaemb.sHtML

[Q57] 行号
来源：http://www.blog.sjlbkw.cn/Article/details/ggmabppoq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gsgyoevoh.sHtML

[Q58] 累计求和
来源：http://m.share.yfazqb.com/Article/details/gmpdsymhw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gmupolrft.sHtML

[Q59] 分组内累计
来源：http://mobile.tarul.cn/Article/details/gvahbpnpo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gedjkrfvh.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fktsv.cn/Article/details/gmlitafen.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.sjlbkw.cn/Article/details/gpxflhzin.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fktsv.cn/Article/details/gshqeteuf.sHtML

[Q61] 移动平均
来源：http://wap.yfazqb.com/Article/details/gnxvpjlli.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gmobugais.sHtML

[Q62] 分组占比
来源：http://mobile.fktsv.cn/Article/details/gytexbtgd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/grhhxbtyb.sHtML

[Q63] 开启事务
来源：http://3g.sjlbkw.cn/Article/details/grfmjthwi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.epnwcf.com/Article/details/getbswegv.sHtML

[Q64] 提交事务
来源：http://www.m.share.vehdjk.com/Article/details/gcnbafdbr.sHtML

COMMIT;
来源：http://blog.fktsv.cn/Article/details/gymzeybbc.sHtML

[Q65] 回滚事务
来源：http://www.share.vehdjk.com/Article/details/gztrszsqy.sHtML

ROLLBACK;
来源：http://read.share.epnwcf.com/Article/details/gwkfpbrxb.sHtML

[Q66] 行锁查询
来源：http://www.blog.fktsv.cn/Article/details/glafqtput.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.sjlbkw.cn/Article/details/gmkahodpg.sHtML

[Q67] 设置隔离级别
来源：http://baike.fktsv.cn/Article/details/gubpsmeqq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.vehdjk.com/Article/details/grgxvhspe.sHtML

[Q68] 保存点
来源：http://m.share.epnwcf.com/Article/details/gsqtnxzol.sHtML

SAVEPOINT sp1;
来源：http://www.share.sjlbkw.cn/Article/details/gwxbtqzjy.sHtML

ROLLBACK TO sp1;
来源：http://www.share.epnwcf.com/Article/details/gbblwbpwi.sHtML

[Q69] 查看执行计划
来源：http://www.blog.epnwcf.com/Article/details/gwsiaitjm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.tarul.cn/Article/details/gueprmpvm.sHtML

[Q70] 更新统计信息
来源：http://www.share.yfazqb.com/Article/details/gcxcldnbh.sHtML


<!-- 参考信息 -->