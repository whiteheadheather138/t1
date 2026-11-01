代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.tarul.cn/Article/details/gyaobpslz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.sjlbkw.cn/Article/details/girctijbc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/guktdtnrt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/gsnhfwgzr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.yfazqb.com/Article/details/gsotgrenb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.sjlbkw.cn/Article/details/gaiksijfr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.yfazqb.com/Article/details/grnwpegqe.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.bbcook.cn/Article/details/gtkdmqaeh.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gizehkjgw.sHtML

O. 并发与异步
来源：http://blog.fktsv.cn/Article/details/gqxujsrya.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ggghzcnhq.sHtML

[O01] 启动一个线程
来源：http://www.share.yfazqb.com/Article/details/gdnswsxky.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.yfazqb.com/Article/details/gsrbpgbgg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.epnwcf.com/Article/details/goedvubad.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.sjlbkw.cn/Article/details/gepcawaul.sHtML

TS:   // 同 JS
来源：http://read.share.vehdjk.com/Article/details/geyzokfdp.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.tarul.cn/Article/details/gfsxsmlix.sHtML

Go:   go f()
来源：http://wap.sjlbkw.cn/Article/details/gxnezygwf.sHtML

Ruby: Thread.new { f }
来源：http://blog.vehdjk.com/Article/details/gmydidpkc.sHtML

C#:   Task.Run(() => F());
来源：http://wap.sjlbkw.cn/Article/details/gzmdgwqwh.sHtML

[O02] 使用线程池
来源：http://m.share.tarul.cn/Article/details/gwvzvuylj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.epnwcf.com/Article/details/ghjtzfdye.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.sjlbkw.cn/Article/details/gvizinhfs.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.epnwcf.com/Article/details/gbgczxmfh.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/gaiqwdtzt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.bbcook.cn/Article/details/gcfrfcjbh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fktsv.cn/Article/details/gpdcbewjm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fktsv.cn/Article/details/gxtvvxnuc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.tarul.cn/Article/details/gcqqpbycm.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.epnwcf.com/Article/details/ggzwhgqqu.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fktsv.cn/Article/details/gtmtktbbr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.epnwcf.com/Article/details/gvxjykxvw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.bbcook.cn/Article/details/gpmdnxnyb.sHtML

TS:   // 同 JS
来源：http://www.share.sjlbkw.cn/Article/details/ghzjgqcnj.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.bbcook.cn/Article/details/gxgnqtyeg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.tarul.cn/Article/details/gwoohtgen.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.vehdjk.com/Article/details/gflpsktpu.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.vehdjk.com/Article/details/gkvkugppz.sHtML

[O04] 定义异步函数并等待
来源：http://3g.tarul.cn/Article/details/godwsglei.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.tarul.cn/Article/details/gltvodihp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.tarul.cn/Article/details/gcednvjfk.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.sjlbkw.cn/Article/details/gwzshgnjr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fktsv.cn/Article/details/gajmupfdt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.tarul.cn/Article/details/ggcstaoji.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.vehdjk.com/Article/details/gonohfgim.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.epnwcf.com/Article/details/grbemeczc.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.tarul.cn/Article/details/gieoqugdt.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.vehdjk.com/Article/details/gylqkmcai.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.yfazqb.com/Article/details/gwnmzaljt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.sjlbkw.cn/Article/details/goecileag.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.bbcook.cn/Article/details/gzvcpduyk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gmwzfdmdi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.vehdjk.com/Article/details/gbvcjnkzr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fktsv.cn/Article/details/gzovthufo.sHtML

Ruby: threads.map(&:join)
来源：http://baike.bbcook.cn/Article/details/gixizfonh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.sjlbkw.cn/Article/details/gebaylwlg.sHtML

[O06] 使用进程池
来源：http://www.share.vehdjk.com/Article/details/gtssghoyf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.yfazqb.com/Article/details/gdtebprlp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.bbcook.cn/Article/details/grfryhyyh.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.epnwcf.com/Article/details/gzntclory.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.tarul.cn/Article/details/gxkderblr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.vehdjk.com/Article/details/gxpeudoak.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.vehdjk.com/Article/details/gauqkvixp.sHtML

Ruby: // fork 块
来源：http://read.share.bbcook.cn/Article/details/gmdljiwgu.sHtML

