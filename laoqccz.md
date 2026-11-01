代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fktsv.cn/Article/details/gebwjcofy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.sjlbkw.cn/Article/details/gzhlzknum.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.bbcook.cn/Article/details/gmcuxbvws.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.sjlbkw.cn/Article/details/gatdvkson.sHtML

PHP:  // 手写递归函数
来源：http://baike.bbcook.cn/Article/details/gxfplotiq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.yfazqb.com/Article/details/gjaxtxmbc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/gxqkeiuft.sHtML

Java: // 手写递归
来源：http://3g.vehdjk.com/Article/details/guljgvesa.sHtML

Go:   // 手写递归
来源：http://baike.sjlbkw.cn/Article/details/gennsldve.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.bbcook.cn/Article/details/gvwyhghpe.sHtML

C#:   // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gxwunnvka.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fktsv.cn/Article/details/gojwtvoyb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.epnwcf.com/Article/details/gfdoradcy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.yfazqb.com/Article/details/gtrbbqpyy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/gbrzkbtff.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.vehdjk.com/Article/details/gzqiebump.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.vehdjk.com/Article/details/gisaybiln.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.sjlbkw.cn/Article/details/gccfryiev.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.epnwcf.com/Article/details/grqaftsls.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.sjlbkw.cn/Article/details/grorkcfwz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gsxwiluin.sHtML

O. 并发与异步
来源：http://www.blog.sjlbkw.cn/Article/details/ggenoyoea.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gqokvpdvs.sHtML

[O01] 启动一个线程
来源：http://blog.bbcook.cn/Article/details/ghjyfjsbd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.epnwcf.com/Article/details/gabmlhfsq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.epnwcf.com/Article/details/grsbqrpfn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fktsv.cn/Article/details/giagnumqa.sHtML

TS:   // 同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gqalzkuho.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.yfazqb.com/Article/details/gcwemudnx.sHtML

Go:   go f()
来源：http://wap.yfazqb.com/Article/details/gjocsuwpi.sHtML

Ruby: Thread.new { f }
来源：http://wap.yfazqb.com/Article/details/gblsdyxci.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.epnwcf.com/Article/details/gboryuzbr.sHtML

[O02] 使用线程池
来源：http://3g.fktsv.cn/Article/details/gxgxbvcdh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.sjlbkw.cn/Article/details/gihukiwdk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fktsv.cn/Article/details/gvkwvzqyi.sHtML

JS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/gagogqviy.sHtML

TS:   // worker_threads 线程池
来源：http://blog.vehdjk.com/Article/details/gwdtqyxej.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.vehdjk.com/Article/details/gfmaceplf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.epnwcf.com/Article/details/gioeqgcvm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.sjlbkw.cn/Article/details/gypixmznf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.tarul.cn/Article/details/gxrnggvxr.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fktsv.cn/Article/details/gvsepqqsy.sHtML

Py:   with lock: shared += 1
来源：http://baike.tarul.cn/Article/details/grcvnhpes.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.vehdjk.com/Article/details/gwoaivizz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.sjlbkw.cn/Article/details/gtuzbxdix.sHtML

TS:   // 同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gvpiplgra.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gboqissne.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.vehdjk.com/Article/details/gdyhukhao.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.yfazqb.com/Article/details/gukghnbkz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.sjlbkw.cn/Article/details/gubfxwzux.sHtML

[O04] 定义异步函数并等待
来源：http://blog.tarul.cn/Article/details/gadwfskuk.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fktsv.cn/Article/details/ghhifneua.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fktsv.cn/Article/details/gxwfmliss.sHtML

JS:   async function f() { await g(); }
来源：http://baike.tarul.cn/Article/details/gjeursccm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.epnwcf.com/Article/details/gmdggyire.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.epnwcf.com/Article/details/gprozdmaw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.sjlbkw.cn/Article/details/gzqokljct.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.bbcook.cn/Article/details/geehpiloh.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.tarul.cn/Article/details/glybedmtd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.vehdjk.com/Article/details/gekrrievt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.yfazqb.com/Article/details/gwqktqwma.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.bbcook.cn/Article/details/gyotwxldu.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.tarul.cn/Article/details/gttzehgpp.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.tarul.cn/Article/details/gyabfgbhz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.epnwcf.com/Article/details/ghiyamjcr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.epnwcf.com/Article/details/gsbbpdzjv.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/gyhqvebvm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.vehdjk.com/Article/details/gnbmwgogo.sHtML

