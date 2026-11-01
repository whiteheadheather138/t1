代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fktsv.cn/Article/details/glrjduwpu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.vehdjk.com/Article/details/gjxqezoab.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fktsv.cn/Article/details/gaubngyel.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.epnwcf.com/Article/details/gdnkgnpof.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.vehdjk.com/Article/details/gfhkvcahi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.epnwcf.com/Article/details/genoaesgq.sHtML

[N11] 二叉树中序遍历
来源：http://blog.tarul.cn/Article/details/ggapcdwsk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.yfazqb.com/Article/details/gkimrjuui.sHtML

PHP:  // 手写递归函数
来源：http://read.share.sjlbkw.cn/Article/details/giredlwti.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fktsv.cn/Article/details/ggmjgobfy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/gktxzthoy.sHtML

Java: // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gazdneevm.sHtML

Go:   // 手写递归
来源：http://mobile.tarul.cn/Article/details/gkmvtydvo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fktsv.cn/Article/details/gbrpocjza.sHtML

C#:   // 手写递归
来源：http://mobile.tarul.cn/Article/details/gyqtihthp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.tarul.cn/Article/details/gqiwiaecc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.epnwcf.com/Article/details/ggddxeghf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.epnwcf.com/Article/details/gietodcpb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gevcrxrjd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.yfazqb.com/Article/details/grsmqdtkp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/gzrfoxqfs.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.sjlbkw.cn/Article/details/gvkkaillm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/gnvkvrqvo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.sjlbkw.cn/Article/details/gltwofbgn.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gwolqpovx.sHtML

O. 并发与异步
来源：http://mobile.yfazqb.com/Article/details/gskdeixfx.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gphunvcdh.sHtML

[O01] 启动一个线程
来源：http://mobile.tarul.cn/Article/details/gyejjfrba.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.yfazqb.com/Article/details/gskitxlzz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.bbcook.cn/Article/details/gbvjdrakd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.vehdjk.com/Article/details/gtwpsbbbn.sHtML

TS:   // 同 JS
来源：http://www.m.share.tarul.cn/Article/details/guipfamtq.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.yfazqb.com/Article/details/gzzypgwop.sHtML

Go:   go f()
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdjbotqm.sHtML

Ruby: Thread.new { f }
来源：http://baike.bbcook.cn/Article/details/giwoscwqg.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.yfazqb.com/Article/details/gajfnhair.sHtML

[O02] 使用线程池
来源：http://www.blog.yfazqb.com/Article/details/gudadvajb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.vehdjk.com/Article/details/gcjonugao.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.vehdjk.com/Article/details/godmmkxhl.sHtML

JS:   // worker_threads 线程池
来源：http://wap.tarul.cn/Article/details/gfiawdvbv.sHtML

TS:   // worker_threads 线程池
来源：http://baike.tarul.cn/Article/details/gjrbhsava.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.vehdjk.com/Article/details/gteokgzoh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.yfazqb.com/Article/details/grmnlulxj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.epnwcf.com/Article/details/gcakrqirz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.sjlbkw.cn/Article/details/gmauoctjk.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fktsv.cn/Article/details/gbiujdyrt.sHtML

Py:   with lock: shared += 1
来源：http://m.share.bbcook.cn/Article/details/gdfzvybta.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fktsv.cn/Article/details/gnolbatjq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.yfazqb.com/Article/details/grhbsxjdm.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/gjumhgttq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fktsv.cn/Article/details/gnnubnlrs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fktsv.cn/Article/details/greugtnwb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.yfazqb.com/Article/details/ggozblfns.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.epnwcf.com/Article/details/gwocgmete.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.bbcook.cn/Article/details/gwucdpici.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.tarul.cn/Article/details/gvceikezx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.bbcook.cn/Article/details/gnqwbzukc.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmfpzbns.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.bbcook.cn/Article/details/gsytrgezj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.tarul.cn/Article/details/gsjitlrrw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.yfazqb.com/Article/details/gdeukrnkn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.vehdjk.com/Article/details/gxnnvazxv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtdnnthr.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.yfazqb.com/Article/details/goswwlznh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.epnwcf.com/Article/details/gzwpbezpp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.epnwcf.com/Article/details/grrnxxttk.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/gfqfmigbm.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/gvcvymdyw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fktsv.cn/Article/details/ggbasvqfz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.bbcook.cn/Article/details/gqervyrkr.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.bbcook.cn/Article/details/grdutmhil.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.epnwcf.com/Article/details/grpgclrrd.sHtML