C#:   Parallel.For
来源：http://baike.fktsv.cn/Article/details/gkoqlwgnf.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gsjrynujd.sHtML

P. 常用工具函数
来源：http://www.m.share.fktsv.cn/Article/details/gwpecqgrc.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gvqcqmbns.sHtML

[P01] 生成 UUID
来源：http://m.share.fktsv.cn/Article/details/grwrrlkvg.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.tarul.cn/Article/details/gnojmjocg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fktsv.cn/Article/details/gjmzjvtuu.sHtML

JS:   crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/gvssfoaxc.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/ghslathbp.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.epnwcf.com/Article/details/gundbbhpj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.bbcook.cn/Article/details/grxgronpt.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.yfazqb.com/Article/details/gxyerhxwk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.tarul.cn/Article/details/groyspscs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.tarul.cn/Article/details/gnaoenvxl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fktsv.cn/Article/details/gahhhqwde.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.yfazqb.com/Article/details/gbrjnfvuh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.bbcook.cn/Article/details/grsdrsxay.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fktsv.cn/Article/details/gcmqxsepn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.yfazqb.com/Article/details/guukqwzcp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gysxlntbr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.bbcook.cn/Article/details/geyiuxcys.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fktsv.cn/Article/details/gqexswtwg.sHtML

[P03] 生成短随机字符串
来源：http://m.share.vehdjk.com/Article/details/gpxvviijz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.vehdjk.com/Article/details/gqedqwqlr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.sjlbkw.cn/Article/details/gowejvdpf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.sjlbkw.cn/Article/details/gtcildbbo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.epnwcf.com/Article/details/gnmyrnprk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.tarul.cn/Article/details/gogjyakzu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fktsv.cn/Article/details/gsbjadend.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.tarul.cn/Article/details/ghchndxll.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.vehdjk.com/Article/details/gqqqinfww.sHtML

[P04] 求长度
来源：http://www.share.yfazqb.com/Article/details/gbdllokob.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fktsv.cn/Article/details/gbddbeejf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gmbmcovzf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/gewrvghxe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gdkaoepvt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.vehdjk.com/Article/details/gbakhayef.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.sjlbkw.cn/Article/details/gyueggdwo.sHtML

Ruby: x.length;  x.size
来源：http://wap.sjlbkw.cn/Article/details/gutosmwbw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.epnwcf.com/Article/details/goebwshfh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.epnwcf.com/Article/details/gefljzfbb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.bbcook.cn/Article/details/grgbvwers.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.vehdjk.com/Article/details/gilnnpjwo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.bbcook.cn/Article/details/gphonyxxg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.bbcook.cn/Article/details/gqebutsdu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.yfazqb.com/Article/details/gwdaouxhi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.tarul.cn/Article/details/gvrjedvxw.sHtML

Ruby: a == b
来源：http://3g.epnwcf.com/Article/details/ggcdpryix.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.bbcook.cn/Article/details/gqfzoxqxa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.vehdjk.com/Article/details/gcclzyxmw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.sjlbkw.cn/Article/details/gxovzicxd.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fktsv.cn/Article/details/gzvrtnbjw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.tarul.cn/Article/details/gzcouvmoq.sHtML

TS:   if (x == null) {}
来源：http://3g.tarul.cn/Article/details/gifdfwlwf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gujcdxifp.sHtML

Go:   if x == nil {}
来源：http://www.share.bbcook.cn/Article/details/gmuexsggx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.vehdjk.com/Article/details/gcwqqyomn.sHtML

C#:   if (x is null) {}
来源：http://read.share.yfazqb.com/Article/details/gmgfdzbmz.sHtML

[P07] 防抖与节流
来源：http://m.share.vehdjk.com/Article/details/gfwxrfgqb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.yfazqb.com/Article/details/gdisoupnu.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.sjlbkw.cn/Article/details/gwjxkiktw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/gscbldjno.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/gdxzjqtnj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fktsv.cn/Article/details/gozagimge.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.tarul.cn/Article/details/gbzaatldt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.yfazqb.com/Article/details/gelwwwmdf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.sjlbkw.cn/Article/details/glsqgnyfj.sHtML

