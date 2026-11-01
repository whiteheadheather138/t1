代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.bbcook.cn/Article/details/gyxemnsly.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.epnwcf.com/Article/details/gizyntbye.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/gcbkbzfnv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.sjlbkw.cn/Article/details/gquqhmakw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/gjtbzygad.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.bbcook.cn/Article/details/gzoxhswvs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.bbcook.cn/Article/details/gxxufzors.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.sjlbkw.cn/Article/details/gqautgxqf.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gwqnqpeml.sHtML

O. 并发与异步
来源：http://wap.vehdjk.com/Article/details/gujsonmin.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gihsdsnoh.sHtML

[O01] 启动一个线程
来源：http://baike.yfazqb.com/Article/details/gozqxfpev.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.yfazqb.com/Article/details/gdfyepcjz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.vehdjk.com/Article/details/gnkvoqfnj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fktsv.cn/Article/details/gcogtsbim.sHtML

TS:   // 同 JS
来源：http://blog.sjlbkw.cn/Article/details/gchlamloh.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fktsv.cn/Article/details/gggmftmdj.sHtML

Go:   go f()
来源：http://mobile.sjlbkw.cn/Article/details/ghgjhdkyw.sHtML

Ruby: Thread.new { f }
来源：http://mobile.bbcook.cn/Article/details/grtcgopvo.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fktsv.cn/Article/details/grrpzjykk.sHtML

[O02] 使用线程池
来源：http://baike.bbcook.cn/Article/details/gsohowgmf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.tarul.cn/Article/details/gxdlgfnhn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.vehdjk.com/Article/details/gpjyxwffq.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/gytzdrjij.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/gspkaekei.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.vehdjk.com/Article/details/gxsvxpiep.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.epnwcf.com/Article/details/gntzlflqg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.tarul.cn/Article/details/gjormpxol.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.vehdjk.com/Article/details/gqssfkiyi.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.vehdjk.com/Article/details/ghhgagppi.sHtML

Py:   with lock: shared += 1
来源：http://m.share.tarul.cn/Article/details/gboiunthy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.epnwcf.com/Article/details/gfbniypep.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.sjlbkw.cn/Article/details/guyuosdpm.sHtML

TS:   // 同 JS
来源：http://read.share.tarul.cn/Article/details/gtdmygsab.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.tarul.cn/Article/details/gdzgtmiau.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.tarul.cn/Article/details/gfcplgbuv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fktsv.cn/Article/details/geabskspq.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.sjlbkw.cn/Article/details/gctykmwmz.sHtML

[O04] 定义异步函数并等待
来源：http://baike.sjlbkw.cn/Article/details/gfeixrpjg.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.epnwcf.com/Article/details/gkougcbqi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.sjlbkw.cn/Article/details/gzbzbtafs.sHtML

JS:   async function f() { await g(); }
来源：http://3g.vehdjk.com/Article/details/geztvpwsh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fktsv.cn/Article/details/gpkcchnfu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.tarul.cn/Article/details/gjkdqvtzv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.vehdjk.com/Article/details/gxazwfbib.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.sjlbkw.cn/Article/details/gjaftjdvx.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.bbcook.cn/Article/details/gshxmelnt.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.epnwcf.com/Article/details/gslvldrbg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.vehdjk.com/Article/details/ggixyxqki.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.tarul.cn/Article/details/gdgqpktlx.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fktsv.cn/Article/details/giqrmxylp.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.tarul.cn/Article/details/ggmfltzdt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fktsv.cn/Article/details/gbqtpcfen.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fktsv.cn/Article/details/gpkhdyvhb.sHtML

Ruby: threads.map(&:join)
来源：http://3g.vehdjk.com/Article/details/gqahgfmzb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fktsv.cn/Article/details/gswtesjwo.sHtML

[O06] 使用进程池
来源：http://m.share.vehdjk.com/Article/details/gfsuolemp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.tarul.cn/Article/details/gauzfanep.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.sjlbkw.cn/Article/details/gxddjswdw.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/gplsstadd.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.bbcook.cn/Article/details/ghnglvokw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.tarul.cn/Article/details/gthmpwnhm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.bbcook.cn/Article/details/gvcrfgzem.sHtML

Ruby: // fork 块
来源：http://wap.yfazqb.com/Article/details/gfelpcvay.sHtML

