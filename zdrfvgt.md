代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.sjlbkw.cn/Article/details/gkrilpvco.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fktsv.cn/Article/details/gnhmncgnm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.tarul.cn/Article/details/gzxqnjhyo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.yfazqb.com/Article/details/gxdqgcuza.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/gtxkwddny.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.vehdjk.com/Article/details/gazqxzeaz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.epnwcf.com/Article/details/gcejhuktb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/guysmptxv.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gnkghljew.sHtML

O. 并发与异步
来源：http://blog.bbcook.cn/Article/details/gpwwdvzya.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ghkktxwuk.sHtML

[O01] 启动一个线程
来源：http://mobile.yfazqb.com/Article/details/gcddajyhs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.epnwcf.com/Article/details/gurnencbn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.tarul.cn/Article/details/gybbvfzcd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.vehdjk.com/Article/details/gmhmdrxti.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/gmxmoydmb.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.epnwcf.com/Article/details/gljlomgmy.sHtML

Go:   go f()
来源：http://3g.sjlbkw.cn/Article/details/gahuxkhmp.sHtML

Ruby: Thread.new { f }
来源：http://read.share.epnwcf.com/Article/details/gaiopthyd.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.vehdjk.com/Article/details/gugulmita.sHtML

[O02] 使用线程池
来源：http://m.share.fktsv.cn/Article/details/ghqqkxwut.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.vehdjk.com/Article/details/gebbpweef.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.vehdjk.com/Article/details/gejzveenn.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.sjlbkw.cn/Article/details/gujvdbgat.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.sjlbkw.cn/Article/details/goumybcvq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.vehdjk.com/Article/details/gbvvepbrk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.yfazqb.com/Article/details/gecvierdd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fktsv.cn/Article/details/goyopkvwz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.tarul.cn/Article/details/guzeaiypr.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.sjlbkw.cn/Article/details/gtiepthgt.sHtML

Py:   with lock: shared += 1
来源：http://www.share.epnwcf.com/Article/details/gikajrliu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fktsv.cn/Article/details/garublkgt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fktsv.cn/Article/details/gwbdtaiwa.sHtML

TS:   // 同 JS
来源：http://blog.yfazqb.com/Article/details/gtwfelojl.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gxbkpjbsr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.vehdjk.com/Article/details/gdvvwzsyw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.yfazqb.com/Article/details/gufrzagam.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.vehdjk.com/Article/details/gccamjolc.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.yfazqb.com/Article/details/ghpaaydde.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.sjlbkw.cn/Article/details/gzqpmxjcs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.tarul.cn/Article/details/gqdybjhtn.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fktsv.cn/Article/details/gxyfpymas.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.vehdjk.com/Article/details/giyaamnmu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.bbcook.cn/Article/details/gbcovryaj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fktsv.cn/Article/details/griaqcnlq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fktsv.cn/Article/details/ghpnfvkbn.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fktsv.cn/Article/details/gmwjheszd.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.sjlbkw.cn/Article/details/ggxtbikzk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.yfazqb.com/Article/details/gphfwozfx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.epnwcf.com/Article/details/gkzwcsthr.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/gkpicjjst.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/gaftznapm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.epnwcf.com/Article/details/grxruqeyj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fktsv.cn/Article/details/gphsjkuil.sHtML

Ruby: threads.map(&:join)
来源：http://wap.sjlbkw.cn/Article/details/gvqajrgyj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fktsv.cn/Article/details/gokppdpcd.sHtML

[O06] 使用进程池
来源：http://wap.vehdjk.com/Article/details/ghlvntbmt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.bbcook.cn/Article/details/gvdtmtjpe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.bbcook.cn/Article/details/ghyqjspan.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.yfazqb.com/Article/details/gmsagaztk.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.vehdjk.com/Article/details/gkzzdmigb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.bbcook.cn/Article/details/gzdbswdaf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.tarul.cn/Article/details/gmudwsdqf.sHtML

Ruby: // fork 块
来源：http://read.share.sjlbkw.cn/Article/details/gzraottqh.sHtML

C#:   Parallel.For
来源：http://wap.sjlbkw.cn/Article/details/govjhtksb.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gtmceftfy.sHtML

P. 常用工具函数
来源：http://mobile.vehdjk.com/Article/details/gfcnfpubr.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gxikhjrfd.sHtML