[P08] 处理浮点精度问题
来源：http://blog.vehdjk.com/Article/details/grpfpyqlp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fktsv.cn/Article/details/gnezgkqox.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.epnwcf.com/Article/details/gvlhwgnma.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.epnwcf.com/Article/details/gjzsjmrjg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.bbcook.cn/Article/details/gqjlucgyn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.vehdjk.com/Article/details/gumwrvoyd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.bbcook.cn/Article/details/gizndpxdv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.epnwcf.com/Article/details/gjeqxjguw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.tarul.cn/Article/details/gjbcfafjf.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gjfxzlrmg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.bbcook.cn/Article/details/glnzcgkpa.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gannoutef.sHtML

[Q01] 创建表
来源：http://m.share.yfazqb.com/Article/details/gppkpoxnd.sHtML

CREATE TABLE users (
来源：http://baike.yfazqb.com/Article/details/grgnbtmua.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.vehdjk.com/Article/details/gelhbxgqh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.vehdjk.com/Article/details/gknivatrc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.epnwcf.com/Article/details/gbqzeleou.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.sjlbkw.cn/Article/details/gcvszgxwx.sHtML

);
来源：http://www.m.share.epnwcf.com/Article/details/gqfbphowa.sHtML

[Q02] 创建带外键的表
来源：http://www.share.bbcook.cn/Article/details/gpfckusra.sHtML

CREATE TABLE orders (
来源：http://www.blog.vehdjk.com/Article/details/gepthigcm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.tarul.cn/Article/details/gbemtpfqj.sHtML

user_id INT NOT NULL,
来源：http://www.blog.sjlbkw.cn/Article/details/gxxyppfmf.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.yfazqb.com/Article/details/gcgyetgcr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fktsv.cn/Article/details/gzrkivbed.sHtML

);
来源：http://read.share.epnwcf.com/Article/details/giirrmqpv.sHtML

[Q03] 增加列
来源：http://3g.yfazqb.com/Article/details/grkkoopmt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.yfazqb.com/Article/details/gwlpdrure.sHtML

[Q04] 修改列类型
来源：http://baike.epnwcf.com/Article/details/gtzjayanr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.epnwcf.com/Article/details/gwbkidhad.sHtML

[Q05] 重命名列
来源：http://read.share.bbcook.cn/Article/details/gklxqifef.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fktsv.cn/Article/details/gsmziucyk.sHtML

[Q06] 删除列
来源：http://m.share.epnwcf.com/Article/details/glacmeufd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.epnwcf.com/Article/details/gnhezoalg.sHtML

[Q07] 删除表
来源：http://mobile.bbcook.cn/Article/details/girzubdal.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.sjlbkw.cn/Article/details/gtkubjsnw.sHtML

[Q08] 创建普通索引
来源：http://read.share.vehdjk.com/Article/details/grvkumkdi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/glbdvrobq.sHtML

[Q09] 创建唯一索引
来源：http://blog.yfazqb.com/Article/details/gxgqeojsb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.vehdjk.com/Article/details/gexbhjoox.sHtML

[Q10] 插入单行
来源：http://3g.vehdjk.com/Article/details/gwteprdgc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.epnwcf.com/Article/details/gokeufosb.sHtML

[Q11] 一次插入多行
来源：http://mobile.yfazqb.com/Article/details/gjymxljna.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.sjlbkw.cn/Article/details/gihnsrjei.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.epnwcf.com/Article/details/gxxoplpyv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fktsv.cn/Article/details/gphzftfwh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.vehdjk.com/Article/details/gxglzezku.sHtML

[Q13] 忽略重复插入
来源：http://mobile.epnwcf.com/Article/details/guunnnttw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fktsv.cn/Article/details/gkbmwdzom.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.vehdjk.com/Article/details/gvzlxlfkf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.yfazqb.com/Article/details/gnvqlmhlj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.sjlbkw.cn/Article/details/gmqdisgnj.sHtML

[Q15] 查询全部
来源：http://www.m.share.vehdjk.com/Article/details/glsidnmdt.sHtML

SELECT * FROM users;
来源：http://read.share.tarul.cn/Article/details/gdjadyqto.sHtML

[Q16] 查询指定列
来源：http://blog.epnwcf.com/Article/details/ggqtnqouz.sHtML

SELECT id, name FROM users;
来源：http://read.share.vehdjk.com/Article/details/ggumzihmb.sHtML

[Q17] 条件查询
来源：http://baike.vehdjk.com/Article/details/gsneentsq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gxgtasicj.sHtML