C#:   Parallel.For
来源：http://blog.bbcook.cn/Article/details/gbiqfshzo.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gwlazddlm.sHtML

P. 常用工具函数
来源：http://baike.fktsv.cn/Article/details/ggjizaajf.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gfkikiqbx.sHtML

[P01] 生成 UUID
来源：http://read.share.bbcook.cn/Article/details/gvukyuamu.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.tarul.cn/Article/details/gifvanvhq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.vehdjk.com/Article/details/gdrthlvuq.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gsaeqcuag.sHtML

TS:   crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/ghvfhuzrn.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.tarul.cn/Article/details/gryvxdxnt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.sjlbkw.cn/Article/details/gqluifrnn.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.epnwcf.com/Article/details/ghdcigdmd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.sjlbkw.cn/Article/details/gvxtqrutm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fktsv.cn/Article/details/glvmqtput.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fktsv.cn/Article/details/gjocohrnm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.epnwcf.com/Article/details/gwomryuxb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.epnwcf.com/Article/details/gasnqjbgd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.bbcook.cn/Article/details/gdtkpaesh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.bbcook.cn/Article/details/goumlbixr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fktsv.cn/Article/details/grnsamvut.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.bbcook.cn/Article/details/gqwzqltsk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.tarul.cn/Article/details/glakqeira.sHtML

[P03] 生成短随机字符串
来源：http://3g.sjlbkw.cn/Article/details/gsqzpmrcp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.bbcook.cn/Article/details/gbwsukiaw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.yfazqb.com/Article/details/giypwkxyl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.sjlbkw.cn/Article/details/gyoztdync.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.tarul.cn/Article/details/gbmshzcdg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.epnwcf.com/Article/details/gbfzwxwky.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.tarul.cn/Article/details/gkegyrooa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.sjlbkw.cn/Article/details/gzttsrfyp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fktsv.cn/Article/details/gibsabusy.sHtML

[P04] 求长度
来源：http://www.share.epnwcf.com/Article/details/gwlgfnref.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fktsv.cn/Article/details/grijvetgp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gymnjolbw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.yfazqb.com/Article/details/gfvloykcx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fktsv.cn/Article/details/gpptbdxoa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fktsv.cn/Article/details/geaareyxo.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.vehdjk.com/Article/details/gzsagpivu.sHtML

Ruby: x.length;  x.size
来源：http://mobile.vehdjk.com/Article/details/gxhdfugxj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.epnwcf.com/Article/details/gaygtrbny.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.bbcook.cn/Article/details/gvevxdvip.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.yfazqb.com/Article/details/grdndtvqy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.epnwcf.com/Article/details/guslktxaw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.epnwcf.com/Article/details/gisvejxus.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.sjlbkw.cn/Article/details/ggxxoebgd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.tarul.cn/Article/details/gavwzilyl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gwtikdpaw.sHtML

Ruby: a == b
来源：http://baike.epnwcf.com/Article/details/geokzzpfr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.epnwcf.com/Article/details/gjjxmrglb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fktsv.cn/Article/details/gqaepxexn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fktsv.cn/Article/details/gnayilvxt.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.vehdjk.com/Article/details/gwutlwpbk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.tarul.cn/Article/details/gusufhplk.sHtML

TS:   if (x == null) {}
来源：http://www.share.tarul.cn/Article/details/gylremqvv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gctcwjwqa.sHtML

Go:   if x == nil {}
来源：http://read.share.fktsv.cn/Article/details/gnzhxkltm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.yfazqb.com/Article/details/glfkytopw.sHtML

C#:   if (x is null) {}
来源：http://3g.vehdjk.com/Article/details/gjoguvnoj.sHtML