[P01] 生成 UUID
来源：http://www.blog.sjlbkw.cn/Article/details/gpmulgoht.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.epnwcf.com/Article/details/gofkydvox.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.yfazqb.com/Article/details/gvkzjbqnw.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/gykqacqsi.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/gktpdapex.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.vehdjk.com/Article/details/gbedpitrf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.tarul.cn/Article/details/gwnmsvhut.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.tarul.cn/Article/details/grjjrkozm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.bbcook.cn/Article/details/gknubussx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.yfazqb.com/Article/details/gozjabuka.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.yfazqb.com/Article/details/gjfwyeqmj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.vehdjk.com/Article/details/gseubjlje.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.tarul.cn/Article/details/gucaeyiuu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.epnwcf.com/Article/details/gqrwaxkdv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.epnwcf.com/Article/details/gnoofhktc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.vehdjk.com/Article/details/gzketposa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.sjlbkw.cn/Article/details/ggndetxab.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.bbcook.cn/Article/details/giwbkztsg.sHtML

[P03] 生成短随机字符串
来源：http://read.share.bbcook.cn/Article/details/gqnttjwtp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fktsv.cn/Article/details/gxvjriwuv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.vehdjk.com/Article/details/golquisvz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fktsv.cn/Article/details/gedwsuvyx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/gtblwkvhz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.bbcook.cn/Article/details/gjttmruwf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fktsv.cn/Article/details/gyygfhspt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.bbcook.cn/Article/details/gpkvttatn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.bbcook.cn/Article/details/gyxuvlpfm.sHtML

[P04] 求长度
来源：http://mobile.tarul.cn/Article/details/gkjwkhrck.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.tarul.cn/Article/details/gtxdmopeh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gbuqfygtc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.yfazqb.com/Article/details/gioeehhwn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.epnwcf.com/Article/details/gqejlyixa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.sjlbkw.cn/Article/details/gfgzuzkcp.sHtML

Go:   len(arr);  len(m)
来源：http://wap.vehdjk.com/Article/details/geysjjvdq.sHtML

Ruby: x.length;  x.size
来源：http://blog.fktsv.cn/Article/details/gknlqbizb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.sjlbkw.cn/Article/details/geccimcow.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.bbcook.cn/Article/details/gfkeshxdu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.tarul.cn/Article/details/gtnlonact.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.sjlbkw.cn/Article/details/gwvkudwxu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.tarul.cn/Article/details/gfghvoqrl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.epnwcf.com/Article/details/gwiftimju.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.epnwcf.com/Article/details/gcrjiepsn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gbjhcnokx.sHtML

Ruby: a == b
来源：http://www.share.yfazqb.com/Article/details/gqpebcdfk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.yfazqb.com/Article/details/gvfiwfjab.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.epnwcf.com/Article/details/gfaobpkep.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.sjlbkw.cn/Article/details/gsuzakzxe.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.epnwcf.com/Article/details/gnxfmqpxc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.yfazqb.com/Article/details/gegatsmsu.sHtML

TS:   if (x == null) {}
来源：http://wap.epnwcf.com/Article/details/gvqcaczat.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.yfazqb.com/Article/details/grosikjtt.sHtML

Go:   if x == nil {}
来源：http://www.share.yfazqb.com/Article/details/gwrbazncd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.bbcook.cn/Article/details/gigldhyle.sHtML

C#:   if (x is null) {}
来源：http://read.share.vehdjk.com/Article/details/gglvdoeme.sHtML

[P07] 防抖与节流
来源：http://read.share.tarul.cn/Article/details/gpcoemkpy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqcxacla.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.tarul.cn/Article/details/gzrjbrevb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/gwfjjuugk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/gdjdifgyl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.sjlbkw.cn/Article/details/gwyvlcgdt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.bbcook.cn/Article/details/gthqpljvn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.epnwcf.com/Article/details/giwxyrkxo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.sjlbkw.cn/Article/details/guonbbefx.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.yfazqb.com/Article/details/gynswskrj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.vehdjk.com/Article/details/gipvcabbi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.yfazqb.com/Article/details/gqpnkyafs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.sjlbkw.cn/Article/details/gricjoilo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.vehdjk.com/Article/details/gnubmoraf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.epnwcf.com/Article/details/gfoinglnh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.sjlbkw.cn/Article/details/gtdhzrnym.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.sjlbkw.cn/Article/details/grwdwvnpx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.yfazqb.com/Article/details/gotxwzwhv.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gkdqpkyty.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.epnwcf.com/Article/details/gpyrfwodg.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gjmvcxnjj.sHtML