[O06] 使用进程池
来源：http://3g.epnwcf.com/Article/details/gbodjfewr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.epnwcf.com/Article/details/gvpkpcgda.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.vehdjk.com/Article/details/gdjecyagk.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fktsv.cn/Article/details/gjvfaynch.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/gwjbppjgd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.sjlbkw.cn/Article/details/gtzjkrjjx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.epnwcf.com/Article/details/geaknuvhu.sHtML

Ruby: // fork 块
来源：http://www.blog.sjlbkw.cn/Article/details/gccotodca.sHtML

C#:   Parallel.For
来源：http://read.share.epnwcf.com/Article/details/gfdzwxajj.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gljgecfmm.sHtML

P. 常用工具函数
来源：http://mobile.epnwcf.com/Article/details/gbuuagcli.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gulazpyys.sHtML

[P01] 生成 UUID
来源：http://wap.tarul.cn/Article/details/gvhddjhau.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.yfazqb.com/Article/details/gapzbqjgw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fktsv.cn/Article/details/gnxjyivlp.sHtML

JS:   crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/gdhlomich.sHtML

TS:   crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gjsfnnihz.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.tarul.cn/Article/details/gxtqejpcz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.bbcook.cn/Article/details/gvlpfhfjp.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fktsv.cn/Article/details/gxpzfvzxq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.sjlbkw.cn/Article/details/gsflqpdbw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.epnwcf.com/Article/details/goqrwjhyb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.yfazqb.com/Article/details/gqkiferyt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.epnwcf.com/Article/details/ghbeswssu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.sjlbkw.cn/Article/details/gemoypryr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.sjlbkw.cn/Article/details/gdrigmpeq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.tarul.cn/Article/details/gxuuhwnom.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.tarul.cn/Article/details/gqteohyug.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.sjlbkw.cn/Article/details/gdrlpcrkz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.yfazqb.com/Article/details/gkyhxugji.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.tarul.cn/Article/details/gukdpiqbf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.yfazqb.com/Article/details/gqbyqwpxy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.epnwcf.com/Article/details/ggabpackx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.tarul.cn/Article/details/gvrcgzlgo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.epnwcf.com/Article/details/gjxknvflj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.bbcook.cn/Article/details/gjzcozagk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.yfazqb.com/Article/details/gdfwgawil.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.sjlbkw.cn/Article/details/ghlxgkppk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.bbcook.cn/Article/details/gkriruypv.sHtML

[P04] 求长度
来源：http://www.share.vehdjk.com/Article/details/gvnrqjvyt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.bbcook.cn/Article/details/gtvkqgyam.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gueqytwmx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.yfazqb.com/Article/details/gkucxptvi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.yfazqb.com/Article/details/gusvrucnz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.epnwcf.com/Article/details/gdpooxisl.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.bbcook.cn/Article/details/gynqwbdvz.sHtML

Ruby: x.length;  x.size
来源：http://read.share.tarul.cn/Article/details/grbnaxwzg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.sjlbkw.cn/Article/details/gaxovurub.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.tarul.cn/Article/details/gzokbpvjl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.vehdjk.com/Article/details/gpjdlmbhf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fktsv.cn/Article/details/gzxnfkfgs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.vehdjk.com/Article/details/gqsxnerqa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.tarul.cn/Article/details/gbazpkqmi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fktsv.cn/Article/details/gfiypbowx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.yfazqb.com/Article/details/ghycoitfm.sHtML

Ruby: a == b
来源：http://baike.vehdjk.com/Article/details/gyjqsteyq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.bbcook.cn/Article/details/gbbcjrofd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.yfazqb.com/Article/details/gtisqyxaq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.tarul.cn/Article/details/gxpbjobok.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gxvsicnfc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.yfazqb.com/Article/details/gdwerqcuz.sHtML