[O06] 使用进程池
来源：http://www.blog.vehdjk.com/Article/details/gkravctbe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.yfazqb.com/Article/details/gbqhqbmjz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.epnwcf.com/Article/details/gyiqzeykz.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/gcfkyqmfq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.epnwcf.com/Article/details/glhxuzmtk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.sjlbkw.cn/Article/details/ghcauyuyk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.epnwcf.com/Article/details/gjezdktiy.sHtML

Ruby: // fork 块
来源：http://3g.yfazqb.com/Article/details/gtdawbmib.sHtML

C#:   Parallel.For
来源：http://mobile.vehdjk.com/Article/details/gyompslig.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gaclglony.sHtML

P. 常用工具函数
来源：http://blog.sjlbkw.cn/Article/details/gothqvudo.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gwswijwmg.sHtML

[P01] 生成 UUID
来源：http://m.share.fktsv.cn/Article/details/ggzkdnrdr.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.epnwcf.com/Article/details/gapkxtqoq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.epnwcf.com/Article/details/gwxsxtjlq.sHtML

JS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gfwxyuwag.sHtML

TS:   crypto.randomUUID()
来源：http://3g.bbcook.cn/Article/details/gvjltyxsy.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.epnwcf.com/Article/details/gqhijkbzb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.epnwcf.com/Article/details/gaharstph.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.bbcook.cn/Article/details/gwxoteovn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.vehdjk.com/Article/details/gjtwzqzjj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fktsv.cn/Article/details/gmtakrayx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fktsv.cn/Article/details/gsalxxzrc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.vehdjk.com/Article/details/gljjixnmq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.vehdjk.com/Article/details/gszanzopb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fktsv.cn/Article/details/guqzyyvnl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.vehdjk.com/Article/details/gxeqcznej.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.bbcook.cn/Article/details/gficwakqp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.sjlbkw.cn/Article/details/gufvgklxz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fktsv.cn/Article/details/goqaezmbo.sHtML

[P03] 生成短随机字符串
来源：http://mobile.epnwcf.com/Article/details/gozgpjnan.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.vehdjk.com/Article/details/gglqcwele.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.sjlbkw.cn/Article/details/gboconxzj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/gxsujklmt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.sjlbkw.cn/Article/details/gjqwebfak.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.tarul.cn/Article/details/ggauxhqkp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.vehdjk.com/Article/details/gebivlaec.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.tarul.cn/Article/details/guxlpdxte.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/gapxunyoc.sHtML

[P04] 求长度
来源：http://www.share.sjlbkw.cn/Article/details/gpfrilqbm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.epnwcf.com/Article/details/gozqgvqbv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gwquynnpm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fktsv.cn/Article/details/gtivjjzud.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.tarul.cn/Article/details/gudglipau.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.bbcook.cn/Article/details/gyciizpdk.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.vehdjk.com/Article/details/grqtwyukl.sHtML

Ruby: x.length;  x.size
来源：http://mobile.tarul.cn/Article/details/gtwwmyyyn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.yfazqb.com/Article/details/guhpgktwk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fktsv.cn/Article/details/gnzgxukwn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.epnwcf.com/Article/details/gohpjojbb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.epnwcf.com/Article/details/gtnagptla.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.yfazqb.com/Article/details/gxxcuktlw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.sjlbkw.cn/Article/details/gayfhyvrt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.bbcook.cn/Article/details/grsplubvr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.epnwcf.com/Article/details/gcueuwega.sHtML

Ruby: a == b
来源：http://3g.fktsv.cn/Article/details/gdqxwdxfw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.epnwcf.com/Article/details/gogvpvtum.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.bbcook.cn/Article/details/gcrrqjqfn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.epnwcf.com/Article/details/gdzflhhhp.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.yfazqb.com/Article/details/gmkcvkiae.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.vehdjk.com/Article/details/glmistovy.sHtML

TS:   if (x == null) {}
来源：http://www.share.bbcook.cn/Article/details/gbmsdjmhl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.yfazqb.com/Article/details/ggsdnzalm.sHtML

