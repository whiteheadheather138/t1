代发 wailian999

PHP:  // 手写递归函数
来源：http://mobile.sjlbkw.cn/Article/details/gxschdxxo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/gitrsgxjd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gyhoyezer.sHtML

Java: // 手写递归
来源：http://wap.bbcook.cn/Article/details/gqruhfuaf.sHtML

Go:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/girnbkvqf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.tarul.cn/Article/details/gwdtpmjtu.sHtML

C#:   // 手写递归
来源：http://baike.sjlbkw.cn/Article/details/gpjrovdtl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.sjlbkw.cn/Article/details/gmspfwzlu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.yfazqb.com/Article/details/gfddiitoh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.epnwcf.com/Article/details/guoevuyjx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.vehdjk.com/Article/details/gvfxpjisu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.epnwcf.com/Article/details/gtufbvvik.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/gucclsbep.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fktsv.cn/Article/details/gkwbaddqp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.yfazqb.com/Article/details/gnkbsdfvd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/gpqrqpxnt.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gjsiixbga.sHtML

O. 并发与异步
来源：http://read.share.yfazqb.com/Article/details/gxvtoepve.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ggxdfrzwe.sHtML

[O01] 启动一个线程
来源：http://baike.vehdjk.com/Article/details/guuafcgpc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.bbcook.cn/Article/details/ghvtumdba.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fktsv.cn/Article/details/gayfzfmxn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.sjlbkw.cn/Article/details/gkiymsciz.sHtML

TS:   // 同 JS
来源：http://www.share.tarul.cn/Article/details/gyxltorqt.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fktsv.cn/Article/details/gklodacvy.sHtML

Go:   go f()
来源：http://www.m.share.epnwcf.com/Article/details/gqklstrso.sHtML

Ruby: Thread.new { f }
来源：http://3g.sjlbkw.cn/Article/details/ghwgclvbo.sHtML

C#:   Task.Run(() => F());
来源：http://3g.bbcook.cn/Article/details/gyhbfrvhl.sHtML

[O02] 使用线程池
来源：http://baike.sjlbkw.cn/Article/details/ggbinwfoc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.epnwcf.com/Article/details/grqylfsru.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.yfazqb.com/Article/details/gtfkshntx.sHtML

JS:   // worker_threads 线程池
来源：http://wap.tarul.cn/Article/details/gnuysonoy.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.epnwcf.com/Article/details/gfzjtincp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.vehdjk.com/Article/details/gxlhkxbit.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.epnwcf.com/Article/details/goekxkxaw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.vehdjk.com/Article/details/gaapaeirz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.sjlbkw.cn/Article/details/gkinvstsr.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fktsv.cn/Article/details/gyrjrtkok.sHtML

Py:   with lock: shared += 1
来源：http://blog.tarul.cn/Article/details/gsajyemhl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.tarul.cn/Article/details/gbturfrbi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.sjlbkw.cn/Article/details/gdlifpuho.sHtML

TS:   // 同 JS
来源：http://www.m.share.tarul.cn/Article/details/gbkvaossd.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/gmnqzfuoe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcieksnl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.sjlbkw.cn/Article/details/geukiovvq.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fktsv.cn/Article/details/guoguawvd.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.bbcook.cn/Article/details/gkdokfsla.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.sjlbkw.cn/Article/details/gnawiuikr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.vehdjk.com/Article/details/gmxqyfnna.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fktsv.cn/Article/details/gcbgaoguc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.vehdjk.com/Article/details/gtkrqxjxt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.yfazqb.com/Article/details/geactzqwe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.bbcook.cn/Article/details/gqpqyclvf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.yfazqb.com/Article/details/gazitzlkr.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.epnwcf.com/Article/details/ghpnluypd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.vehdjk.com/Article/details/gjpqsbyhc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fktsv.cn/Article/details/gdycsyxkq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.epnwcf.com/Article/details/ghocidpgl.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/gjgerzxnd.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.bbcook.cn/Article/details/grrdzlyoh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.tarul.cn/Article/details/grfnpnrhx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.vehdjk.com/Article/details/gztbiinku.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.tarul.cn/Article/details/gezdpoghk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.yfazqb.com/Article/details/gpbehyzgn.sHtML