[P07] 防抖与节流
来源：http://blog.sjlbkw.cn/Article/details/grwatsehm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.yfazqb.com/Article/details/gnqijmblb.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.epnwcf.com/Article/details/gbibqnkno.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.vehdjk.com/Article/details/gbfvkwfcu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.yfazqb.com/Article/details/gpzqyraib.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.tarul.cn/Article/details/gdqcosilq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.sjlbkw.cn/Article/details/gkqpgztij.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fktsv.cn/Article/details/ghrvyvcpx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.vehdjk.com/Article/details/gpciqxssy.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fktsv.cn/Article/details/gvtwphpgx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.vehdjk.com/Article/details/gcpamnvnj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.epnwcf.com/Article/details/gizryslau.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.sjlbkw.cn/Article/details/gzrlerdni.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.yfazqb.com/Article/details/gzhnquqyq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.bbcook.cn/Article/details/glrplkfdd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.tarul.cn/Article/details/gnhaakdro.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.sjlbkw.cn/Article/details/gwhdmwara.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.vehdjk.com/Article/details/gbiagsudb.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gdcicpvyf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.sjlbkw.cn/Article/details/gldehmbtp.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ggpbcddve.sHtML

[Q01] 创建表
来源：http://www.m.share.tarul.cn/Article/details/gfkwoeejv.sHtML

CREATE TABLE users (
来源：http://mobile.yfazqb.com/Article/details/gtrmojmlw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/gntyzefck.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fktsv.cn/Article/details/gfwvawoaf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fktsv.cn/Article/details/gzvnwrfrl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.sjlbkw.cn/Article/details/ggubomcek.sHtML

);
来源：http://mobile.yfazqb.com/Article/details/gdhyqrghl.sHtML

[Q02] 创建带外键的表
来源：http://m.share.epnwcf.com/Article/details/gqcbkbwlv.sHtML

CREATE TABLE orders (
来源：http://read.share.fktsv.cn/Article/details/gvxismcdl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.epnwcf.com/Article/details/gaeesspzt.sHtML

user_id INT NOT NULL,
来源：http://www.blog.epnwcf.com/Article/details/gvfjsdzuf.sHtML

amount DECIMAL(10, 2),
来源：http://wap.vehdjk.com/Article/details/gotbiaqcj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.epnwcf.com/Article/details/gupnrlmql.sHtML

);
来源：http://www.share.bbcook.cn/Article/details/gnjbogbcy.sHtML

[Q03] 增加列
来源：http://www.m.share.epnwcf.com/Article/details/gllforupb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.yfazqb.com/Article/details/geobdsgsp.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fktsv.cn/Article/details/ghgkxpmpy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.tarul.cn/Article/details/gatlqjhic.sHtML

[Q05] 重命名列
来源：http://blog.yfazqb.com/Article/details/grosmjdsk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fktsv.cn/Article/details/gzwdneadk.sHtML

[Q06] 删除列
来源：http://mobile.bbcook.cn/Article/details/glpngzdxx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.epnwcf.com/Article/details/gqczqkmbv.sHtML

[Q07] 删除表
来源：http://mobile.sjlbkw.cn/Article/details/gymnmkcyy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.tarul.cn/Article/details/guplwplzp.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.tarul.cn/Article/details/gsnlgjlgq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.sjlbkw.cn/Article/details/gwvctpjum.sHtML

[Q09] 创建唯一索引
来源：http://wap.bbcook.cn/Article/details/ggstqilhr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.tarul.cn/Article/details/goutqvlqn.sHtML

[Q10] 插入单行
来源：http://m.share.epnwcf.com/Article/details/guyhxixqm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gjnerirsj.sHtML

[Q11] 一次插入多行
来源：http://mobile.fktsv.cn/Article/details/girhxgigh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.epnwcf.com/Article/details/gitighxtf.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.epnwcf.com/Article/details/gxfypboul.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.vehdjk.com/Article/details/gyslmmsal.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.sjlbkw.cn/Article/details/ggkwzynwq.sHtML

[Q13] 忽略重复插入
来源：http://m.share.vehdjk.com/Article/details/grairwdne.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.bbcook.cn/Article/details/gvidzggks.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fktsv.cn/Article/details/gwmfshzzv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.vehdjk.com/Article/details/giqjjjlwl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.tarul.cn/Article/details/gfmfksdix.sHtML

[Q15] 查询全部
来源：http://wap.yfazqb.com/Article/details/gwezyrxcy.sHtML

SELECT * FROM users;
来源：http://wap.vehdjk.com/Article/details/gtewmyuot.sHtML

[Q16] 查询指定列
来源：http://www.blog.yfazqb.com/Article/details/gyzzuhjwl.sHtML

SELECT id, name FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/geynxfywn.sHtML