Go:   if x == nil {}
来源：http://www.share.bbcook.cn/Article/details/garedvwlm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fktsv.cn/Article/details/gwdafsfcj.sHtML

C#:   if (x is null) {}
来源：http://m.share.vehdjk.com/Article/details/gvmiqiyoq.sHtML

[P07] 防抖与节流
来源：http://m.share.sjlbkw.cn/Article/details/gaqxyyjvk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.bbcook.cn/Article/details/gzacbmkwg.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.epnwcf.com/Article/details/glxvzaukc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/gwphsrhwm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.yfazqb.com/Article/details/gguedrfto.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.yfazqb.com/Article/details/gtswseeqx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fktsv.cn/Article/details/gidrzvsni.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.yfazqb.com/Article/details/gfbshsmjg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fktsv.cn/Article/details/gktlqsidv.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.tarul.cn/Article/details/gvdvyvmka.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fktsv.cn/Article/details/glsjgfhyw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.yfazqb.com/Article/details/gcjtjmxne.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.bbcook.cn/Article/details/grrczifyb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.bbcook.cn/Article/details/gvgevflzm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.yfazqb.com/Article/details/gtgwebrdl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.tarul.cn/Article/details/gmeirlhrw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.epnwcf.com/Article/details/gqtrwnyfi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.epnwcf.com/Article/details/gddxqtosg.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gqytkqjtm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.tarul.cn/Article/details/gdptnfxef.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gixdenruo.sHtML

[Q01] 创建表
来源：http://3g.sjlbkw.cn/Article/details/govgvwmgz.sHtML

CREATE TABLE users (
来源：http://baike.bbcook.cn/Article/details/gxjvkhlhi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.tarul.cn/Article/details/gukqmzlbp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.bbcook.cn/Article/details/gbqpgfnpt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fktsv.cn/Article/details/gkcttlayo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.yfazqb.com/Article/details/geyqrtsmt.sHtML

);
来源：http://mobile.sjlbkw.cn/Article/details/gpfnaldie.sHtML

[Q02] 创建带外键的表
来源：http://wap.epnwcf.com/Article/details/ghbkbwrhx.sHtML

CREATE TABLE orders (
来源：http://read.share.yfazqb.com/Article/details/grihaoslh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.tarul.cn/Article/details/gdjkukyjt.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.bbcook.cn/Article/details/grfyjbbwb.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.epnwcf.com/Article/details/gvedaljjd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.epnwcf.com/Article/details/ghdyhexlo.sHtML

);
来源：http://3g.tarul.cn/Article/details/gknepmvwh.sHtML

[Q03] 增加列
来源：http://www.m.share.vehdjk.com/Article/details/gmsyuhqpk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.yfazqb.com/Article/details/gzxopvqqx.sHtML

[Q04] 修改列类型
来源：http://read.share.yfazqb.com/Article/details/gfmcgzfkt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.vehdjk.com/Article/details/gilcqszjz.sHtML

[Q05] 重命名列
来源：http://blog.vehdjk.com/Article/details/guodxsyxe.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.tarul.cn/Article/details/gkyhfvius.sHtML

[Q06] 删除列
来源：http://www.blog.tarul.cn/Article/details/gatigvwqd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.epnwcf.com/Article/details/gjvyejlif.sHtML

[Q07] 删除表
来源：http://www.blog.sjlbkw.cn/Article/details/ggcegfehe.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.bbcook.cn/Article/details/gbjpqeldn.sHtML

[Q08] 创建普通索引
来源：http://www.share.bbcook.cn/Article/details/ghoklhuqp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/gqvjabdlw.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fktsv.cn/Article/details/gcdcttzee.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/gphiqcced.sHtML

[Q10] 插入单行
来源：http://read.share.yfazqb.com/Article/details/gvvktcxok.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.vehdjk.com/Article/details/gyewznpjp.sHtML

[Q11] 一次插入多行
来源：http://blog.fktsv.cn/Article/details/gjauifosl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/gzikzvzyh.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.yfazqb.com/Article/details/ggxyegezi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.sjlbkw.cn/Article/details/gtdemijix.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.bbcook.cn/Article/details/ghdocfgmd.sHtML