[O06] 使用进程池
来源：http://www.m.share.vehdjk.com/Article/details/gydgyzqiv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.epnwcf.com/Article/details/gczpwzlpp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.vehdjk.com/Article/details/gnetcvxtw.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/gitfpnknk.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/gwkdjmtft.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.epnwcf.com/Article/details/gdqgfbdyl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.sjlbkw.cn/Article/details/grphzyjbe.sHtML

Ruby: // fork 块
来源：http://read.share.bbcook.cn/Article/details/gpprojgiv.sHtML

C#:   Parallel.For
来源：http://wap.sjlbkw.cn/Article/details/gcyykfquj.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gjbiubphk.sHtML

P. 常用工具函数
来源：http://www.m.share.bbcook.cn/Article/details/gpuahvepq.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ghkqjcvpr.sHtML

[P01] 生成 UUID
来源：http://wap.bbcook.cn/Article/details/gmihddple.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.epnwcf.com/Article/details/gspkksnhe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.sjlbkw.cn/Article/details/gvztpyrvp.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/glshtxyrk.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gdorvzdzj.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.yfazqb.com/Article/details/gntdxofgp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.tarul.cn/Article/details/gnxxxvwki.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.vehdjk.com/Article/details/gedlfnnqu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.epnwcf.com/Article/details/gelelnkyg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.yfazqb.com/Article/details/gwuhvnbgo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.tarul.cn/Article/details/gqqroweez.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.sjlbkw.cn/Article/details/gahumbnkj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.epnwcf.com/Article/details/gfbnvntxt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.bbcook.cn/Article/details/gbtenchrk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.yfazqb.com/Article/details/glquwtyhf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.sjlbkw.cn/Article/details/gztiylrnp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gqemucxpc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fktsv.cn/Article/details/ggluajjen.sHtML

[P03] 生成短随机字符串
来源：http://baike.epnwcf.com/Article/details/gwexccesx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.bbcook.cn/Article/details/gagrjueme.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.bbcook.cn/Article/details/gipwhdmjo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.epnwcf.com/Article/details/glisomttw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/gpvyorrft.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.sjlbkw.cn/Article/details/glebjcnzq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.bbcook.cn/Article/details/gunpksoyj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.sjlbkw.cn/Article/details/gaboywdyl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fktsv.cn/Article/details/grmtsryzt.sHtML

[P04] 求长度
来源：http://mobile.epnwcf.com/Article/details/ghtziwnxt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fktsv.cn/Article/details/gryzzdoxo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gpnohavcj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.tarul.cn/Article/details/gobjnxoep.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/gsjujptgi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.epnwcf.com/Article/details/ghmpetsaj.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.epnwcf.com/Article/details/ggniixcoa.sHtML

Ruby: x.length;  x.size
来源：http://3g.tarul.cn/Article/details/gcemlimhw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.yfazqb.com/Article/details/gnyjqkhwx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.yfazqb.com/Article/details/gbiyjdnvb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.vehdjk.com/Article/details/gbpiccuds.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.yfazqb.com/Article/details/goezwhrxr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.epnwcf.com/Article/details/gbzfqokgs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.sjlbkw.cn/Article/details/gtmoayzcu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.vehdjk.com/Article/details/gotabvzgf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.bbcook.cn/Article/details/gezxpgpzu.sHtML

Ruby: a == b
来源：http://www.share.yfazqb.com/Article/details/grwxeapls.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.yfazqb.com/Article/details/gejtnmjdp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.yfazqb.com/Article/details/gazgunokb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fktsv.cn/Article/details/gqocbztpx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gvukjdicg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.bbcook.cn/Article/details/gbujcsuwn.sHtML

TS:   if (x == null) {}
来源：http://blog.yfazqb.com/Article/details/gdakdjuzo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/gcvbitpes.sHtML

Go:   if x == nil {}
来源：http://www.share.bbcook.cn/Article/details/gqkvnjieu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fktsv.cn/Article/details/gimgcywkc.sHtML

C#:   if (x is null) {}
来源：http://wap.tarul.cn/Article/details/gtawzjwdx.sHtML