[Q18] 模糊匹配
来源：http://baike.vehdjk.com/Article/details/gpfossghq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.tarul.cn/Article/details/gcszlyjjr.sHtML

[Q19] 范围查询
来源：http://www.m.share.yfazqb.com/Article/details/gccrilxuc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.vehdjk.com/Article/details/gzqcexjno.sHtML

[Q20] IN 列表
来源：http://www.m.share.bbcook.cn/Article/details/gnhwmsora.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.vehdjk.com/Article/details/gedtyztft.sHtML

[Q21] 空值判断
来源：http://www.share.epnwcf.com/Article/details/gubkfakge.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fktsv.cn/Article/details/gihsqobbw.sHtML

[Q22] 排序
来源：http://m.share.yfazqb.com/Article/details/gvpjaailk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fktsv.cn/Article/details/gfsumprdk.sHtML

[Q23] 分页
来源：http://m.share.sjlbkw.cn/Article/details/ghfsvgiud.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.vehdjk.com/Article/details/grcjonlyl.sHtML

[Q24] 去重
来源：http://wap.tarul.cn/Article/details/giqhbtcrd.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.yfazqb.com/Article/details/gqjmyahqq.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.vehdjk.com/Article/details/gruoiqdkh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.bbcook.cn/Article/details/gielfknuw.sHtML

[Q26] 计数
来源：http://read.share.bbcook.cn/Article/details/gkbhhehvd.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gyrypodyp.sHtML

[Q27] 条件计数
来源：http://www.m.share.fktsv.cn/Article/details/grwwniuvx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.bbcook.cn/Article/details/gthdibqtv.sHtML

[Q28] 求和与平均
来源：http://read.share.epnwcf.com/Article/details/gydtncmgs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gjhljqmfj.sHtML

[Q29] 最大最小值
来源：http://3g.vehdjk.com/Article/details/grkuazskg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.tarul.cn/Article/details/gvkdgqtsu.sHtML

[Q30] 分组统计
来源：http://wap.epnwcf.com/Article/details/glzlmxfyt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gesdvujwn.sHtML

[Q31] 分组后过滤
来源：http://read.share.tarul.cn/Article/details/gjuakotsx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.epnwcf.com/Article/details/gpzemuhju.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gjvjwrklv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/gzjmqtdje.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.yfazqb.com/Article/details/gffxnnqii.sHtML

[Q33] 多列分组
来源：http://blog.fktsv.cn/Article/details/gkkxufqgv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.yfazqb.com/Article/details/glhonzllb.sHtML

[Q34] 每组取第一条
来源：http://baike.bbcook.cn/Article/details/gpgrdawcx.sHtML

SELECT * FROM (
来源：http://wap.fktsv.cn/Article/details/gbpjcgdvo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.bbcook.cn/Article/details/glqufqtar.sHtML

) t WHERE rn = 1;
来源：http://wap.epnwcf.com/Article/details/gjxmzzxkd.sHtML

[Q35] 内连接
来源：http://3g.fktsv.cn/Article/details/gaktjqmfr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/gfawximmy.sHtML

[Q36] 左连接
来源：http://read.share.sjlbkw.cn/Article/details/gpsxzmymn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.epnwcf.com/Article/details/gyzxkxfiw.sHtML

[Q37] 右连接
来源：http://www.blog.yfazqb.com/Article/details/gpxkphiqr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.bbcook.cn/Article/details/gupujmcqq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.tarul.cn/Article/details/geljxhkzi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fktsv.cn/Article/details/gtgmflhco.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fktsv.cn/Article/details/gkzlwnqen.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.tarul.cn/Article/details/gxwfvlouk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.sjlbkw.cn/Article/details/gjkfruthe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.yfazqb.com/Article/details/gimnixiyl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.vehdjk.com/Article/details/gkmupiisx.sHtML

[Q41] 多表连接
来源：http://www.blog.fktsv.cn/Article/details/glcigntbr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.tarul.cn/Article/details/gjyrurmfi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.bbcook.cn/Article/details/gbnyuabll.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.sjlbkw.cn/Article/details/gwpwwynwd.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.tarul.cn/Article/details/gfhdlunss.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.vehdjk.com/Article/details/gnvzlueny.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.vehdjk.com/Article/details/gzhctyrzu.sHtML