[Q13] 忽略重复插入
来源：http://www.share.yfazqb.com/Article/details/gwjrdbwbx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.bbcook.cn/Article/details/gcotnomfg.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fktsv.cn/Article/details/gbqzhgqth.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.tarul.cn/Article/details/gyytvawbo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.yfazqb.com/Article/details/gvhktjcmu.sHtML

[Q15] 查询全部
来源：http://3g.fktsv.cn/Article/details/gvnfqxveq.sHtML

SELECT * FROM users;
来源：http://www.share.yfazqb.com/Article/details/glkbhkbim.sHtML

[Q16] 查询指定列
来源：http://blog.bbcook.cn/Article/details/gqnwrkavk.sHtML

SELECT id, name FROM users;
来源：http://m.share.tarul.cn/Article/details/gsiqdrwei.sHtML

[Q17] 条件查询
来源：http://www.share.tarul.cn/Article/details/grpzdnasl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.vehdjk.com/Article/details/gkgdoqhlt.sHtML

[Q18] 模糊匹配
来源：http://wap.tarul.cn/Article/details/gvzkoggsd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.tarul.cn/Article/details/gkdpkjknp.sHtML

[Q19] 范围查询
来源：http://blog.sjlbkw.cn/Article/details/gmdsrvhrt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.bbcook.cn/Article/details/gftuanjvu.sHtML

[Q20] IN 列表
来源：http://wap.epnwcf.com/Article/details/ggikjitzr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.sjlbkw.cn/Article/details/gqnveyolp.sHtML

[Q21] 空值判断
来源：http://m.share.tarul.cn/Article/details/gwdqsqbof.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.tarul.cn/Article/details/ggyofgeyg.sHtML

[Q22] 排序
来源：http://wap.vehdjk.com/Article/details/gmgmdyrlf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.epnwcf.com/Article/details/gukowshxh.sHtML

[Q23] 分页
来源：http://mobile.vehdjk.com/Article/details/gzftphvgu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.sjlbkw.cn/Article/details/gtzosldxa.sHtML

[Q24] 去重
来源：http://blog.fktsv.cn/Article/details/gdthcatby.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.epnwcf.com/Article/details/gihzuwbue.sHtML

[Q25] 只取前 N 条
来源：http://blog.vehdjk.com/Article/details/grekaqdoa.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.epnwcf.com/Article/details/givpzfrlg.sHtML

[Q26] 计数
来源：http://wap.epnwcf.com/Article/details/gpaqcisti.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gahbgemaa.sHtML

[Q27] 条件计数
来源：http://3g.tarul.cn/Article/details/grbwomuac.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.tarul.cn/Article/details/gnvuuvntn.sHtML

[Q28] 求和与平均
来源：http://m.share.tarul.cn/Article/details/gdlewtwxm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gvrrbuigb.sHtML

[Q29] 最大最小值
来源：http://blog.fktsv.cn/Article/details/gnovejrdb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.epnwcf.com/Article/details/gxlrovfwd.sHtML

[Q30] 分组统计
来源：http://mobile.tarul.cn/Article/details/gumtxjxbt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.tarul.cn/Article/details/ghuuxckcv.sHtML

[Q31] 分组后过滤
来源：http://m.share.yfazqb.com/Article/details/gtorwuphm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.bbcook.cn/Article/details/gkzggmhnn.sHtML

[Q32] 分组拼接字符串
来源：http://baike.vehdjk.com/Article/details/gyjrjtiys.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/gktkajvug.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.tarul.cn/Article/details/gwmmzopml.sHtML

[Q33] 多列分组
来源：http://blog.tarul.cn/Article/details/gklhrtaym.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.epnwcf.com/Article/details/ggqrvxerq.sHtML

[Q34] 每组取第一条
来源：http://wap.epnwcf.com/Article/details/gkrimezfx.sHtML