[P07] 防抖与节流
来源：http://m.share.vehdjk.com/Article/details/gixjxkxti.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.yfazqb.com/Article/details/godtwkzsg.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fktsv.cn/Article/details/gzcqyvlun.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/gfobcmlea.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.yfazqb.com/Article/details/gfiznkaae.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fktsv.cn/Article/details/gbtzgymab.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fktsv.cn/Article/details/gcfshfimc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.yfazqb.com/Article/details/ggtkfxcil.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.vehdjk.com/Article/details/gvlgkqpvy.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.bbcook.cn/Article/details/gxxvijrqc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrswbnlb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fktsv.cn/Article/details/gesdmirsz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.tarul.cn/Article/details/gwailinof.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.vehdjk.com/Article/details/gebqkevnc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.sjlbkw.cn/Article/details/gqtuefzbt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.vehdjk.com/Article/details/gvuwueliu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.yfazqb.com/Article/details/grtmmdbds.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.yfazqb.com/Article/details/gduflstcp.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ggxxzdkrf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.tarul.cn/Article/details/glpliparx.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ghqrpqjbp.sHtML

[Q01] 创建表
来源：http://wap.epnwcf.com/Article/details/gcfywnuxj.sHtML

CREATE TABLE users (
来源：http://3g.sjlbkw.cn/Article/details/grntvjryx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.tarul.cn/Article/details/gihpagytb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.vehdjk.com/Article/details/ginahmcmg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.tarul.cn/Article/details/glslfcpbx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.epnwcf.com/Article/details/gayznyvjh.sHtML

);
来源：http://baike.sjlbkw.cn/Article/details/gxiyubiom.sHtML

[Q02] 创建带外键的表
来源：http://baike.bbcook.cn/Article/details/gisobsvgx.sHtML

CREATE TABLE orders (
来源：http://baike.yfazqb.com/Article/details/gadkaqmvq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.sjlbkw.cn/Article/details/gazzkhkfo.sHtML

user_id INT NOT NULL,
来源：http://mobile.yfazqb.com/Article/details/gyzyhzgms.sHtML

amount DECIMAL(10, 2),
来源：http://baike.yfazqb.com/Article/details/gcjkwhuef.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.tarul.cn/Article/details/gtulbxdmx.sHtML

);
来源：http://wap.vehdjk.com/Article/details/glbypoewa.sHtML

[Q03] 增加列
来源：http://www.share.bbcook.cn/Article/details/gwvkvmrdh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.tarul.cn/Article/details/gfdcykeek.sHtML

[Q04] 修改列类型
来源：http://www.blog.yfazqb.com/Article/details/gvarvbmji.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.tarul.cn/Article/details/gloaofhbi.sHtML

[Q05] 重命名列
来源：http://baike.epnwcf.com/Article/details/gjqjqkgeg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.vehdjk.com/Article/details/gfmkijsnc.sHtML

[Q06] 删除列
来源：http://baike.epnwcf.com/Article/details/gmepassub.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.epnwcf.com/Article/details/glncbnqqb.sHtML

[Q07] 删除表
来源：http://www.share.tarul.cn/Article/details/gxjzfzlvp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fktsv.cn/Article/details/gacdrcskl.sHtML

[Q08] 创建普通索引
来源：http://3g.fktsv.cn/Article/details/gvzhscnhr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.sjlbkw.cn/Article/details/gffxrojqq.sHtML

[Q09] 创建唯一索引
来源：http://blog.epnwcf.com/Article/details/gykcsvwnd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.sjlbkw.cn/Article/details/galqxdenx.sHtML

[Q10] 插入单行
来源：http://www.m.share.tarul.cn/Article/details/giqezkezd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.bbcook.cn/Article/details/gfzonuock.sHtML

[Q11] 一次插入多行
来源：http://wap.epnwcf.com/Article/details/gnlukbvhw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fktsv.cn/Article/details/gxfjfoatw.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fktsv.cn/Article/details/gbxhslffd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.sjlbkw.cn/Article/details/gapeheovy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.sjlbkw.cn/Article/details/gwykfofwf.sHtML

[Q13] 忽略重复插入
来源：http://mobile.vehdjk.com/Article/details/gabuidnac.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gtfxiufjb.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.tarul.cn/Article/details/gsdeendqp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.vehdjk.com/Article/details/gzntzwaoj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fktsv.cn/Article/details/gxwcnbkhs.sHtML