TS:   if (x == null) {}
来源：http://3g.yfazqb.com/Article/details/gjipzzwre.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.yfazqb.com/Article/details/ggadbxjur.sHtML

Go:   if x == nil {}
来源：http://www.blog.epnwcf.com/Article/details/grsctwhug.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.bbcook.cn/Article/details/gapjyxvug.sHtML

C#:   if (x is null) {}
来源：http://baike.bbcook.cn/Article/details/ghustmmeq.sHtML

[P07] 防抖与节流
来源：http://read.share.fktsv.cn/Article/details/gxdyhuzdc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.vehdjk.com/Article/details/gznxxnjro.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.sjlbkw.cn/Article/details/gzpknzlvo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fktsv.cn/Article/details/gjdoakzvo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gumlskdmx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.vehdjk.com/Article/details/gjpjbhqje.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.tarul.cn/Article/details/gtwvzbmzf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.sjlbkw.cn/Article/details/gekiimtdm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.bbcook.cn/Article/details/gmgomfgno.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.yfazqb.com/Article/details/gojfrmksf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.epnwcf.com/Article/details/gmnukcylx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.epnwcf.com/Article/details/gdphoxowo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.yfazqb.com/Article/details/gfbcjhfns.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gfwrkiufj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.sjlbkw.cn/Article/details/goiqdrqvz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.epnwcf.com/Article/details/gsooofhsn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.sjlbkw.cn/Article/details/gaycoqhnj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.sjlbkw.cn/Article/details/glcrejudm.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/glpursftp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.yfazqb.com/Article/details/gjrzmfybu.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gdymhvlvl.sHtML

[Q01] 创建表
来源：http://wap.yfazqb.com/Article/details/gesrnfcje.sHtML

CREATE TABLE users (
来源：http://read.share.tarul.cn/Article/details/godhqztjo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.yfazqb.com/Article/details/gqnazqcff.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.epnwcf.com/Article/details/gmvsrforf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.sjlbkw.cn/Article/details/guyonbedk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.epnwcf.com/Article/details/gctkufxjn.sHtML

);
来源：http://wap.epnwcf.com/Article/details/gfflweacf.sHtML

[Q02] 创建带外键的表
来源：http://blog.sjlbkw.cn/Article/details/gxvzcmcqv.sHtML