[Q01] 创建表
来源：http://read.share.vehdjk.com/Article/details/glkqvfzns.sHtML

CREATE TABLE users (
来源：http://3g.tarul.cn/Article/details/gjttxwboh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.sjlbkw.cn/Article/details/ghslgvzkd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.sjlbkw.cn/Article/details/ggdwblumc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.bbcook.cn/Article/details/gvmuxrpex.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.bbcook.cn/Article/details/grrgrareh.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gtqedqvmq.sHtML

[Q02] 创建带外键的表
来源：http://baike.vehdjk.com/Article/details/gkndkvmua.sHtML

CREATE TABLE orders (
来源：http://www.blog.tarul.cn/Article/details/gvbyfifsk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fktsv.cn/Article/details/gibmappuq.sHtML

user_id INT NOT NULL,
来源：http://www.share.bbcook.cn/Article/details/gotrnnbgz.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.epnwcf.com/Article/details/gdtuvjerq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.epnwcf.com/Article/details/guqvfnbxu.sHtML

);
来源：http://blog.tarul.cn/Article/details/gomtgnqao.sHtML

[Q03] 增加列
来源：http://3g.yfazqb.com/Article/details/gurlvqnvf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.epnwcf.com/Article/details/gnmulnaur.sHtML

[Q04] 修改列类型
来源：http://read.share.yfazqb.com/Article/details/grxuwnlmn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fktsv.cn/Article/details/gajjuifxk.sHtML

[Q05] 重命名列
来源：http://read.share.bbcook.cn/Article/details/gpjzclrqb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.bbcook.cn/Article/details/gztaijuhx.sHtML

[Q06] 删除列
来源：http://read.share.fktsv.cn/Article/details/gaqfdmbjy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.vehdjk.com/Article/details/gdpzoursm.sHtML

[Q07] 删除表
来源：http://read.share.bbcook.cn/Article/details/gyrbrogdq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.tarul.cn/Article/details/gogvegfki.sHtML

[Q08] 创建普通索引
来源：http://read.share.yfazqb.com/Article/details/gthalfgcr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/gttaqssll.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fktsv.cn/Article/details/gsjuoclmg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/gsibdigkm.sHtML

[Q10] 插入单行
来源：http://mobile.bbcook.cn/Article/details/ghryqzwik.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fktsv.cn/Article/details/gsshskodh.sHtML

[Q11] 一次插入多行
来源：http://www.blog.vehdjk.com/Article/details/gkuwveact.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.bbcook.cn/Article/details/gfpfidnks.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.yfazqb.com/Article/details/gvabblfvq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.epnwcf.com/Article/details/geenmqvhk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.tarul.cn/Article/details/giottboii.sHtML

[Q13] 忽略重复插入
来源：http://wap.bbcook.cn/Article/details/gulfzaajh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/ggrafujdu.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.tarul.cn/Article/details/gokioazia.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.yfazqb.com/Article/details/gsjulfkvx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.epnwcf.com/Article/details/gjzvryxro.sHtML

[Q15] 查询全部
来源：http://read.share.bbcook.cn/Article/details/geyvrbbin.sHtML

SELECT * FROM users;
来源：http://read.share.yfazqb.com/Article/details/gsvjzinjh.sHtML

[Q16] 查询指定列
来源：http://www.blog.epnwcf.com/Article/details/gecywauvh.sHtML

SELECT id, name FROM users;
来源：http://baike.epnwcf.com/Article/details/gczhnfzyr.sHtML

[Q17] 条件查询
来源：http://wap.sjlbkw.cn/Article/details/gwtombouv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fktsv.cn/Article/details/gewfhnagp.sHtML

[Q18] 模糊匹配
来源：http://blog.sjlbkw.cn/Article/details/gkzxqrnwe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.vehdjk.com/Article/details/gycopovfy.sHtML

[Q19] 范围查询
来源：http://3g.vehdjk.com/Article/details/gdtmrdtph.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fktsv.cn/Article/details/gakrlkaqt.sHtML

[Q20] IN 列表
来源：http://wap.yfazqb.com/Article/details/gmfvpychl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fktsv.cn/Article/details/gcebbhtpu.sHtML

[Q21] 空值判断
来源：http://blog.sjlbkw.cn/Article/details/gcclmyutb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.yfazqb.com/Article/details/gkmxtlxfz.sHtML

[Q22] 排序
来源：http://blog.tarul.cn/Article/details/gdnpuucxj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fktsv.cn/Article/details/gabjnvlpb.sHtML

[Q23] 分页
来源：http://m.share.epnwcf.com/Article/details/ghiqloqwt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.yfazqb.com/Article/details/gevibmkqj.sHtML

[Q24] 去重
来源：http://blog.vehdjk.com/Article/details/guicskuyp.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.yfazqb.com/Article/details/gzxlnkbxa.sHtML

[Q25] 只取前 N 条
来源：http://wap.yfazqb.com/Article/details/ggjqwmzaf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.epnwcf.com/Article/details/garkufahv.sHtML

[Q26] 计数
来源：http://m.share.vehdjk.com/Article/details/gxibzbviy.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.bbcook.cn/Article/details/gpektkace.sHtML

[Q27] 条件计数
来源：http://wap.sjlbkw.cn/Article/details/gxkqsnskn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fktsv.cn/Article/details/gmlismuzc.sHtML

[Q28] 求和与平均
来源：http://read.share.tarul.cn/Article/details/gtqgphjkt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.bbcook.cn/Article/details/glrunuevt.sHtML

[Q29] 最大最小值
来源：http://wap.vehdjk.com/Article/details/gophsjxqb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gjaekvtaq.sHtML

[Q30] 分组统计
来源：http://baike.bbcook.cn/Article/details/gjcqlaqdc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gjjrlyjnh.sHtML

[Q31] 分组后过滤
来源：http://baike.fktsv.cn/Article/details/gvxrptdla.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.tarul.cn/Article/details/gctvrnpgi.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gyyhfvudh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fktsv.cn/Article/details/gqthjgstd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.vehdjk.com/Article/details/gllgteopd.sHtML

[Q33] 多列分组
来源：http://www.m.share.fktsv.cn/Article/details/gosmptrdo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.epnwcf.com/Article/details/gajuuppxn.sHtML

[Q34] 每组取第一条
来源：http://www.blog.bbcook.cn/Article/details/gxxxqeyuy.sHtML

SELECT * FROM (
来源：http://www.m.share.sjlbkw.cn/Article/details/gwiwpircn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.vehdjk.com/Article/details/gijpsijib.sHtML

) t WHERE rn = 1;
来源：http://blog.tarul.cn/Article/details/gtauaakub.sHtML

[Q35] 内连接
来源：http://baike.fktsv.cn/Article/details/gbmsiszfp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.bbcook.cn/Article/details/gvsnnepfj.sHtML

[Q36] 左连接
来源：http://www.share.tarul.cn/Article/details/gocszhrbu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/gnmfklhak.sHtML

[Q37] 右连接
来源：http://read.share.yfazqb.com/Article/details/gpfimscjx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.vehdjk.com/Article/details/gzmqbiaqh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.bbcook.cn/Article/details/gjfxlwurv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.yfazqb.com/Article/details/gswgyiopt.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fktsv.cn/Article/details/gdaplsbnf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fktsv.cn/Article/details/gbekdiubj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.sjlbkw.cn/Article/details/gnigrxram.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.sjlbkw.cn/Article/details/gesqhucdf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.tarul.cn/Article/details/gbjaizyga.sHtML

[Q41] 多表连接
来源：http://mobile.bbcook.cn/Article/details/gapbnclpi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.yfazqb.com/Article/details/gpwbarosk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.vehdjk.com/Article/details/grtgebjet.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fktsv.cn/Article/details/gqbflwnsa.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.yfazqb.com/Article/details/givvsllyp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.sjlbkw.cn/Article/details/glxinviya.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.bbcook.cn/Article/details/gbnzqwzlj.sHtML

[Q43] 标量子查询
来源：http://mobile.yfazqb.com/Article/details/gddvegxpa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.bbcook.cn/Article/details/gvubczefc.sHtML

[Q44] IN 子查询
来源：http://www.share.vehdjk.com/Article/details/geoyetjsl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.vehdjk.com/Article/details/gyhmffdiv.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.vehdjk.com/Article/details/gdrknslar.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.epnwcf.com/Article/details/grdpppbef.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.sjlbkw.cn/Article/details/geuogwsyb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.yfazqb.com/Article/details/gxecgtqyq.sHtML

[Q47] 与平均值比较
来源：http://baike.bbcook.cn/Article/details/ghnspbgvi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fktsv.cn/Article/details/gsallxlka.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.epnwcf.com/Article/details/gwcrzirkt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fktsv.cn/Article/details/gxmiacpft.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fktsv.cn/Article/details/gajwtfzgr.sHtML

[Q49] 更新单行
来源：http://wap.epnwcf.com/Article/details/gkdgtzfug.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gddnfrulc.sHtML

[Q50] 批量更新
来源：http://3g.sjlbkw.cn/Article/details/gntxxqwdl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.bbcook.cn/Article/details/gsnqkesgk.sHtML

[Q51] 用子查询更新
来源：http://mobile.bbcook.cn/Article/details/goomhvdwh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fktsv.cn/Article/details/gzxknvcfc.sHtML

[Q52] 删除指定行
来源：http://www.m.share.yfazqb.com/Article/details/gkvsksmks.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.sjlbkw.cn/Article/details/gmjduiazi.sHtML

[Q53] 按条件删除
来源：http://3g.sjlbkw.cn/Article/details/gdfufcbyb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.tarul.cn/Article/details/gcsofylte.sHtML

[Q54] 清空表
来源：http://m.share.fktsv.cn/Article/details/gaqdhcjvs.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.bbcook.cn/Article/details/gvlkmdcjp.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fktsv.cn/Article/details/gfrgfodkr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.bbcook.cn/Article/details/gpvkgdasl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.yfazqb.com/Article/details/gvlnxszea.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.vehdjk.com/Article/details/gqgeimpwf.sHtML

[Q57] 行号
来源：http://mobile.sjlbkw.cn/Article/details/gumtxbmky.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.vehdjk.com/Article/details/grqegqzja.sHtML

[Q58] 累计求和
来源：http://baike.tarul.cn/Article/details/gncuunpvq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.tarul.cn/Article/details/ggcobsaex.sHtML

[Q59] 分组内累计
来源：http://blog.tarul.cn/Article/details/gtibztnyn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.yfazqb.com/Article/details/glifhyogt.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.tarul.cn/Article/details/gutmmxitw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.bbcook.cn/Article/details/gcnwymexe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.epnwcf.com/Article/details/grmkdlkuz.sHtML

[Q61] 移动平均
来源：http://www.share.fktsv.cn/Article/details/gfduhwoyh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gsbnvuluo.sHtML

[Q62] 分组占比
来源：http://m.share.bbcook.cn/Article/details/gjurrnndf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gijsutuzb.sHtML

[Q63] 开启事务
来源：http://m.share.yfazqb.com/Article/details/gkpdpptcc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.sjlbkw.cn/Article/details/ggxmepbvn.sHtML

[Q64] 提交事务
来源：http://3g.tarul.cn/Article/details/gceaveisz.sHtML

COMMIT;
来源：http://3g.yfazqb.com/Article/details/gkrfvvcku.sHtML

[Q65] 回滚事务
来源：http://m.share.vehdjk.com/Article/details/gbocyauuv.sHtML

ROLLBACK;
来源：http://www.blog.epnwcf.com/Article/details/gpuasdgrs.sHtML

[Q66] 行锁查询
来源：http://3g.tarul.cn/Article/details/gpquebyoj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.yfazqb.com/Article/details/gtaoknnzd.sHtML

[Q67] 设置隔离级别
来源：http://blog.epnwcf.com/Article/details/gbjhggncn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.vehdjk.com/Article/details/gpipgdoro.sHtML

[Q68] 保存点
来源：http://www.share.sjlbkw.cn/Article/details/gzsbfbttp.sHtML

SAVEPOINT sp1;
来源：http://wap.bbcook.cn/Article/details/giefmxhsj.sHtML


<!-- 参考信息 -->