SELECT * FROM (
来源：http://blog.epnwcf.com/Article/details/ghllcwzsp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.tarul.cn/Article/details/gxrsfybiz.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gmqvzauks.sHtML

[Q35] 内连接
来源：http://wap.vehdjk.com/Article/details/gsdsiscjp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fktsv.cn/Article/details/gvcdcesqb.sHtML

[Q36] 左连接
来源：http://blog.bbcook.cn/Article/details/glvisoatu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/gyikgypzv.sHtML

[Q37] 右连接
来源：http://www.m.share.epnwcf.com/Article/details/geaafkgqo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.sjlbkw.cn/Article/details/gyidrigzu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fktsv.cn/Article/details/geuhugibt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fktsv.cn/Article/details/gfbqwpxkg.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.epnwcf.com/Article/details/gpekfmpre.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fktsv.cn/Article/details/gydwpbyjm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fktsv.cn/Article/details/gtuqjphnf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.bbcook.cn/Article/details/gpdzidgrx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.epnwcf.com/Article/details/gbqunwiyg.sHtML

[Q41] 多表连接
来源：http://blog.epnwcf.com/Article/details/guxnxcckc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.epnwcf.com/Article/details/ghgplgbid.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqabwddz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.vehdjk.com/Article/details/gyodmrguc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.yfazqb.com/Article/details/grwuwudqx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.epnwcf.com/Article/details/gtwrwloxo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgcyokah.sHtML

[Q43] 标量子查询
来源：http://m.share.vehdjk.com/Article/details/gvefeqfbu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.yfazqb.com/Article/details/gjwmdandy.sHtML

[Q44] IN 子查询
来源：http://baike.sjlbkw.cn/Article/details/ggrmbglcd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.vehdjk.com/Article/details/gnhjiubcq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fktsv.cn/Article/details/gifurtmco.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.epnwcf.com/Article/details/gkvngwqtf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.tarul.cn/Article/details/gkxygzjvf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.bbcook.cn/Article/details/gykxjrpdx.sHtML

[Q47] 与平均值比较
来源：http://baike.sjlbkw.cn/Article/details/gxizulgvo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.sjlbkw.cn/Article/details/gwbhwabya.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsniguvo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.yfazqb.com/Article/details/gtafktauy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.epnwcf.com/Article/details/gtuaxerwq.sHtML

[Q49] 更新单行
来源：http://www.share.sjlbkw.cn/Article/details/gicskxdfx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.tarul.cn/Article/details/gcvduxwts.sHtML

[Q50] 批量更新
来源：http://read.share.vehdjk.com/Article/details/gipxzwaqq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.tarul.cn/Article/details/gqjnlfsgg.sHtML

[Q51] 用子查询更新
来源：http://www.blog.sjlbkw.cn/Article/details/grrwfsder.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.tarul.cn/Article/details/gzymydpim.sHtML

[Q52] 删除指定行
来源：http://read.share.sjlbkw.cn/Article/details/gowwdirei.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.sjlbkw.cn/Article/details/gsntftndt.sHtML

[Q53] 按条件删除
来源：http://wap.vehdjk.com/Article/details/ggubnlalb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.bbcook.cn/Article/details/gslrzzbvq.sHtML

[Q54] 清空表
来源：http://www.m.share.tarul.cn/Article/details/giygkpsij.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.tarul.cn/Article/details/gkoflvudb.sHtML

[Q55] 排名（并列占位）
来源：http://baike.tarul.cn/Article/details/gsjnembdo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.sjlbkw.cn/Article/details/gcbeldpuh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.epnwcf.com/Article/details/gzwojfrik.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.vehdjk.com/Article/details/gfxigrymi.sHtML

[Q57] 行号
来源：http://baike.fktsv.cn/Article/details/gsjjmofyt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.bbcook.cn/Article/details/gndjronlj.sHtML

[Q58] 累计求和
来源：http://www.blog.yfazqb.com/Article/details/ghhvjinzy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.epnwcf.com/Article/details/gkypevrsz.sHtML

[Q59] 分组内累计
来源：http://3g.yfazqb.com/Article/details/giruvetok.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.bbcook.cn/Article/details/grcynpbev.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.sjlbkw.cn/Article/details/gqvnmprln.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.bbcook.cn/Article/details/gtkflwiwu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fktsv.cn/Article/details/gikehptyq.sHtML

[Q61] 移动平均
来源：http://blog.tarul.cn/Article/details/gqnskabva.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gnnibuahb.sHtML

[Q62] 分组占比
来源：http://m.share.yfazqb.com/Article/details/gnorsyjns.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gfakpwgsd.sHtML


<!-- 参考信息 -->