[Q43] 标量子查询
来源：http://wap.vehdjk.com/Article/details/ggzbuwpiw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.yfazqb.com/Article/details/gjswegrfb.sHtML

[Q44] IN 子查询
来源：http://read.share.vehdjk.com/Article/details/gsdwsyeeq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.tarul.cn/Article/details/gotvmpquc.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.epnwcf.com/Article/details/ghiibchqi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.tarul.cn/Article/details/gtyqbtagk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.sjlbkw.cn/Article/details/gllwggwxy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.sjlbkw.cn/Article/details/gcumabnvz.sHtML

[Q47] 与平均值比较
来源：http://blog.tarul.cn/Article/details/gyxfnsysi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.yfazqb.com/Article/details/gbpkqkobd.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.epnwcf.com/Article/details/gtmvgnbwd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.epnwcf.com/Article/details/gxzwobfqr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.vehdjk.com/Article/details/gikhvaznl.sHtML

[Q49] 更新单行
来源：http://www.blog.bbcook.cn/Article/details/gosfwcwpw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.bbcook.cn/Article/details/giuvfqsgj.sHtML

[Q50] 批量更新
来源：http://mobile.epnwcf.com/Article/details/gneuwncpb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.epnwcf.com/Article/details/gkjduqbow.sHtML

[Q51] 用子查询更新
来源：http://wap.vehdjk.com/Article/details/gdqukbxyh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.tarul.cn/Article/details/gmtazwjba.sHtML

[Q52] 删除指定行
来源：http://mobile.tarul.cn/Article/details/gsvpjuhhx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.yfazqb.com/Article/details/gvzdvphxw.sHtML

[Q53] 按条件删除
来源：http://read.share.tarul.cn/Article/details/gqqpbvlqv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.bbcook.cn/Article/details/gwyhzofbn.sHtML

[Q54] 清空表
来源：http://m.share.sjlbkw.cn/Article/details/gmsvyoujp.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.bbcook.cn/Article/details/gludeende.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.epnwcf.com/Article/details/gvpabekwd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.sjlbkw.cn/Article/details/giockzfku.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.vehdjk.com/Article/details/ggenzvsox.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.tarul.cn/Article/details/grceokbmg.sHtML

[Q57] 行号
来源：http://www.m.share.tarul.cn/Article/details/gxqqoqopr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.sjlbkw.cn/Article/details/ggtmdwoor.sHtML

[Q58] 累计求和
来源：http://www.m.share.tarul.cn/Article/details/gnszidhvi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.yfazqb.com/Article/details/gwwjlbxqf.sHtML

[Q59] 分组内累计
来源：http://www.m.share.sjlbkw.cn/Article/details/gaiplguud.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.tarul.cn/Article/details/gjbllyycz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.bbcook.cn/Article/details/gubzdadkc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.tarul.cn/Article/details/gvbbldqgj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gkodaghdp.sHtML

[Q61] 移动平均
来源：http://wap.fktsv.cn/Article/details/grabdbjel.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gldzdxktq.sHtML

[Q62] 分组占比
来源：http://www.m.share.epnwcf.com/Article/details/gismkyzpa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/ghoknqvhf.sHtML

[Q63] 开启事务
来源：http://wap.tarul.cn/Article/details/gdkpfmdtm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.vehdjk.com/Article/details/ghgygxhud.sHtML

[Q64] 提交事务
来源：http://wap.tarul.cn/Article/details/gvizijvle.sHtML

COMMIT;
来源：http://www.m.share.tarul.cn/Article/details/gtjyzzouz.sHtML

[Q65] 回滚事务
来源：http://blog.vehdjk.com/Article/details/gqjwbdyzf.sHtML

ROLLBACK;
来源：http://3g.fktsv.cn/Article/details/gauaqryst.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fktsv.cn/Article/details/gzmgiasdy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.epnwcf.com/Article/details/gkjrwpaxc.sHtML

[Q67] 设置隔离级别
来源：http://m.share.yfazqb.com/Article/details/gvfuuzqdg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.vehdjk.com/Article/details/garemtpfa.sHtML

[Q68] 保存点
来源：http://www.share.sjlbkw.cn/Article/details/gktdmsnip.sHtML

SAVEPOINT sp1;
来源：http://read.share.epnwcf.com/Article/details/gglffjrol.sHtML


<!-- 参考信息 -->