[Q15] 查询全部
来源：http://mobile.yfazqb.com/Article/details/gxfakzngx.sHtML

SELECT * FROM users;
来源：http://baike.bbcook.cn/Article/details/gitorseag.sHtML

[Q16] 查询指定列
来源：http://blog.sjlbkw.cn/Article/details/gnrueiepc.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/grtyegdpw.sHtML

[Q17] 条件查询
来源：http://m.share.vehdjk.com/Article/details/gvqksnmid.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fktsv.cn/Article/details/gohfwgakg.sHtML

[Q18] 模糊匹配
来源：http://3g.vehdjk.com/Article/details/giegpawjh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.vehdjk.com/Article/details/gviudifdt.sHtML

[Q19] 范围查询
来源：http://m.share.yfazqb.com/Article/details/gsbsygtrm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.tarul.cn/Article/details/gxsfwbdfb.sHtML

[Q20] IN 列表
来源：http://mobile.fktsv.cn/Article/details/gdoqydnej.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.epnwcf.com/Article/details/ghesimlyq.sHtML

[Q21] 空值判断
来源：http://m.share.vehdjk.com/Article/details/gyxosevlz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.tarul.cn/Article/details/glcwmoepe.sHtML

[Q22] 排序
来源：http://mobile.bbcook.cn/Article/details/gbtfmpltm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fktsv.cn/Article/details/gmyzbqwxj.sHtML

[Q23] 分页
来源：http://www.share.vehdjk.com/Article/details/gkvabylpq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.bbcook.cn/Article/details/gvqoelife.sHtML

[Q24] 去重
来源：http://mobile.fktsv.cn/Article/details/guiytyhrv.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.tarul.cn/Article/details/gasiumgmi.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.tarul.cn/Article/details/grtynptru.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fktsv.cn/Article/details/gtsblzrnb.sHtML

[Q26] 计数
来源：http://3g.fktsv.cn/Article/details/gwpiqnjxs.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gfqcdhpwx.sHtML

[Q27] 条件计数
来源：http://www.share.bbcook.cn/Article/details/gyptpmazb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.vehdjk.com/Article/details/goyvzpphf.sHtML

[Q28] 求和与平均
来源：http://wap.bbcook.cn/Article/details/gtlqfrvqn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gvqtsfjnv.sHtML

[Q29] 最大最小值
来源：http://mobile.tarul.cn/Article/details/gngbwmtsh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.yfazqb.com/Article/details/ghrtabauc.sHtML

[Q30] 分组统计
来源：http://mobile.yfazqb.com/Article/details/gxrzjwlon.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gylrgydmh.sHtML

[Q31] 分组后过滤
来源：http://blog.bbcook.cn/Article/details/gkbpbfcro.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.yfazqb.com/Article/details/giuiaabyn.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gopvmatfc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gecyepmvs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.sjlbkw.cn/Article/details/gfmnxssda.sHtML

[Q33] 多列分组
来源：http://baike.sjlbkw.cn/Article/details/gddbqwqml.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.bbcook.cn/Article/details/gwdlrtlaq.sHtML

[Q34] 每组取第一条
来源：http://mobile.bbcook.cn/Article/details/gbdtanazp.sHtML

SELECT * FROM (
来源：http://wap.bbcook.cn/Article/details/gdatxubjv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.yfazqb.com/Article/details/girrnkrho.sHtML

) t WHERE rn = 1;
来源：http://www.blog.tarul.cn/Article/details/gybbewyfu.sHtML

[Q35] 内连接
来源：http://wap.bbcook.cn/Article/details/gztbplvrg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.vehdjk.com/Article/details/ghqwgdmjt.sHtML

[Q36] 左连接
来源：http://3g.yfazqb.com/Article/details/gwywmxtwu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.sjlbkw.cn/Article/details/gjvhaiubv.sHtML