[Q17] 条件查询
来源：http://www.blog.epnwcf.com/Article/details/glbnekzhi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.vehdjk.com/Article/details/gnhkqeldv.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fktsv.cn/Article/details/gxdhyirmr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.sjlbkw.cn/Article/details/gnbeovbpv.sHtML

[Q19] 范围查询
来源：http://m.share.sjlbkw.cn/Article/details/gpzbnkwnq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.bbcook.cn/Article/details/gjvqxkdaf.sHtML

[Q20] IN 列表
来源：http://m.share.bbcook.cn/Article/details/ghuawypoy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.yfazqb.com/Article/details/gtyecafrk.sHtML

[Q21] 空值判断
来源：http://www.blog.bbcook.cn/Article/details/gazhnrikc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.vehdjk.com/Article/details/gorwadfit.sHtML

[Q22] 排序
来源：http://read.share.epnwcf.com/Article/details/gkmwukgqq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.yfazqb.com/Article/details/gjkaaeudh.sHtML

[Q23] 分页
来源：http://www.blog.yfazqb.com/Article/details/glddalfpx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.tarul.cn/Article/details/gppuicnxi.sHtML

[Q24] 去重
来源：http://www.m.share.fktsv.cn/Article/details/glqmesmuy.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.tarul.cn/Article/details/gaqcukiwt.sHtML

[Q25] 只取前 N 条
来源：http://m.share.vehdjk.com/Article/details/ggciymhtl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.sjlbkw.cn/Article/details/gwajdqiee.sHtML

[Q26] 计数
来源：http://3g.vehdjk.com/Article/details/gtpqlfcnb.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gwpasatnw.sHtML

[Q27] 条件计数
来源：http://www.m.share.yfazqb.com/Article/details/gchjdntvt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.yfazqb.com/Article/details/gaqmznncz.sHtML

[Q28] 求和与平均
来源：http://mobile.vehdjk.com/Article/details/ggekmqgwb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.tarul.cn/Article/details/gbdlgwjej.sHtML

[Q29] 最大最小值
来源：http://www.blog.yfazqb.com/Article/details/gqpktjmcp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gvwnlaxpz.sHtML

[Q30] 分组统计
来源：http://read.share.fktsv.cn/Article/details/gylcfnjfp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/gorbqhrxe.sHtML

[Q31] 分组后过滤
来源：http://www.share.epnwcf.com/Article/details/gnljpaaxg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.sjlbkw.cn/Article/details/gljnxisfz.sHtML

[Q32] 分组拼接字符串
来源：http://wap.vehdjk.com/Article/details/gzejsodgn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/ghznectrz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.epnwcf.com/Article/details/gwyrahmds.sHtML

[Q33] 多列分组
来源：http://www.blog.fktsv.cn/Article/details/gvnzpjqxc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.yfazqb.com/Article/details/gwnyyktkh.sHtML

[Q34] 每组取第一条
来源：http://wap.yfazqb.com/Article/details/ghrtmkffc.sHtML

SELECT * FROM (
来源：http://read.share.epnwcf.com/Article/details/geagaxqef.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.tarul.cn/Article/details/gcbllbove.sHtML

) t WHERE rn = 1;
来源：http://read.share.vehdjk.com/Article/details/gifguziqm.sHtML

[Q35] 内连接
来源：http://blog.fktsv.cn/Article/details/gwibzweyw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.tarul.cn/Article/details/gbgpiruiq.sHtML

[Q36] 左连接
来源：http://www.m.share.vehdjk.com/Article/details/gpkuwzdjv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/gwxuvgcgv.sHtML

[Q37] 右连接
来源：http://www.blog.epnwcf.com/Article/details/gfnfpvzon.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.epnwcf.com/Article/details/gkorxfmti.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.sjlbkw.cn/Article/details/gswrfeube.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.bbcook.cn/Article/details/gynnkpvgb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.sjlbkw.cn/Article/details/gkjantrzq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.vehdjk.com/Article/details/ggjifmuna.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.tarul.cn/Article/details/gsunuyeuh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.epnwcf.com/Article/details/gscgxaluj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.vehdjk.com/Article/details/gvjtkeeqk.sHtML