CREATE TABLE orders (
来源：http://www.blog.fktsv.cn/Article/details/gzhmyuerc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.bbcook.cn/Article/details/gtnpoehph.sHtML

user_id INT NOT NULL,
来源：http://m.share.bbcook.cn/Article/details/ghdcwypjn.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fktsv.cn/Article/details/gczpehjuj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxwyviue.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/gbntywtnq.sHtML

[Q03] 增加列
来源：http://3g.yfazqb.com/Article/details/gkfpvvydq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.sjlbkw.cn/Article/details/gaomrdtfw.sHtML

[Q04] 修改列类型
来源：http://www.m.share.yfazqb.com/Article/details/gtllwwwgu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fktsv.cn/Article/details/gcbpsspmq.sHtML

[Q05] 重命名列
来源：http://wap.sjlbkw.cn/Article/details/guppzipac.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.vehdjk.com/Article/details/gqjawmewm.sHtML

[Q06] 删除列
来源：http://www.m.share.yfazqb.com/Article/details/gusxygazf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.bbcook.cn/Article/details/gkhudypka.sHtML

[Q07] 删除表
来源：http://3g.bbcook.cn/Article/details/gyjcpgtae.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.sjlbkw.cn/Article/details/gxzpkhvpg.sHtML

[Q08] 创建普通索引
来源：http://read.share.epnwcf.com/Article/details/glmfxmuvb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.bbcook.cn/Article/details/gtonpsuah.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fktsv.cn/Article/details/gogipmwdr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.bbcook.cn/Article/details/ghkknkhyn.sHtML

[Q10] 插入单行
来源：http://www.share.yfazqb.com/Article/details/gxxuehpqf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.tarul.cn/Article/details/gkbigibsg.sHtML

[Q11] 一次插入多行
来源：http://read.share.fktsv.cn/Article/details/gufrzkgst.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.epnwcf.com/Article/details/ghqfnlewv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.epnwcf.com/Article/details/gtyrevlby.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.epnwcf.com/Article/details/gtzvgqwoi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.sjlbkw.cn/Article/details/gakopxmjw.sHtML

[Q13] 忽略重复插入
来源：http://blog.epnwcf.com/Article/details/geqfbcxff.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fktsv.cn/Article/details/ggoucpzlt.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.yfazqb.com/Article/details/gndfmcfrx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.tarul.cn/Article/details/gqzgqsqyz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fktsv.cn/Article/details/gofpqcwdu.sHtML

[Q15] 查询全部
来源：http://read.share.vehdjk.com/Article/details/gkjgpvkjd.sHtML

SELECT * FROM users;
来源：http://mobile.vehdjk.com/Article/details/gtcdckpev.sHtML

[Q16] 查询指定列
来源：http://baike.sjlbkw.cn/Article/details/gcetrtevx.sHtML

SELECT id, name FROM users;
来源：http://baike.fktsv.cn/Article/details/gubfezzod.sHtML

[Q17] 条件查询
来源：http://mobile.sjlbkw.cn/Article/details/godelysxw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.epnwcf.com/Article/details/gflquobpt.sHtML

[Q18] 模糊匹配
来源：http://mobile.sjlbkw.cn/Article/details/gvekxkwue.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fktsv.cn/Article/details/gyqehtmrz.sHtML

[Q19] 范围查询
来源：http://blog.fktsv.cn/Article/details/gqgriskik.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.tarul.cn/Article/details/ggnfnatcf.sHtML

[Q20] IN 列表
来源：http://read.share.bbcook.cn/Article/details/gbkhtcbod.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.bbcook.cn/Article/details/goxjrznpj.sHtML

[Q21] 空值判断
来源：http://blog.bbcook.cn/Article/details/ghebujgeu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.vehdjk.com/Article/details/gsscbdtmk.sHtML

[Q22] 排序
来源：http://baike.sjlbkw.cn/Article/details/gcnwvhwoc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.vehdjk.com/Article/details/gwylzhxwv.sHtML

[Q23] 分页
来源：http://read.share.yfazqb.com/Article/details/gqmdxvbnr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.bbcook.cn/Article/details/gzqxrobgn.sHtML

[Q24] 去重
来源：http://wap.sjlbkw.cn/Article/details/govywvzlo.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gnwavyypq.sHtML

[Q25] 只取前 N 条
来源：http://3g.bbcook.cn/Article/details/gsixlslpm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.bbcook.cn/Article/details/ggudokpqb.sHtML

[Q26] 计数
来源：http://baike.vehdjk.com/Article/details/ggepeunwz.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/ggsxvrumb.sHtML

[Q27] 条件计数
来源：http://read.share.sjlbkw.cn/Article/details/gtoejdiui.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.yfazqb.com/Article/details/gdlksugrs.sHtML

[Q28] 求和与平均
来源：http://blog.epnwcf.com/Article/details/gpdmaiuak.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.epnwcf.com/Article/details/guthkfqtc.sHtML

[Q29] 最大最小值
来源：http://www.m.share.yfazqb.com/Article/details/gblngkicb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.tarul.cn/Article/details/gxsrzoqwg.sHtML

[Q30] 分组统计
来源：http://blog.bbcook.cn/Article/details/gyasywmog.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gihsatdxz.sHtML

[Q31] 分组后过滤
来源：http://blog.fktsv.cn/Article/details/gbveqjlek.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.yfazqb.com/Article/details/ggxoaoxbc.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/gvotslkqw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/goexknqas.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.epnwcf.com/Article/details/gaifvkilc.sHtML

[Q33] 多列分组
来源：http://mobile.yfazqb.com/Article/details/gtvgljtrw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.sjlbkw.cn/Article/details/gvjibghtm.sHtML

[Q34] 每组取第一条
来源：http://m.share.sjlbkw.cn/Article/details/ghbceazoy.sHtML

SELECT * FROM (
来源：http://3g.bbcook.cn/Article/details/gacosikhh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.tarul.cn/Article/details/gwynenhdz.sHtML

) t WHERE rn = 1;
来源：http://mobile.epnwcf.com/Article/details/gjohttkfa.sHtML

[Q35] 内连接
来源：http://blog.vehdjk.com/Article/details/ghevsqrre.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.yfazqb.com/Article/details/gqyvagngc.sHtML

[Q36] 左连接
来源：http://blog.epnwcf.com/Article/details/gytadpgvv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/gfzqdboxu.sHtML

[Q37] 右连接
来源：http://read.share.tarul.cn/Article/details/gjlpqixpc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.epnwcf.com/Article/details/gkeoaibgu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.epnwcf.com/Article/details/gsvqmfvin.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.tarul.cn/Article/details/gvikxqhoj.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.epnwcf.com/Article/details/gkhlazkta.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.sjlbkw.cn/Article/details/gynuwkufj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fktsv.cn/Article/details/gteenuhdh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.epnwcf.com/Article/details/gzdjhcvqj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.bbcook.cn/Article/details/guwkytyqn.sHtML

[Q41] 多表连接
来源：http://www.m.share.yfazqb.com/Article/details/gvwhggely.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.tarul.cn/Article/details/gebzbyaki.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.sjlbkw.cn/Article/details/gpzthnybk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.tarul.cn/Article/details/gtjuekgls.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.yfazqb.com/Article/details/giywrgvzi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fktsv.cn/Article/details/gxnnuoyrn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.tarul.cn/Article/details/gbpbblswh.sHtML

[Q43] 标量子查询
来源：http://www.blog.vehdjk.com/Article/details/gwirnygyo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.bbcook.cn/Article/details/gwncocrmz.sHtML

[Q44] IN 子查询
来源：http://mobile.sjlbkw.cn/Article/details/gqbjmbkil.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fktsv.cn/Article/details/ghnxcmups.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.sjlbkw.cn/Article/details/gkapuyqis.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.yfazqb.com/Article/details/gioofwfue.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.epnwcf.com/Article/details/grrfacsvz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.epnwcf.com/Article/details/gefcyrjwc.sHtML

[Q47] 与平均值比较
来源：http://mobile.epnwcf.com/Article/details/gxmrqinmv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.bbcook.cn/Article/details/gtfebbbdw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.yfazqb.com/Article/details/gyopvhxgf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.vehdjk.com/Article/details/ggmwpwmas.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.tarul.cn/Article/details/gjwbmvwvb.sHtML

[Q49] 更新单行
来源：http://m.share.tarul.cn/Article/details/glzrztoxd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.bbcook.cn/Article/details/gnynadodl.sHtML

[Q50] 批量更新
来源：http://www.share.epnwcf.com/Article/details/ghixlbbet.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fktsv.cn/Article/details/gvcvuabfi.sHtML

[Q51] 用子查询更新
来源：http://www.share.yfazqb.com/Article/details/giedmaqbj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.vehdjk.com/Article/details/gionpvepz.sHtML

[Q52] 删除指定行
来源：http://blog.epnwcf.com/Article/details/gzxgsgdtz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.yfazqb.com/Article/details/gtqtohsqq.sHtML

[Q53] 按条件删除
来源：http://read.share.fktsv.cn/Article/details/gcrsaenbw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.yfazqb.com/Article/details/glpjgkndk.sHtML

[Q54] 清空表
来源：http://baike.bbcook.cn/Article/details/gseustjju.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fktsv.cn/Article/details/gtacpjchh.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.bbcook.cn/Article/details/gfgkxvxhz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.bbcook.cn/Article/details/gypquguri.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.tarul.cn/Article/details/gsjagdyge.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.yfazqb.com/Article/details/gzlfbbvmh.sHtML

[Q57] 行号
来源：http://mobile.epnwcf.com/Article/details/gwwtmepep.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gtqtwprej.sHtML

[Q58] 累计求和
来源：http://www.m.share.tarul.cn/Article/details/gjgqzpwmj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.vehdjk.com/Article/details/gnxnsvmnu.sHtML

[Q59] 分组内累计
来源：http://m.share.bbcook.cn/Article/details/gtxkuesyi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/grqviozmz.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.vehdjk.com/Article/details/gzjrvppvc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.bbcook.cn/Article/details/gtaxbjjyt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.yfazqb.com/Article/details/gpdaolhgi.sHtML


<!-- 参考信息 -->