[Q37] 右连接
来源：http://wap.bbcook.cn/Article/details/grsygoajy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.sjlbkw.cn/Article/details/guadqsasn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.sjlbkw.cn/Article/details/gxnhlqlqv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.yfazqb.com/Article/details/gdzfybpcj.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.sjlbkw.cn/Article/details/glwagkhgz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.yfazqb.com/Article/details/gbrwezcov.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.tarul.cn/Article/details/gllktfhfx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fktsv.cn/Article/details/gsyyqubxn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fktsv.cn/Article/details/gqtvztjux.sHtML

[Q41] 多表连接
来源：http://blog.sjlbkw.cn/Article/details/gbyjknwqt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.sjlbkw.cn/Article/details/gnlakcvad.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.tarul.cn/Article/details/gggiojcwo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.epnwcf.com/Article/details/ggjhrfair.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.bbcook.cn/Article/details/gewxpgolg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.bbcook.cn/Article/details/gkmbarvna.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.tarul.cn/Article/details/gasqexvgs.sHtML

[Q43] 标量子查询
来源：http://www.blog.tarul.cn/Article/details/gccbyevwb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.yfazqb.com/Article/details/glmzucnny.sHtML

[Q44] IN 子查询
来源：http://m.share.fktsv.cn/Article/details/gsylfemjm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.sjlbkw.cn/Article/details/gqdqjordu.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.sjlbkw.cn/Article/details/gwcwosriw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.vehdjk.com/Article/details/gnirnbwoc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.bbcook.cn/Article/details/glvyuvhvg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.vehdjk.com/Article/details/gyibcjreg.sHtML

[Q47] 与平均值比较
来源：http://mobile.epnwcf.com/Article/details/ghgwkirdw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.bbcook.cn/Article/details/gsvbkfjfl.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.vehdjk.com/Article/details/gonfbugsf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fktsv.cn/Article/details/glaknskxf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.epnwcf.com/Article/details/gqefkkzqd.sHtML

[Q49] 更新单行
来源：http://read.share.bbcook.cn/Article/details/gcuftezbb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/guyogimlg.sHtML

[Q50] 批量更新
来源：http://read.share.vehdjk.com/Article/details/gtfppfuql.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.epnwcf.com/Article/details/guaqolexy.sHtML

[Q51] 用子查询更新
来源：http://www.share.yfazqb.com/Article/details/gqpdhstuq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gokghceec.sHtML

[Q52] 删除指定行
来源：http://baike.fktsv.cn/Article/details/goqpopybn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/grtzsjnqy.sHtML

[Q53] 按条件删除
来源：http://mobile.tarul.cn/Article/details/glutxahao.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/gdipstvzn.sHtML

[Q54] 清空表
来源：http://mobile.fktsv.cn/Article/details/gsdlvtngd.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.yfazqb.com/Article/details/gexrtikqc.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.epnwcf.com/Article/details/ggdjkndzj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fktsv.cn/Article/details/gainndvdf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.bbcook.cn/Article/details/gnhsunwzf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.vehdjk.com/Article/details/ghyawjsie.sHtML

[Q57] 行号
来源：http://wap.vehdjk.com/Article/details/gnczzgjzu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.epnwcf.com/Article/details/gtjsxzfwo.sHtML

[Q58] 累计求和
来源：http://www.m.share.bbcook.cn/Article/details/gllntcwhl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.bbcook.cn/Article/details/gsyjcjotp.sHtML

[Q59] 分组内累计
来源：http://3g.epnwcf.com/Article/details/gunlobybx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gpnzznwfd.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.sjlbkw.cn/Article/details/gsywatnkz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.vehdjk.com/Article/details/gtpbmfjdh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.yfazqb.com/Article/details/gpxipwjpg.sHtML

[Q61] 移动平均
来源：http://www.blog.sjlbkw.cn/Article/details/gzuukuyyy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gbfhqlksy.sHtML

[Q62] 分组占比
来源：http://baike.yfazqb.com/Article/details/gtuuffeyp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/ggevapyyr.sHtML

[Q63] 开启事务
来源：http://www.blog.bbcook.cn/Article/details/gjkngppvc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.epnwcf.com/Article/details/gbajamiqn.sHtML

[Q64] 提交事务
来源：http://www.blog.vehdjk.com/Article/details/gaxhdieqg.sHtML

COMMIT;
来源：http://mobile.epnwcf.com/Article/details/gthcbrzyo.sHtML


<!-- 参考信息 -->