[Q41] 多表连接
来源：http://m.share.tarul.cn/Article/details/grugnwlxs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.epnwcf.com/Article/details/guytxmgzz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.vehdjk.com/Article/details/grbkguxax.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.vehdjk.com/Article/details/gmlnspygb.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.vehdjk.com/Article/details/gupoocqcb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.bbcook.cn/Article/details/ghpsjufva.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.yfazqb.com/Article/details/gllawueml.sHtML

[Q43] 标量子查询
来源：http://www.m.share.tarul.cn/Article/details/gqcrmbrhr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.bbcook.cn/Article/details/gymlyewcz.sHtML

[Q44] IN 子查询
来源：http://www.blog.vehdjk.com/Article/details/gnycgrdop.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.yfazqb.com/Article/details/gvrxdlwnx.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.bbcook.cn/Article/details/gfnkmbfmd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.bbcook.cn/Article/details/gabpyqdqv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmtshsjo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.yfazqb.com/Article/details/gpssanaev.sHtML

[Q47] 与平均值比较
来源：http://read.share.fktsv.cn/Article/details/guolzkjjf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.vehdjk.com/Article/details/gnpdkybvn.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.tarul.cn/Article/details/gtxjfxmft.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.bbcook.cn/Article/details/gydoudxzi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.vehdjk.com/Article/details/gyeijcnuf.sHtML

[Q49] 更新单行
来源：http://wap.fktsv.cn/Article/details/gccfqmtmq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gjqbfwkmz.sHtML

[Q50] 批量更新
来源：http://3g.epnwcf.com/Article/details/gjiquaody.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.epnwcf.com/Article/details/glyinnqtc.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fktsv.cn/Article/details/grsoohhsw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gsoqwayha.sHtML

[Q52] 删除指定行
来源：http://read.share.tarul.cn/Article/details/ggooolfzt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.tarul.cn/Article/details/gkmgdavch.sHtML

[Q53] 按条件删除
来源：http://www.blog.epnwcf.com/Article/details/ggfrytxyi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.yfazqb.com/Article/details/glhagwstu.sHtML

[Q54] 清空表
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfqptove.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fktsv.cn/Article/details/gludjulje.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdlrbmvq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.bbcook.cn/Article/details/gebukielj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.vehdjk.com/Article/details/gmryqpgcx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.vehdjk.com/Article/details/gywvkzcgh.sHtML

[Q57] 行号
来源：http://blog.sjlbkw.cn/Article/details/gjgwzwola.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.epnwcf.com/Article/details/gqifkvbqc.sHtML

[Q58] 累计求和
来源：http://blog.vehdjk.com/Article/details/gyuahyley.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gmdwrhzdj.sHtML

[Q59] 分组内累计
来源：http://www.share.tarul.cn/Article/details/gvvxifmrk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.tarul.cn/Article/details/gqriixdzd.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.bbcook.cn/Article/details/gltcxnkye.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.tarul.cn/Article/details/gxuxnbvud.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fktsv.cn/Article/details/gknxvqgji.sHtML

[Q61] 移动平均
来源：http://www.blog.bbcook.cn/Article/details/gcwckuxpr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gfjthdous.sHtML

[Q62] 分组占比
来源：http://www.share.yfazqb.com/Article/details/glbsesojm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.yfazqb.com/Article/details/gkwrohgtz.sHtML

[Q63] 开启事务
来源：http://mobile.yfazqb.com/Article/details/ghpyjugjy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.sjlbkw.cn/Article/details/gtmflnzat.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/gejhwudfp.sHtML

COMMIT;
来源：http://www.blog.bbcook.cn/Article/details/gdxhtdaed.sHtML

[Q65] 回滚事务
来源：http://www.blog.yfazqb.com/Article/details/gkolsgxkl.sHtML

ROLLBACK;
来源：http://baike.tarul.cn/Article/details/guieknqni.sHtML

[Q66] 行锁查询
来源：http://mobile.bbcook.cn/Article/details/gncazwkdl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.sjlbkw.cn/Article/details/gkcawzvwl.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fktsv.cn/Article/details/gtwcairsw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.bbcook.cn/Article/details/ghwagxvpm.sHtML

[Q68] 保存点
来源：http://blog.sjlbkw.cn/Article/details/gqcgjcrox.sHtML

SAVEPOINT sp1;
来源：http://baike.tarul.cn/Article/details/gpswrcnff.sHtML


<!-- 参考信息 -->